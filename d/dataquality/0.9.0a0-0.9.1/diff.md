# Comparing `tmp/dataquality-0.9.0a0.tar.gz` & `tmp/dataquality-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataquality-0.9.0a0.tar", last modified: Fri Jun 23 16:27:27 2023, max compression
+gzip compressed data, was "dataquality-0.9.1.tar", last modified: Fri Jun 23 17:22:35 2023, max compression
```

## Comparing `dataquality-0.9.0a0.tar` & `dataquality-0.9.1.tar`

### file list

```diff
@@ -1,161 +1,161 @@
-drwxr-xr-x   0 franz      (501) staff       (20)        0 2023-06-23 16:27:27.793130 dataquality-0.9.0a0/
--rw-r--r--   0 franz      (501) staff       (20)     1066 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/LICENSE
--rw-r--r--   0 franz      (501) staff       (20)     4939 2023-06-23 16:27:27.793340 dataquality-0.9.0a0/PKG-INFO
--rw-r--r--   0 franz      (501) staff       (20)     4429 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/README.md
-drwxr-xr-x   0 franz      (501) staff       (20)        0 2023-06-23 16:27:27.703515 dataquality-0.9.0a0/dataquality/
--rw-r--r--   0 franz      (501) staff       (20)     6071 2023-06-23 16:27:08.000000 dataquality-0.9.0a0/dataquality/__init__.py
--rw-r--r--   0 franz      (501) staff       (20)     8300 2023-06-23 16:26:44.000000 dataquality-0.9.0a0/dataquality/analytics.py
-drwxr-xr-x   0 franz      (501) staff       (20)        0 2023-06-23 16:27:27.707654 dataquality-0.9.0a0/dataquality/clients/
--rw-r--r--   0 franz      (501) staff       (20)        0 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/clients/__init__.py
--rw-r--r--   0 franz      (501) staff       (20)    33222 2023-06-21 17:17:50.000000 dataquality-0.9.0a0/dataquality/clients/api.py
--rw-r--r--   0 franz      (501) staff       (20)     8187 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/clients/objectstore.py
-drwxr-xr-x   0 franz      (501) staff       (20)        0 2023-06-23 16:27:27.710400 dataquality-0.9.0a0/dataquality/core/
--rw-r--r--   0 franz      (501) staff       (20)     1848 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/core/__init__.py
--rw-r--r--   0 franz      (501) staff       (20)     9495 2023-06-21 17:17:50.000000 dataquality-0.9.0a0/dataquality/core/_config.py
--rw-r--r--   0 franz      (501) staff       (20)     3104 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/core/auth.py
--rw-r--r--   0 franz      (501) staff       (20)     6499 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/core/finish.py
--rw-r--r--   0 franz      (501) staff       (20)     9615 2023-06-21 17:17:50.000000 dataquality-0.9.0a0/dataquality/core/init.py
--rw-r--r--   0 franz      (501) staff       (20)    23390 2023-06-21 17:17:50.000000 dataquality-0.9.0a0/dataquality/core/log.py
--rw-r--r--   0 franz      (501) staff       (20)     7039 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/core/report.py
-drwxr-xr-x   0 franz      (501) staff       (20)        0 2023-06-23 16:27:27.714469 dataquality-0.9.0a0/dataquality/dq_auto/
--rw-r--r--   0 franz      (501) staff       (20)        0 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/dq_auto/__init__.py
--rw-r--r--   0 franz      (501) staff       (20)    10048 2023-06-21 17:17:50.000000 dataquality-0.9.0a0/dataquality/dq_auto/auto.py
--rw-r--r--   0 franz      (501) staff       (20)     4699 2023-06-21 17:17:50.000000 dataquality-0.9.0a0/dataquality/dq_auto/base_data_manager.py
--rw-r--r--   0 franz      (501) staff       (20)     7430 2023-06-21 17:17:50.000000 dataquality-0.9.0a0/dataquality/dq_auto/ner.py
--rw-r--r--   0 franz      (501) staff       (20)     4265 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/dq_auto/ner_trainer.py
--rw-r--r--   0 franz      (501) staff       (20)     1594 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/dq_auto/notebook.py
--rw-r--r--   0 franz      (501) staff       (20)     3559 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/dq_auto/tc_trainer.py
--rw-r--r--   0 franz      (501) staff       (20)    10676 2023-06-21 17:17:50.000000 dataquality-0.9.0a0/dataquality/dq_auto/text_classification.py
-drwxr-xr-x   0 franz      (501) staff       (20)        0 2023-06-23 16:27:27.715032 dataquality-0.9.0a0/dataquality/dq_start/
--rw-r--r--   0 franz      (501) staff       (20)    11313 2023-06-23 16:26:44.000000 dataquality-0.9.0a0/dataquality/dq_start/__init__.py
--rw-r--r--   0 franz      (501) staff       (20)     4512 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/dqyolo.py
--rw-r--r--   0 franz      (501) staff       (20)      293 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/exceptions.py
-drwxr-xr-x   0 franz      (501) staff       (20)        0 2023-06-23 16:27:27.719267 dataquality-0.9.0a0/dataquality/integrations/
--rw-r--r--   0 franz      (501) staff       (20)        0 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/integrations/__init__.py
--rw-r--r--   0 franz      (501) staff       (20)    14966 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/integrations/fastai.py
--rw-r--r--   0 franz      (501) staff       (20)    10024 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/integrations/hf.py
--rw-r--r--   0 franz      (501) staff       (20)    15575 2023-06-23 16:26:44.000000 dataquality-0.9.0a0/dataquality/integrations/keras.py
--rw-r--r--   0 franz      (501) staff       (20)    14309 2023-06-21 17:17:50.000000 dataquality-0.9.0a0/dataquality/integrations/setfit.py
--rw-r--r--   0 franz      (501) staff       (20)    13302 2023-06-23 16:26:44.000000 dataquality-0.9.0a0/dataquality/integrations/torch.py
--rw-r--r--   0 franz      (501) staff       (20)    27174 2023-06-23 16:26:44.000000 dataquality-0.9.0a0/dataquality/integrations/torch_semantic_segmentation.py
--rw-r--r--   0 franz      (501) staff       (20)    13430 2023-06-23 16:26:44.000000 dataquality-0.9.0a0/dataquality/integrations/transformers_trainer.py
--rw-r--r--   0 franz      (501) staff       (20)    17147 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/integrations/ultralytics.py
--rw-r--r--   0 franz      (501) staff       (20)     4165 2023-06-21 17:17:50.000000 dataquality-0.9.0a0/dataquality/internal.py
-drwxr-xr-x   0 franz      (501) staff       (20)        0 2023-06-23 16:27:27.720398 dataquality-0.9.0a0/dataquality/loggers/
--rw-r--r--   0 franz      (501) staff       (20)       95 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/loggers/__init__.py
--rw-r--r--   0 franz      (501) staff       (20)    13410 2023-06-21 17:17:50.000000 dataquality-0.9.0a0/dataquality/loggers/base_logger.py
-drwxr-xr-x   0 franz      (501) staff       (20)        0 2023-06-23 16:27:27.724043 dataquality-0.9.0a0/dataquality/loggers/data_logger/
--rw-r--r--   0 franz      (501) staff       (20)      517 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/loggers/data_logger/__init__.py
--rw-r--r--   0 franz      (501) staff       (20)    27255 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/loggers/data_logger/base_data_logger.py
--rw-r--r--   0 franz      (501) staff       (20)    12826 2023-06-23 16:26:44.000000 dataquality-0.9.0a0/dataquality/loggers/data_logger/image_classification.py
--rw-r--r--   0 franz      (501) staff       (20)    10355 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/loggers/data_logger/object_detection.py
--rw-r--r--   0 franz      (501) staff       (20)     5888 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/loggers/data_logger/semantic_segmentation.py
--rw-r--r--   0 franz      (501) staff       (20)     9864 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/loggers/data_logger/tabular_classification.py
--rw-r--r--   0 franz      (501) staff       (20)    21106 2023-06-21 17:17:50.000000 dataquality-0.9.0a0/dataquality/loggers/data_logger/text_classification.py
--rw-r--r--   0 franz      (501) staff       (20)    14941 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/loggers/data_logger/text_multi_label.py
--rw-r--r--   0 franz      (501) staff       (20)    31953 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/loggers/data_logger/text_ner.py
-drwxr-xr-x   0 franz      (501) staff       (20)        0 2023-06-23 16:27:27.729046 dataquality-0.9.0a0/dataquality/loggers/logger_config/
--rw-r--r--   0 franz      (501) staff       (20)        0 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/loggers/logger_config/__init__.py
--rw-r--r--   0 franz      (501) staff       (20)     2042 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/loggers/logger_config/base_logger_config.py
--rw-r--r--   0 franz      (501) staff       (20)      510 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/loggers/logger_config/image_classification.py
--rw-r--r--   0 franz      (501) staff       (20)      537 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/loggers/logger_config/object_detection.py
--rw-r--r--   0 franz      (501) staff       (20)      226 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/loggers/logger_config/semantic_segmentation.py
--rw-r--r--   0 franz      (501) staff       (20)      398 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/loggers/logger_config/tabular_classification.py
--rw-r--r--   0 franz      (501) staff       (20)      958 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/loggers/logger_config/text_classification.py
--rw-r--r--   0 franz      (501) staff       (20)     1510 2023-06-21 17:18:47.000000 dataquality-0.9.0a0/dataquality/loggers/logger_config/text_multi_label.py
--rw-r--r--   0 franz      (501) staff       (20)     1608 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/loggers/logger_config/text_ner.py
-drwxr-xr-x   0 franz      (501) staff       (20)        0 2023-06-23 16:27:27.732480 dataquality-0.9.0a0/dataquality/loggers/model_logger/
--rw-r--r--   0 franz      (501) staff       (20)      420 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/loggers/model_logger/__init__.py
--rw-r--r--   0 franz      (501) staff       (20)     7510 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/loggers/model_logger/base_model_logger.py
--rw-r--r--   0 franz      (501) staff       (20)     3309 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/loggers/model_logger/image_classification.py
--rw-r--r--   0 franz      (501) staff       (20)     9435 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/loggers/model_logger/object_detection.py
--rw-r--r--   0 franz      (501) staff       (20)    11742 2023-06-23 16:26:44.000000 dataquality-0.9.0a0/dataquality/loggers/model_logger/semantic_segmentation.py
--rw-r--r--   0 franz      (501) staff       (20)      519 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/loggers/model_logger/tabular_classification.py
--rw-r--r--   0 franz      (501) staff       (20)     7555 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/loggers/model_logger/text_classification.py
--rw-r--r--   0 franz      (501) staff       (20)     9120 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/loggers/model_logger/text_multi_label.py
--rw-r--r--   0 franz      (501) staff       (20)    32052 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/loggers/model_logger/text_ner.py
--rw-r--r--   0 franz      (501) staff       (20)    28653 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/metrics.py
--rw-r--r--   0 franz      (501) staff       (20)        0 2023-06-21 17:17:50.000000 dataquality-0.9.0a0/dataquality/py.typed
-drwxr-xr-x   0 franz      (501) staff       (20)        0 2023-06-23 16:27:27.746117 dataquality-0.9.0a0/dataquality/schemas/
--rw-r--r--   0 franz      (501) staff       (20)      165 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/schemas/__init__.py
--rw-r--r--   0 franz      (501) staff       (20)     8361 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/schemas/condition.py
--rw-r--r--   0 franz      (501) staff       (20)      569 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/schemas/dataframe.py
--rw-r--r--   0 franz      (501) staff       (20)     4382 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/schemas/edit.py
--rw-r--r--   0 franz      (501) staff       (20)      662 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/schemas/hf.py
--rw-r--r--   0 franz      (501) staff       (20)      118 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/schemas/job.py
--rw-r--r--   0 franz      (501) staff       (20)     5241 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/schemas/metrics.py
--rw-r--r--   0 franz      (501) staff       (20)      145 2023-06-23 16:26:44.000000 dataquality-0.9.0a0/dataquality/schemas/model.py
--rw-r--r--   0 franz      (501) staff       (20)      992 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/schemas/ner.py
--rw-r--r--   0 franz      (501) staff       (20)      617 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/schemas/report.py
--rw-r--r--   0 franz      (501) staff       (20)      287 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/schemas/request_type.py
--rw-r--r--   0 franz      (501) staff       (20)     1495 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/schemas/route.py
--rw-r--r--   0 franz      (501) staff       (20)     4190 2023-06-23 16:26:44.000000 dataquality-0.9.0a0/dataquality/schemas/semantic_segmentation.py
--rw-r--r--   0 franz      (501) staff       (20)      992 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/schemas/split.py
--rw-r--r--   0 franz      (501) staff       (20)     1295 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/schemas/task_type.py
--rw-r--r--   0 franz      (501) staff       (20)      740 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/schemas/torch.py
-drwxr-xr-x   0 franz      (501) staff       (20)        0 2023-06-23 16:27:27.772433 dataquality-0.9.0a0/dataquality/utils/
--rw-r--r--   0 franz      (501) staff       (20)      222 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/utils/__init__.py
--rw-r--r--   0 franz      (501) staff       (20)      634 2023-06-23 16:26:44.000000 dataquality-0.9.0a0/dataquality/utils/ampli.py
--rw-r--r--   0 franz      (501) staff       (20)      401 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/utils/auth.py
--rw-r--r--   0 franz      (501) staff       (20)     8903 2023-06-21 17:17:50.000000 dataquality-0.9.0a0/dataquality/utils/auto.py
--rw-r--r--   0 franz      (501) staff       (20)      925 2023-06-21 17:17:50.000000 dataquality-0.9.0a0/dataquality/utils/auto_trainer.py
--rw-r--r--   0 franz      (501) staff       (20)      154 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/utils/cloud.py
--rw-r--r--   0 franz      (501) staff       (20)     1229 2023-06-21 17:17:50.000000 dataquality-0.9.0a0/dataquality/utils/cuda.py
--rw-r--r--   0 franz      (501) staff       (20)     2082 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/utils/cv.py
--rw-r--r--   0 franz      (501) staff       (20)     3387 2023-06-21 17:17:50.000000 dataquality-0.9.0a0/dataquality/utils/dq_logger.py
--rw-r--r--   0 franz      (501) staff       (20)     3514 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/utils/dqyolo.py
--rw-r--r--   0 franz      (501) staff       (20)     4898 2023-06-21 17:17:50.000000 dataquality-0.9.0a0/dataquality/utils/emb.py
--rw-r--r--   0 franz      (501) staff       (20)     3591 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/utils/file.py
--rw-r--r--   0 franz      (501) staff       (20)     5685 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/utils/hdf5_store.py
--rw-r--r--   0 franz      (501) staff       (20)     3784 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/utils/helpers.py
--rw-r--r--   0 franz      (501) staff       (20)     2163 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/utils/hf_images.py
--rw-r--r--   0 franz      (501) staff       (20)    10182 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/utils/hf_tokenizer.py
--rw-r--r--   0 franz      (501) staff       (20)      429 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/utils/imports.py
--rw-r--r--   0 franz      (501) staff       (20)     8023 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/utils/keras.py
--rw-r--r--   0 franz      (501) staff       (20)     2408 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/utils/ml.py
--rw-r--r--   0 franz      (501) staff       (20)    24732 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/utils/name.py
--rw-r--r--   0 franz      (501) staff       (20)     1661 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/utils/od.py
--rw-r--r--   0 franz      (501) staff       (20)     3187 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/utils/patcher.py
--rw-r--r--   0 franz      (501) staff       (20)     5923 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/utils/profiler.py
-drwxr-xr-x   0 franz      (501) staff       (20)        0 2023-06-23 16:27:27.778864 dataquality-0.9.0a0/dataquality/utils/semantic_segmentation/
--rw-r--r--   0 franz      (501) staff       (20)        0 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/utils/semantic_segmentation/__init__.py
--rw-r--r--   0 franz      (501) staff       (20)       43 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/utils/semantic_segmentation/constants.py
--rw-r--r--   0 franz      (501) staff       (20)    10033 2023-06-23 16:26:44.000000 dataquality-0.9.0a0/dataquality/utils/semantic_segmentation/errors.py
--rw-r--r--   0 franz      (501) staff       (20)    11898 2023-06-21 17:17:50.000000 dataquality-0.9.0a0/dataquality/utils/semantic_segmentation/lm.py
--rw-r--r--   0 franz      (501) staff       (20)    10144 2023-06-23 16:26:44.000000 dataquality-0.9.0a0/dataquality/utils/semantic_segmentation/metrics.py
--rw-r--r--   0 franz      (501) staff       (20)     5309 2023-06-23 16:26:44.000000 dataquality-0.9.0a0/dataquality/utils/semantic_segmentation/polygons.py
--rw-r--r--   0 franz      (501) staff       (20)     1914 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/utils/semantic_segmentation/utils.py
--rw-r--r--   0 franz      (501) staff       (20)    15187 2023-06-21 17:17:50.000000 dataquality-0.9.0a0/dataquality/utils/setfit.py
--rw-r--r--   0 franz      (501) staff       (20)      260 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/utils/tf.py
--rw-r--r--   0 franz      (501) staff       (20)     1987 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/utils/thread_pool.py
--rw-r--r--   0 franz      (501) staff       (20)    24980 2023-06-23 16:26:44.000000 dataquality-0.9.0a0/dataquality/utils/torch.py
--rw-r--r--   0 franz      (501) staff       (20)     5087 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/utils/transformers.py
--rw-r--r--   0 franz      (501) staff       (20)    12825 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/utils/ultralytics.py
--rw-r--r--   0 franz      (501) staff       (20)     5597 2023-06-21 17:17:50.000000 dataquality-0.9.0a0/dataquality/utils/upload.py
--rw-r--r--   0 franz      (501) staff       (20)    10670 2023-06-21 17:17:50.000000 dataquality-0.9.0a0/dataquality/utils/vaex.py
--rw-r--r--   0 franz      (501) staff       (20)     1087 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/utils/version.py
-drwxr-xr-x   0 franz      (501) staff       (20)        0 2023-06-23 16:27:27.706319 dataquality-0.9.0a0/dataquality.egg-info/
--rw-r--r--   0 franz      (501) staff       (20)     4939 2023-06-23 16:27:27.000000 dataquality-0.9.0a0/dataquality.egg-info/PKG-INFO
--rw-r--r--   0 franz      (501) staff       (20)     5079 2023-06-23 16:27:27.000000 dataquality-0.9.0a0/dataquality.egg-info/SOURCES.txt
--rw-r--r--   0 franz      (501) staff       (20)        1 2023-06-23 16:27:27.000000 dataquality-0.9.0a0/dataquality.egg-info/dependency_links.txt
--rw-r--r--   0 franz      (501) staff       (20)       51 2023-06-23 16:27:27.000000 dataquality-0.9.0a0/dataquality.egg-info/entry_points.txt
--rw-r--r--   0 franz      (501) staff       (20)     1293 2023-06-23 16:27:27.000000 dataquality-0.9.0a0/dataquality.egg-info/requires.txt
--rw-r--r--   0 franz      (501) staff       (20)       18 2023-06-23 16:27:27.000000 dataquality-0.9.0a0/dataquality.egg-info/top_level.txt
--rw-r--r--   0 franz      (501) staff       (20)     3847 2023-06-23 16:26:44.000000 dataquality-0.9.0a0/pyproject.toml
--rw-r--r--   0 franz      (501) staff       (20)      293 2023-06-23 16:27:27.794154 dataquality-0.9.0a0/setup.cfg
--rw-r--r--   0 franz      (501) staff       (20)       38 2023-06-21 17:17:50.000000 dataquality-0.9.0a0/setup.py
-drwxr-xr-x   0 franz      (501) staff       (20)        0 2023-06-23 16:27:27.781134 dataquality-0.9.0a0/tests/
--rw-r--r--   0 franz      (501) staff       (20)    31396 2023-06-21 17:17:50.000000 dataquality-0.9.0a0/tests/test_dataquality.py
--rw-r--r--   0 franz      (501) staff       (20)     1783 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/tests/test_telemetrics.py
-drwxr-xr-x   0 franz      (501) staff       (20)        0 2023-06-23 16:27:27.792454 dataquality-0.9.0a0/tests/test_utils/
--rw-r--r--   0 franz      (501) staff       (20)        0 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/tests/test_utils/__init__.py
--rw-r--r--   0 franz      (501) staff       (20)     6129 2023-06-21 17:17:50.000000 dataquality-0.9.0a0/tests/test_utils/data_utils.py
--rw-r--r--   0 franz      (501) staff       (20)     1692 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/tests/test_utils/hf_datasets_mock.py
--rw-r--r--   0 franz      (501) staff       (20)    11616 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/tests/test_utils/hf_integration_constants.py
--rw-r--r--   0 franz      (501) staff       (20)     8122 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/tests/test_utils/hf_integration_constants_inference.py
--rw-r--r--   0 franz      (501) staff       (20)     3695 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/tests/test_utils/lightning_model.py
--rw-r--r--   0 franz      (501) staff       (20)     3017 2023-06-23 16:26:44.000000 dataquality-0.9.0a0/tests/test_utils/mock_data.py
--rw-r--r--   0 franz      (501) staff       (20)     5594 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/tests/test_utils/mock_request.py
--rw-r--r--   0 franz      (501) staff       (20)     2840 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/tests/test_utils/ner_constants.py
--rw-r--r--   0 franz      (501) staff       (20)      863 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/tests/test_utils/pt_datasets_mock.py
--rw-r--r--   0 franz      (501) staff       (20)     7910 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/tests/test_utils/tc_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:22:35.340109 dataquality-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-23 17:21:15.000000 dataquality-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-06-23 17:22:35.340109 dataquality-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-06-23 17:21:15.000000 dataquality-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:22:35.284109 dataquality-0.9.1/dataquality/
+-rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/analytics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:22:35.288109 dataquality-0.9.1/dataquality/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33222 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/clients/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8187 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/clients/objectstore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:22:35.288109 dataquality-0.9.1/dataquality/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9495 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/core/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/core/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6499 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/core/finish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9615 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/core/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23390 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/core/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7039 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/core/report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:22:35.292109 dataquality-0.9.1/dataquality/dq_auto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/dq_auto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10048 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/dq_auto/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/dq_auto/base_data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/dq_auto/ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/dq_auto/ner_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/dq_auto/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/dq_auto/tc_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10676 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/dq_auto/text_classification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:22:35.292109 dataquality-0.9.1/dataquality/dq_start/
+-rw-r--r--   0 runner    (1001) docker     (123)    11313 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/dq_start/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4512 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/dqyolo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:22:35.296109 dataquality-0.9.1/dataquality/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/integrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/integrations/fastai.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10024 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/integrations/hf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/integrations/keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14309 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/integrations/setfit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13302 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/integrations/torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27174 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/integrations/torch_semantic_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13430 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/integrations/transformers_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17147 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/integrations/ultralytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/internal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:22:35.300109 dataquality-0.9.1/dataquality/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13410 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/loggers/base_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:22:35.304109 dataquality-0.9.1/dataquality/loggers/data_logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/loggers/data_logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27255 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/loggers/data_logger/base_data_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12826 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/loggers/data_logger/image_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10355 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/loggers/data_logger/object_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/loggers/data_logger/semantic_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9864 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/loggers/data_logger/tabular_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21106 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/loggers/data_logger/text_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14941 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/loggers/data_logger/text_multi_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31953 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/loggers/data_logger/text_ner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:22:35.308109 dataquality-0.9.1/dataquality/loggers/logger_config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/loggers/logger_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/loggers/logger_config/base_logger_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/loggers/logger_config/image_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/loggers/logger_config/object_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/loggers/logger_config/semantic_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/loggers/logger_config/tabular_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/loggers/logger_config/text_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/loggers/logger_config/text_multi_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/loggers/logger_config/text_ner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:22:35.308109 dataquality-0.9.1/dataquality/loggers/model_logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/loggers/model_logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7510 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/loggers/model_logger/base_model_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/loggers/model_logger/image_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9435 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/loggers/model_logger/object_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11742 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/loggers/model_logger/semantic_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/loggers/model_logger/tabular_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7555 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/loggers/model_logger/text_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9120 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/loggers/model_logger/text_multi_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32052 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/loggers/model_logger/text_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28653 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:22:35.316109 dataquality-0.9.1/dataquality/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/schemas/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/schemas/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/schemas/edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/schemas/hf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/schemas/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/schemas/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/schemas/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/schemas/ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/schemas/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/schemas/request_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/schemas/route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/schemas/semantic_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/schemas/split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/schemas/task_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/schemas/torch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:22:35.332110 dataquality-0.9.1/dataquality/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/utils/ampli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/utils/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8903 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/utils/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/utils/auto_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/utils/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/utils/cuda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/utils/cv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/utils/dq_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/utils/dqyolo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/utils/emb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/utils/hdf5_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/utils/hf_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10182 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/utils/hf_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/utils/imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8023 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/utils/keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/utils/ml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24732 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/utils/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/utils/od.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/utils/patcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/utils/profiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:22:35.332110 dataquality-0.9.1/dataquality/utils/semantic_segmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/utils/semantic_segmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/utils/semantic_segmentation/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10033 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/utils/semantic_segmentation/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11898 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/utils/semantic_segmentation/lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10144 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/utils/semantic_segmentation/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/utils/semantic_segmentation/polygons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/utils/semantic_segmentation/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15187 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/utils/setfit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/utils/tf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/utils/thread_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24980 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/utils/torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/utils/transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12825 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/utils/ultralytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/utils/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10670 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/utils/vaex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-23 17:21:15.000000 dataquality-0.9.1/dataquality/utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:22:35.284109 dataquality-0.9.1/dataquality.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-06-23 17:22:35.000000 dataquality-0.9.1/dataquality.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-06-23 17:22:35.000000 dataquality-0.9.1/dataquality.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 17:22:35.000000 dataquality-0.9.1/dataquality.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-23 17:22:35.000000 dataquality-0.9.1/dataquality.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-23 17:22:35.000000 dataquality-0.9.1/dataquality.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-23 17:22:35.000000 dataquality-0.9.1/dataquality.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-06-23 17:21:15.000000 dataquality-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-23 17:22:35.340109 dataquality-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 17:21:15.000000 dataquality-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:22:35.336109 dataquality-0.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    31396 2023-06-23 17:21:15.000000 dataquality-0.9.1/tests/test_dataquality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-23 17:21:15.000000 dataquality-0.9.1/tests/test_telemetrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:22:35.340109 dataquality-0.9.1/tests/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 17:21:15.000000 dataquality-0.9.1/tests/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-06-23 17:21:15.000000 dataquality-0.9.1/tests/test_utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-06-23 17:21:15.000000 dataquality-0.9.1/tests/test_utils/hf_datasets_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11616 2023-06-23 17:21:15.000000 dataquality-0.9.1/tests/test_utils/hf_integration_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-06-23 17:21:15.000000 dataquality-0.9.1/tests/test_utils/hf_integration_constants_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-06-23 17:21:15.000000 dataquality-0.9.1/tests/test_utils/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-06-23 17:21:15.000000 dataquality-0.9.1/tests/test_utils/mock_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-06-23 17:21:15.000000 dataquality-0.9.1/tests/test_utils/mock_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-06-23 17:21:15.000000 dataquality-0.9.1/tests/test_utils/ner_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-23 17:21:15.000000 dataquality-0.9.1/tests/test_utils/pt_datasets_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7910 2023-06-23 17:21:15.000000 dataquality-0.9.1/tests/test_utils/tc_constants.py
```

### Comparing `dataquality-0.9.0a0/LICENSE` & `dataquality-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/PKG-INFO` & `dataquality-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataquality
-Version: 0.9.0a0
+Version: 0.9.1
 Author-email: "Galileo Technologies, Inc." <devs+dq@rungalileo.io>
 License: See LICENSE
 Project-URL: Homepage, https://github.com/rungalileo/dataquality
 Project-URL: Documentation, https://rungalileo.gitbook.io/galileo
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: doc
```

### Comparing `dataquality-0.9.0a0/README.md` & `dataquality-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/__init__.py` & `dataquality-0.9.1/dataquality/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     import dataquality
     with dataquality(labels = ["neg", "pos"],
                      train_data = train_data):
         dataquality.get_insights()
 """
 
 
-__version__ = "v0.9.0a0"
+__version__ = "v0.9.1"
 
 import sys
 from typing import Any, List, Optional
 
 import dataquality.core._config
 import dataquality.integrations
```

### Comparing `dataquality-0.9.0a0/dataquality/analytics.py` & `dataquality-0.9.1/dataquality/analytics.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/clients/api.py` & `dataquality-0.9.1/dataquality/clients/api.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/clients/objectstore.py` & `dataquality-0.9.1/dataquality/clients/objectstore.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/core/__init__.py` & `dataquality-0.9.1/dataquality/core/__init__.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/core/_config.py` & `dataquality-0.9.1/dataquality/core/_config.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/core/auth.py` & `dataquality-0.9.1/dataquality/core/auth.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/core/finish.py` & `dataquality-0.9.1/dataquality/core/finish.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/core/init.py` & `dataquality-0.9.1/dataquality/core/init.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/core/log.py` & `dataquality-0.9.1/dataquality/core/log.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/core/report.py` & `dataquality-0.9.1/dataquality/core/report.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/dq_auto/auto.py` & `dataquality-0.9.1/dataquality/dq_auto/auto.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/dq_auto/base_data_manager.py` & `dataquality-0.9.1/dataquality/dq_auto/base_data_manager.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/dq_auto/ner.py` & `dataquality-0.9.1/dataquality/dq_auto/ner.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/dq_auto/ner_trainer.py` & `dataquality-0.9.1/dataquality/dq_auto/ner_trainer.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/dq_auto/notebook.py` & `dataquality-0.9.1/dataquality/dq_auto/notebook.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/dq_auto/tc_trainer.py` & `dataquality-0.9.1/dataquality/dq_auto/tc_trainer.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/dq_auto/text_classification.py` & `dataquality-0.9.1/dataquality/dq_auto/text_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/dq_start/__init__.py` & `dataquality-0.9.1/dataquality/dq_start/__init__.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/dqyolo.py` & `dataquality-0.9.1/dataquality/dqyolo.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/integrations/fastai.py` & `dataquality-0.9.1/dataquality/integrations/fastai.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/integrations/hf.py` & `dataquality-0.9.1/dataquality/integrations/hf.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/integrations/keras.py` & `dataquality-0.9.1/dataquality/integrations/keras.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/integrations/setfit.py` & `dataquality-0.9.1/dataquality/integrations/setfit.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/integrations/torch.py` & `dataquality-0.9.1/dataquality/integrations/torch.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/integrations/torch_semantic_segmentation.py` & `dataquality-0.9.1/dataquality/integrations/torch_semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/integrations/transformers_trainer.py` & `dataquality-0.9.1/dataquality/integrations/transformers_trainer.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/integrations/ultralytics.py` & `dataquality-0.9.1/dataquality/integrations/ultralytics.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/internal.py` & `dataquality-0.9.1/dataquality/internal.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/loggers/base_logger.py` & `dataquality-0.9.1/dataquality/loggers/base_logger.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/loggers/data_logger/__init__.py` & `dataquality-0.9.1/dataquality/loggers/data_logger/__init__.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/loggers/data_logger/base_data_logger.py` & `dataquality-0.9.1/dataquality/loggers/data_logger/base_data_logger.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/loggers/data_logger/image_classification.py` & `dataquality-0.9.1/dataquality/loggers/data_logger/image_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/loggers/data_logger/object_detection.py` & `dataquality-0.9.1/dataquality/loggers/data_logger/object_detection.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/loggers/data_logger/semantic_segmentation.py` & `dataquality-0.9.1/dataquality/loggers/data_logger/semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/loggers/data_logger/tabular_classification.py` & `dataquality-0.9.1/dataquality/loggers/data_logger/tabular_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/loggers/data_logger/text_classification.py` & `dataquality-0.9.1/dataquality/loggers/data_logger/text_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/loggers/data_logger/text_multi_label.py` & `dataquality-0.9.1/dataquality/loggers/data_logger/text_multi_label.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/loggers/data_logger/text_ner.py` & `dataquality-0.9.1/dataquality/loggers/data_logger/text_ner.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/loggers/logger_config/base_logger_config.py` & `dataquality-0.9.1/dataquality/loggers/logger_config/base_logger_config.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/loggers/logger_config/object_detection.py` & `dataquality-0.9.1/dataquality/loggers/logger_config/object_detection.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/loggers/logger_config/text_classification.py` & `dataquality-0.9.1/dataquality/loggers/logger_config/text_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/loggers/logger_config/text_multi_label.py` & `dataquality-0.9.1/dataquality/loggers/logger_config/text_multi_label.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/loggers/logger_config/text_ner.py` & `dataquality-0.9.1/dataquality/loggers/logger_config/text_ner.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/loggers/model_logger/base_model_logger.py` & `dataquality-0.9.1/dataquality/loggers/model_logger/base_model_logger.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/loggers/model_logger/image_classification.py` & `dataquality-0.9.1/dataquality/loggers/model_logger/image_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/loggers/model_logger/object_detection.py` & `dataquality-0.9.1/dataquality/loggers/model_logger/object_detection.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/loggers/model_logger/semantic_segmentation.py` & `dataquality-0.9.1/dataquality/loggers/model_logger/semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/loggers/model_logger/tabular_classification.py` & `dataquality-0.9.1/dataquality/loggers/model_logger/tabular_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/loggers/model_logger/text_classification.py` & `dataquality-0.9.1/dataquality/loggers/model_logger/text_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/loggers/model_logger/text_multi_label.py` & `dataquality-0.9.1/dataquality/loggers/model_logger/text_multi_label.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/loggers/model_logger/text_ner.py` & `dataquality-0.9.1/dataquality/loggers/model_logger/text_ner.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/metrics.py` & `dataquality-0.9.1/dataquality/metrics.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/schemas/condition.py` & `dataquality-0.9.1/dataquality/schemas/condition.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/schemas/dataframe.py` & `dataquality-0.9.1/dataquality/schemas/dataframe.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/schemas/edit.py` & `dataquality-0.9.1/dataquality/schemas/edit.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/schemas/hf.py` & `dataquality-0.9.1/dataquality/schemas/hf.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/schemas/metrics.py` & `dataquality-0.9.1/dataquality/schemas/metrics.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/schemas/ner.py` & `dataquality-0.9.1/dataquality/schemas/ner.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/schemas/report.py` & `dataquality-0.9.1/dataquality/schemas/report.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/schemas/route.py` & `dataquality-0.9.1/dataquality/schemas/route.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/schemas/semantic_segmentation.py` & `dataquality-0.9.1/dataquality/schemas/semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/schemas/split.py` & `dataquality-0.9.1/dataquality/schemas/split.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/schemas/task_type.py` & `dataquality-0.9.1/dataquality/schemas/task_type.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/schemas/torch.py` & `dataquality-0.9.1/dataquality/schemas/torch.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/utils/ampli.py` & `dataquality-0.9.1/dataquality/utils/ampli.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/utils/auto.py` & `dataquality-0.9.1/dataquality/utils/auto.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/utils/auto_trainer.py` & `dataquality-0.9.1/dataquality/utils/auto_trainer.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/utils/cuda.py` & `dataquality-0.9.1/dataquality/utils/cuda.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/utils/cv.py` & `dataquality-0.9.1/dataquality/utils/cv.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/utils/dq_logger.py` & `dataquality-0.9.1/dataquality/utils/dq_logger.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/utils/dqyolo.py` & `dataquality-0.9.1/dataquality/utils/dqyolo.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/utils/emb.py` & `dataquality-0.9.1/dataquality/utils/emb.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/utils/file.py` & `dataquality-0.9.1/dataquality/utils/file.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/utils/hdf5_store.py` & `dataquality-0.9.1/dataquality/utils/hdf5_store.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/utils/helpers.py` & `dataquality-0.9.1/dataquality/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/utils/hf_images.py` & `dataquality-0.9.1/dataquality/utils/hf_images.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/utils/hf_tokenizer.py` & `dataquality-0.9.1/dataquality/utils/hf_tokenizer.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/utils/keras.py` & `dataquality-0.9.1/dataquality/utils/keras.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/utils/ml.py` & `dataquality-0.9.1/dataquality/utils/ml.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/utils/name.py` & `dataquality-0.9.1/dataquality/utils/name.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/utils/od.py` & `dataquality-0.9.1/dataquality/utils/od.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/utils/patcher.py` & `dataquality-0.9.1/dataquality/utils/patcher.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/utils/profiler.py` & `dataquality-0.9.1/dataquality/utils/profiler.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/utils/semantic_segmentation/errors.py` & `dataquality-0.9.1/dataquality/utils/semantic_segmentation/errors.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/utils/semantic_segmentation/lm.py` & `dataquality-0.9.1/dataquality/utils/semantic_segmentation/lm.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/utils/semantic_segmentation/metrics.py` & `dataquality-0.9.1/dataquality/utils/semantic_segmentation/metrics.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/utils/semantic_segmentation/polygons.py` & `dataquality-0.9.1/dataquality/utils/semantic_segmentation/polygons.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/utils/semantic_segmentation/utils.py` & `dataquality-0.9.1/dataquality/utils/semantic_segmentation/utils.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/utils/setfit.py` & `dataquality-0.9.1/dataquality/utils/setfit.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/utils/thread_pool.py` & `dataquality-0.9.1/dataquality/utils/thread_pool.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/utils/torch.py` & `dataquality-0.9.1/dataquality/utils/torch.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/utils/transformers.py` & `dataquality-0.9.1/dataquality/utils/transformers.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/utils/ultralytics.py` & `dataquality-0.9.1/dataquality/utils/ultralytics.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/utils/upload.py` & `dataquality-0.9.1/dataquality/utils/upload.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/utils/vaex.py` & `dataquality-0.9.1/dataquality/utils/vaex.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality/utils/version.py` & `dataquality-0.9.1/dataquality/utils/version.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality.egg-info/PKG-INFO` & `dataquality-0.9.1/dataquality.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataquality
-Version: 0.9.0a0
+Version: 0.9.1
 Author-email: "Galileo Technologies, Inc." <devs+dq@rungalileo.io>
 License: See LICENSE
 Project-URL: Homepage, https://github.com/rungalileo/dataquality
 Project-URL: Documentation, https://rungalileo.gitbook.io/galileo
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: doc
```

### Comparing `dataquality-0.9.0a0/dataquality.egg-info/SOURCES.txt` & `dataquality-0.9.1/dataquality.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/dataquality.egg-info/requires.txt` & `dataquality-0.9.1/dataquality.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/pyproject.toml` & `dataquality-0.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/tests/test_dataquality.py` & `dataquality-0.9.1/tests/test_dataquality.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/tests/test_telemetrics.py` & `dataquality-0.9.1/tests/test_telemetrics.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/tests/test_utils/data_utils.py` & `dataquality-0.9.1/tests/test_utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/tests/test_utils/hf_datasets_mock.py` & `dataquality-0.9.1/tests/test_utils/hf_datasets_mock.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/tests/test_utils/hf_integration_constants.py` & `dataquality-0.9.1/tests/test_utils/hf_integration_constants.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/tests/test_utils/hf_integration_constants_inference.py` & `dataquality-0.9.1/tests/test_utils/hf_integration_constants_inference.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/tests/test_utils/lightning_model.py` & `dataquality-0.9.1/tests/test_utils/lightning_model.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/tests/test_utils/mock_data.py` & `dataquality-0.9.1/tests/test_utils/mock_data.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/tests/test_utils/mock_request.py` & `dataquality-0.9.1/tests/test_utils/mock_request.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/tests/test_utils/ner_constants.py` & `dataquality-0.9.1/tests/test_utils/ner_constants.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/tests/test_utils/pt_datasets_mock.py` & `dataquality-0.9.1/tests/test_utils/pt_datasets_mock.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.0a0/tests/test_utils/tc_constants.py` & `dataquality-0.9.1/tests/test_utils/tc_constants.py`

 * *Files identical despite different names*

