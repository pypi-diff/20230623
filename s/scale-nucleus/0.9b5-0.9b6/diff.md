# Comparing `tmp/scale-nucleus-0.9b5.tar.gz` & `tmp/scale-nucleus-0.9b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scale-nucleus-0.9b5.tar", max compression
+gzip compressed data, was "scale-nucleus-0.9b6.tar", max compression
```

## Comparing `scale-nucleus-0.9b5.tar` & `scale-nucleus-0.9b6.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0     1075 2021-11-01 11:18:08.763493 scale-nucleus-0.9b5/LICENSE
--rw-r--r--   0        0        0     5570 2022-02-08 13:57:07.225081 scale-nucleus-0.9b5/README.md
--rw-r--r--   0        0        0      286 2022-02-08 13:57:07.225304 scale-nucleus-0.9b5/cli/client.py
--rw-r--r--   0        0        0     2351 2022-02-08 13:57:07.225504 scale-nucleus-0.9b5/cli/datasets.py
--rw-r--r--   0        0        0        0 2022-02-08 13:57:07.225606 scale-nucleus-0.9b5/cli/helpers/__init__.py
--rw-r--r--   0        0        0      317 2022-02-08 13:57:07.225878 scale-nucleus-0.9b5/cli/helpers/nucleus_url.py
--rw-r--r--   0        0        0     1162 2022-02-17 13:38:33.548487 scale-nucleus-0.9b5/cli/helpers/web_helper.py
--rw-r--r--   0        0        0     1166 2022-02-08 13:57:07.226207 scale-nucleus-0.9b5/cli/install_completion.py
--rw-r--r--   0        0        0     1176 2022-02-08 13:57:07.226393 scale-nucleus-0.9b5/cli/jobs.py
--rw-r--r--   0        0        0     1039 2022-02-08 13:57:07.226580 scale-nucleus-0.9b5/cli/models.py
--rw-r--r--   0        0        0     2074 2022-02-08 13:57:07.226770 scale-nucleus-0.9b5/cli/nu.py
--rw-r--r--   0        0        0      256 2022-02-17 13:38:33.549453 scale-nucleus-0.9b5/cli/reference.py
--rw-r--r--   0        0        0     2106 2022-02-08 13:57:07.227241 scale-nucleus-0.9b5/cli/slices.py
--rw-r--r--   0        0        0     4508 2022-03-31 13:40:57.683037 scale-nucleus-0.9b5/cli/tests.py
--rw-r--r--   0        0        0    29231 2022-03-31 13:40:57.684914 scale-nucleus-0.9b5/nucleus/__init__.py
--rw-r--r--   0        0        0    28504 2022-04-04 09:00:46.164286 scale-nucleus-0.9b5/nucleus/annotation.py
--rw-r--r--   0        0        0     8419 2022-03-31 13:40:57.685952 scale-nucleus-0.9b5/nucleus/annotation_uploader.py
--rw-r--r--   0        0        0     6709 2022-03-31 13:40:57.686155 scale-nucleus-0.9b5/nucleus/async_utils.py
--rw-r--r--   0        0        0     1074 2022-01-11 15:52:13.816048 scale-nucleus-0.9b5/nucleus/autocurate.py
--rw-r--r--   0        0        0     2651 2022-03-31 13:40:57.686844 scale-nucleus-0.9b5/nucleus/connection.py
--rw-r--r--   0        0        0     3612 2022-03-31 13:40:57.687466 scale-nucleus-0.9b5/nucleus/constants.py
--rw-r--r--   0        0        0        0 2022-01-11 15:52:13.817671 scale-nucleus-0.9b5/nucleus/data_transfer_object/__init__.py
--rw-r--r--   0        0        0      214 2022-01-11 15:52:13.818314 scale-nucleus-0.9b5/nucleus/data_transfer_object/dataset_details.py
--rw-r--r--   0        0        0      940 2022-01-11 15:52:13.818938 scale-nucleus-0.9b5/nucleus/data_transfer_object/dataset_info.py
--rw-r--r--   0        0        0      111 2022-01-11 15:52:13.819442 scale-nucleus-0.9b5/nucleus/data_transfer_object/dataset_size.py
--rw-r--r--   0        0        0      432 2022-02-08 13:57:07.229151 scale-nucleus-0.9b5/nucleus/data_transfer_object/scenes_list.py
--rw-r--r--   0        0        0    62461 2022-03-31 13:40:57.688510 scale-nucleus-0.9b5/nucleus/dataset.py
--rw-r--r--   0        0        0    12791 2022-03-31 13:40:57.689499 scale-nucleus-0.9b5/nucleus/dataset_item.py
--rw-r--r--   0        0        0     6938 2022-03-31 13:40:57.690123 scale-nucleus-0.9b5/nucleus/dataset_item_uploader.py
--rw-r--r--   0        0        0      976 2022-01-11 15:52:13.821897 scale-nucleus-0.9b5/nucleus/deprecation_warning.py
--rw-r--r--   0        0        0     2730 2022-03-31 13:40:57.690681 scale-nucleus-0.9b5/nucleus/errors.py
--rw-r--r--   0        0        0     4745 2022-03-04 09:22:14.026114 scale-nucleus-0.9b5/nucleus/job.py
--rw-r--r--   0        0        0      208 2022-01-11 15:52:13.824420 scale-nucleus-0.9b5/nucleus/logger.py
--rw-r--r--   0        0        0     1258 2022-02-14 17:08:45.745155 scale-nucleus-0.9b5/nucleus/metadata_manager.py
--rw-r--r--   0        0        0      422 2022-03-31 13:44:03.270897 scale-nucleus-0.9b5/nucleus/metrics/__init__.py
--rw-r--r--   0        0        0     8854 2022-04-04 09:26:49.335491 scale-nucleus-0.9b5/nucleus/metrics/base.py
--rw-r--r--   0        0        0    11790 2022-04-04 09:28:12.039894 scale-nucleus-0.9b5/nucleus/metrics/categorization_metrics.py
--rw-r--r--   0        0        0    12461 2022-04-04 08:19:22.821822 scale-nucleus-0.9b5/nucleus/metrics/cuboid_metrics.py
--rw-r--r--   0        0        0    11093 2022-03-31 13:43:54.130285 scale-nucleus-0.9b5/nucleus/metrics/cuboid_utils.py
--rw-r--r--   0        0        0      251 2022-01-14 10:54:22.021293 scale-nucleus-0.9b5/nucleus/metrics/errors.py
--rw-r--r--   0        0        0    11896 2022-04-04 09:23:13.572224 scale-nucleus-0.9b5/nucleus/metrics/filtering.py
--rw-r--r--   0        0        0     1146 2022-02-08 13:57:07.231467 scale-nucleus-0.9b5/nucleus/metrics/filters.py
--rw-r--r--   0        0        0     5390 2022-02-14 17:08:45.746126 scale-nucleus-0.9b5/nucleus/metrics/geometry.py
--rw-r--r--   0        0        0      971 2022-02-08 13:57:07.232258 scale-nucleus-0.9b5/nucleus/metrics/metric_utils.py
--rw-r--r--   0        0        0    29143 2022-04-04 09:29:20.352663 scale-nucleus-0.9b5/nucleus/metrics/polygon_metrics.py
--rw-r--r--   0        0        0    11642 2022-03-22 13:25:23.317068 scale-nucleus-0.9b5/nucleus/metrics/polygon_utils.py
--rw-r--r--   0        0        0     6253 2022-02-14 17:08:45.747326 scale-nucleus-0.9b5/nucleus/model.py
--rw-r--r--   0        0        0     9482 2022-03-31 13:40:57.692482 scale-nucleus-0.9b5/nucleus/model_run.py
--rw-r--r--   0        0        0     4174 2022-03-31 13:40:57.693130 scale-nucleus-0.9b5/nucleus/payload_constructor.py
--rw-r--r--   0        0        0    21200 2022-04-04 08:42:07.614017 scale-nucleus-0.9b5/nucleus/prediction.py
--rw-r--r--   0        0        0      682 2022-02-08 13:57:07.236794 scale-nucleus-0.9b5/nucleus/pydantic_base.py
--rw-r--r--   0        0        0      312 2022-03-31 13:40:57.694305 scale-nucleus-0.9b5/nucleus/retry_strategy.py
--rw-r--r--   0        0        0    21399 2022-03-31 13:40:57.694894 scale-nucleus-0.9b5/nucleus/scene.py
--rw-r--r--   0        0        0    12926 2022-03-31 13:40:57.695550 scale-nucleus-0.9b5/nucleus/slice.py
--rw-r--r--   0        0        0     3287 2022-01-11 15:52:13.837469 scale-nucleus-0.9b5/nucleus/upload_response.py
--rw-r--r--   0        0        0      790 2022-01-11 15:52:13.838289 scale-nucleus-0.9b5/nucleus/url_utils.py
--rw-r--r--   0        0        0    10568 2022-03-31 13:40:57.696157 scale-nucleus-0.9b5/nucleus/utils.py
--rw-r--r--   0        0        0      695 2022-02-14 17:08:45.749355 scale-nucleus-0.9b5/nucleus/validate/__init__.py
--rw-r--r--   0        0        0     6277 2022-03-31 13:44:03.247386 scale-nucleus-0.9b5/nucleus/validate/client.py
--rw-r--r--   0        0        0      633 2022-03-31 13:40:57.697612 scale-nucleus-0.9b5/nucleus/validate/constants.py
--rw-r--r--   0        0        0        0 2022-02-14 17:08:45.750375 scale-nucleus-0.9b5/nucleus/validate/data_transfer_objects/__init__.py
--rw-r--r--   0        0        0     3150 2022-03-31 13:44:03.273558 scale-nucleus-0.9b5/nucleus/validate/data_transfer_objects/eval_function.py
--rw-r--r--   0        0        0      574 2022-03-31 13:44:03.274629 scale-nucleus-0.9b5/nucleus/validate/data_transfer_objects/scenario_test.py
--rw-r--r--   0        0        0      196 2022-02-14 17:08:45.823521 scale-nucleus-0.9b5/nucleus/validate/data_transfer_objects/scenario_test_evaluations.py
--rw-r--r--   0        0        0      208 2022-03-31 13:40:57.700775 scale-nucleus-0.9b5/nucleus/validate/data_transfer_objects/scenario_test_metric.py
--rw-r--r--   0        0        0      110 2022-03-30 11:35:10.506041 scale-nucleus-0.9b5/nucleus/validate/errors.py
--rw-r--r--   0        0        0        0 2022-02-14 17:08:45.752853 scale-nucleus-0.9b5/nucleus/validate/eval_functions/__init__.py
--rw-r--r--   0        0        0    36107 2022-04-04 10:09:55.347282 scale-nucleus-0.9b5/nucleus/validate/eval_functions/available_eval_functions.py
--rw-r--r--   0        0        0     2207 2022-03-31 13:44:03.252310 scale-nucleus-0.9b5/nucleus/validate/eval_functions/base_eval_function.py
--rw-r--r--   0        0        0     6581 2022-03-31 13:40:57.703833 scale-nucleus-0.9b5/nucleus/validate/scenario_test.py
--rw-r--r--   0        0        0     4316 2022-02-17 13:38:33.555798 scale-nucleus-0.9b5/nucleus/validate/scenario_test_evaluation.py
--rw-r--r--   0        0        0     1209 2022-03-31 13:40:57.704662 scale-nucleus-0.9b5/nucleus/validate/scenario_test_metric.py
--rw-r--r--   0        0        0      172 2022-02-14 17:08:45.813140 scale-nucleus-0.9b5/nucleus/validate/utils.py
--rw-r--r--   0        0        0     1851 2022-04-04 10:10:19.323707 scale-nucleus-0.9b5/pyproject.toml
--rw-r--r--   0        0        0     7153 2022-04-04 10:18:40.009224 scale-nucleus-0.9b5/setup.py
--rw-r--r--   0        0        0     6923 2022-04-04 10:18:40.009669 scale-nucleus-0.9b5/PKG-INFO
+-rw-r--r--   0        0        0     1075 2021-11-01 11:18:08.763493 scale-nucleus-0.9b6/LICENSE
+-rw-r--r--   0        0        0     5948 2022-04-05 10:48:36.333423 scale-nucleus-0.9b6/README.md
+-rw-r--r--   0        0        0      286 2022-02-08 13:57:07.225304 scale-nucleus-0.9b6/cli/client.py
+-rw-r--r--   0        0        0     2351 2022-02-08 13:57:07.225504 scale-nucleus-0.9b6/cli/datasets.py
+-rw-r--r--   0        0        0        0 2022-02-08 13:57:07.225606 scale-nucleus-0.9b6/cli/helpers/__init__.py
+-rw-r--r--   0        0        0      317 2022-02-08 13:57:07.225878 scale-nucleus-0.9b6/cli/helpers/nucleus_url.py
+-rw-r--r--   0        0        0     1162 2022-02-17 13:38:33.548487 scale-nucleus-0.9b6/cli/helpers/web_helper.py
+-rw-r--r--   0        0        0     1166 2022-02-08 13:57:07.226207 scale-nucleus-0.9b6/cli/install_completion.py
+-rw-r--r--   0        0        0     1176 2022-02-08 13:57:07.226393 scale-nucleus-0.9b6/cli/jobs.py
+-rw-r--r--   0        0        0     1039 2022-02-08 13:57:07.226580 scale-nucleus-0.9b6/cli/models.py
+-rw-r--r--   0        0        0     2074 2022-02-08 13:57:07.226770 scale-nucleus-0.9b6/cli/nu.py
+-rw-r--r--   0        0        0      256 2022-02-17 13:38:33.549453 scale-nucleus-0.9b6/cli/reference.py
+-rw-r--r--   0        0        0     2106 2022-02-08 13:57:07.227241 scale-nucleus-0.9b6/cli/slices.py
+-rw-r--r--   0        0        0     4508 2022-03-31 13:40:57.683037 scale-nucleus-0.9b6/cli/tests.py
+-rw-r--r--   0        0        0    29231 2022-03-31 13:40:57.684914 scale-nucleus-0.9b6/nucleus/__init__.py
+-rw-r--r--   0        0        0    28569 2022-04-04 13:40:22.081098 scale-nucleus-0.9b6/nucleus/annotation.py
+-rw-r--r--   0        0        0     8419 2022-03-31 13:40:57.685952 scale-nucleus-0.9b6/nucleus/annotation_uploader.py
+-rw-r--r--   0        0        0     6709 2022-03-31 13:40:57.686155 scale-nucleus-0.9b6/nucleus/async_utils.py
+-rw-r--r--   0        0        0     1074 2022-01-11 15:52:13.816048 scale-nucleus-0.9b6/nucleus/autocurate.py
+-rw-r--r--   0        0        0     2651 2022-03-31 13:40:57.686844 scale-nucleus-0.9b6/nucleus/connection.py
+-rw-r--r--   0        0        0     3612 2022-03-31 13:40:57.687466 scale-nucleus-0.9b6/nucleus/constants.py
+-rw-r--r--   0        0        0        0 2022-01-11 15:52:13.817671 scale-nucleus-0.9b6/nucleus/data_transfer_object/__init__.py
+-rw-r--r--   0        0        0      214 2022-01-11 15:52:13.818314 scale-nucleus-0.9b6/nucleus/data_transfer_object/dataset_details.py
+-rw-r--r--   0        0        0      940 2022-01-11 15:52:13.818938 scale-nucleus-0.9b6/nucleus/data_transfer_object/dataset_info.py
+-rw-r--r--   0        0        0      111 2022-01-11 15:52:13.819442 scale-nucleus-0.9b6/nucleus/data_transfer_object/dataset_size.py
+-rw-r--r--   0        0        0      432 2022-02-08 13:57:07.229151 scale-nucleus-0.9b6/nucleus/data_transfer_object/scenes_list.py
+-rw-r--r--   0        0        0    62461 2022-03-31 13:40:57.688510 scale-nucleus-0.9b6/nucleus/dataset.py
+-rw-r--r--   0        0        0    12791 2022-03-31 13:40:57.689499 scale-nucleus-0.9b6/nucleus/dataset_item.py
+-rw-r--r--   0        0        0     6938 2022-03-31 13:40:57.690123 scale-nucleus-0.9b6/nucleus/dataset_item_uploader.py
+-rw-r--r--   0        0        0      976 2022-01-11 15:52:13.821897 scale-nucleus-0.9b6/nucleus/deprecation_warning.py
+-rw-r--r--   0        0        0     2730 2022-03-31 13:40:57.690681 scale-nucleus-0.9b6/nucleus/errors.py
+-rw-r--r--   0        0        0     4745 2022-03-04 09:22:14.026114 scale-nucleus-0.9b6/nucleus/job.py
+-rw-r--r--   0        0        0      208 2022-01-11 15:52:13.824420 scale-nucleus-0.9b6/nucleus/logger.py
+-rw-r--r--   0        0        0     1258 2022-02-14 17:08:45.745155 scale-nucleus-0.9b6/nucleus/metadata_manager.py
+-rw-r--r--   0        0        0      422 2022-04-05 11:01:38.534453 scale-nucleus-0.9b6/nucleus/metrics/__init__.py
+-rw-r--r--   0        0        0     8928 2022-04-05 15:04:19.737319 scale-nucleus-0.9b6/nucleus/metrics/base.py
+-rw-r--r--   0        0        0    11790 2022-04-04 09:28:12.039894 scale-nucleus-0.9b6/nucleus/metrics/categorization_metrics.py
+-rw-r--r--   0        0        0    12461 2022-04-04 08:19:22.821822 scale-nucleus-0.9b6/nucleus/metrics/cuboid_metrics.py
+-rw-r--r--   0        0        0    12204 2022-04-05 11:07:11.224226 scale-nucleus-0.9b6/nucleus/metrics/cuboid_utils.py
+-rw-r--r--   0        0        0      251 2022-01-14 10:54:22.021293 scale-nucleus-0.9b6/nucleus/metrics/errors.py
+-rw-r--r--   0        0        0    12608 2022-04-04 13:45:54.463286 scale-nucleus-0.9b6/nucleus/metrics/filtering.py
+-rw-r--r--   0        0        0     1146 2022-02-08 13:57:07.231467 scale-nucleus-0.9b6/nucleus/metrics/filters.py
+-rw-r--r--   0        0        0     5390 2022-02-14 17:08:45.746126 scale-nucleus-0.9b6/nucleus/metrics/geometry.py
+-rw-r--r--   0        0        0      971 2022-02-08 13:57:07.232258 scale-nucleus-0.9b6/nucleus/metrics/metric_utils.py
+-rw-r--r--   0        0        0    29143 2022-04-04 09:29:20.352663 scale-nucleus-0.9b6/nucleus/metrics/polygon_metrics.py
+-rw-r--r--   0        0        0    11642 2022-03-22 13:25:23.317068 scale-nucleus-0.9b6/nucleus/metrics/polygon_utils.py
+-rw-r--r--   0        0        0     6253 2022-02-14 17:08:45.747326 scale-nucleus-0.9b6/nucleus/model.py
+-rw-r--r--   0        0        0     9482 2022-03-31 13:40:57.692482 scale-nucleus-0.9b6/nucleus/model_run.py
+-rw-r--r--   0        0        0     4174 2022-03-31 13:40:57.693130 scale-nucleus-0.9b6/nucleus/payload_constructor.py
+-rw-r--r--   0        0        0    21222 2022-04-04 13:32:21.106678 scale-nucleus-0.9b6/nucleus/prediction.py
+-rw-r--r--   0        0        0      682 2022-02-08 13:57:07.236794 scale-nucleus-0.9b6/nucleus/pydantic_base.py
+-rw-r--r--   0        0        0      312 2022-03-31 13:40:57.694305 scale-nucleus-0.9b6/nucleus/retry_strategy.py
+-rw-r--r--   0        0        0    21399 2022-03-31 13:40:57.694894 scale-nucleus-0.9b6/nucleus/scene.py
+-rw-r--r--   0        0        0    12926 2022-03-31 13:40:57.695550 scale-nucleus-0.9b6/nucleus/slice.py
+-rw-r--r--   0        0        0     3287 2022-01-11 15:52:13.837469 scale-nucleus-0.9b6/nucleus/upload_response.py
+-rw-r--r--   0        0        0      790 2022-01-11 15:52:13.838289 scale-nucleus-0.9b6/nucleus/url_utils.py
+-rw-r--r--   0        0        0    10568 2022-03-31 13:40:57.696157 scale-nucleus-0.9b6/nucleus/utils.py
+-rw-r--r--   0        0        0      695 2022-02-14 17:08:45.749355 scale-nucleus-0.9b6/nucleus/validate/__init__.py
+-rw-r--r--   0        0        0     6277 2022-03-31 13:44:03.247386 scale-nucleus-0.9b6/nucleus/validate/client.py
+-rw-r--r--   0        0        0      633 2022-03-31 13:40:57.697612 scale-nucleus-0.9b6/nucleus/validate/constants.py
+-rw-r--r--   0        0        0        0 2022-02-14 17:08:45.750375 scale-nucleus-0.9b6/nucleus/validate/data_transfer_objects/__init__.py
+-rw-r--r--   0        0        0     3150 2022-03-31 13:44:03.273558 scale-nucleus-0.9b6/nucleus/validate/data_transfer_objects/eval_function.py
+-rw-r--r--   0        0        0      574 2022-03-31 13:44:03.274629 scale-nucleus-0.9b6/nucleus/validate/data_transfer_objects/scenario_test.py
+-rw-r--r--   0        0        0      196 2022-02-14 17:08:45.823521 scale-nucleus-0.9b6/nucleus/validate/data_transfer_objects/scenario_test_evaluations.py
+-rw-r--r--   0        0        0      208 2022-03-31 13:40:57.700775 scale-nucleus-0.9b6/nucleus/validate/data_transfer_objects/scenario_test_metric.py
+-rw-r--r--   0        0        0      110 2022-03-30 11:35:10.506041 scale-nucleus-0.9b6/nucleus/validate/errors.py
+-rw-r--r--   0        0        0        0 2022-02-14 17:08:45.752853 scale-nucleus-0.9b6/nucleus/validate/eval_functions/__init__.py
+-rw-r--r--   0        0        0    36107 2022-04-04 10:09:55.347282 scale-nucleus-0.9b6/nucleus/validate/eval_functions/available_eval_functions.py
+-rw-r--r--   0        0        0     2207 2022-03-31 13:44:03.252310 scale-nucleus-0.9b6/nucleus/validate/eval_functions/base_eval_function.py
+-rw-r--r--   0        0        0     6581 2022-03-31 13:40:57.703833 scale-nucleus-0.9b6/nucleus/validate/scenario_test.py
+-rw-r--r--   0        0        0     4316 2022-02-17 13:38:33.555798 scale-nucleus-0.9b6/nucleus/validate/scenario_test_evaluation.py
+-rw-r--r--   0        0        0     1209 2022-03-31 13:40:57.704662 scale-nucleus-0.9b6/nucleus/validate/scenario_test_metric.py
+-rw-r--r--   0        0        0      172 2022-02-14 17:08:45.813140 scale-nucleus-0.9b6/nucleus/validate/utils.py
+-rw-r--r--   0        0        0     1928 2022-04-05 15:05:16.557535 scale-nucleus-0.9b6/pyproject.toml
+-rw-r--r--   0        0        0     7556 2022-04-05 15:06:12.596748 scale-nucleus-0.9b6/setup.py
+-rw-r--r--   0        0        0     7338 2022-04-05 15:06:12.597221 scale-nucleus-0.9b6/PKG-INFO
```

### Comparing `scale-nucleus-0.9b5/LICENSE` & `scale-nucleus-0.9b6/LICENSE`

 * *Files identical despite different names*

### Comparing `scale-nucleus-0.9b5/README.md` & `scale-nucleus-0.9b6/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -175,7 +175,26 @@
 To test your local docstring changes, run the following commands from the repository's root directory:
 ```
 poetry shell
 cd docs
 sphinx-autobuild . ./_build/html --watch ../nucleus
 ```
 `sphinx-autobuild` will spin up a server on localhost (port 8000 by default) that will watch for and automatically rebuild a version of the API reference based on your local docstring changes.
+
+
+## Custom Metrics used in Scale Validate
+
+To install the availalbe metrics for Scale Validate add the optional `metrics` extra.
+Note that you might need to install a local GEOS package.
+
+```bash
+#Mac OS
+brew install geos
+# Ubuntu/Debian flavors
+apt-get install libgeos-dev
+```
+
+`pip install scale-nucleus[metrics]`
+
+To develop it locally use
+
+`poetry install --extra metrics`
```

### Comparing `scale-nucleus-0.9b5/cli/datasets.py` & `scale-nucleus-0.9b6/cli/datasets.py`

 * *Files identical despite different names*

### Comparing `scale-nucleus-0.9b5/cli/helpers/web_helper.py` & `scale-nucleus-0.9b6/cli/helpers/web_helper.py`

 * *Files identical despite different names*

### Comparing `scale-nucleus-0.9b5/cli/install_completion.py` & `scale-nucleus-0.9b6/cli/install_completion.py`

 * *Files identical despite different names*

### Comparing `scale-nucleus-0.9b5/cli/jobs.py` & `scale-nucleus-0.9b6/cli/jobs.py`

 * *Files identical despite different names*

### Comparing `scale-nucleus-0.9b5/cli/models.py` & `scale-nucleus-0.9b6/cli/models.py`

 * *Files identical despite different names*

### Comparing `scale-nucleus-0.9b5/cli/nu.py` & `scale-nucleus-0.9b6/cli/nu.py`

 * *Files identical despite different names*

### Comparing `scale-nucleus-0.9b5/cli/slices.py` & `scale-nucleus-0.9b6/cli/slices.py`

 * *Files identical despite different names*

### Comparing `scale-nucleus-0.9b5/cli/tests.py` & `scale-nucleus-0.9b6/cli/tests.py`

 * *Files identical despite different names*

### Comparing `scale-nucleus-0.9b5/nucleus/__init__.py` & `scale-nucleus-0.9b6/nucleus/__init__.py`

 * *Files identical despite different names*

### Comparing `scale-nucleus-0.9b5/nucleus/annotation.py` & `scale-nucleus-0.9b6/nucleus/annotation.py`

 * *Files 1% similar despite different names*

```diff
@@ -553,15 +553,15 @@
           to an external database, and its value will be returned for any export.
     """
 
     mask_url: str
     annotations: List[Segment]
     reference_id: str
     annotation_id: Optional[str] = None
-    metadata: Optional[dict] = None
+    # metadata: Optional[dict] = None # TODO(sc: 422637)
 
     def __post_init__(self):
         if not self.mask_url:
             raise Exception("You must specify a mask_url.")
 
     @classmethod
     def from_json(cls, payload: dict):
@@ -571,24 +571,24 @@
             mask_url=payload[MASK_URL_KEY],
             annotations=[
                 Segment.from_json(ann)
                 for ann in payload.get(ANNOTATIONS_KEY, [])
             ],
             reference_id=payload[REFERENCE_ID_KEY],
             annotation_id=payload.get(ANNOTATION_ID_KEY, None),
-            metadata=payload.get(METADATA_KEY, None),
+            # metadata=payload.get(METADATA_KEY, None),  # TODO(sc: 422637)
         )
 
     def to_payload(self) -> dict:
         payload = {
             TYPE_KEY: MASK_TYPE,
             MASK_URL_KEY: self.mask_url,
             ANNOTATIONS_KEY: [ann.to_payload() for ann in self.annotations],
             ANNOTATION_ID_KEY: self.annotation_id,
-            METADATA_KEY: self.metadata,
+            # METADATA_KEY: self.metadata,  # TODO(sc: 422637)
         }
 
         payload[REFERENCE_ID_KEY] = self.reference_id
 
         return payload
 
     def has_local_files_to_upload(self) -> bool:
```

### Comparing `scale-nucleus-0.9b5/nucleus/annotation_uploader.py` & `scale-nucleus-0.9b6/nucleus/annotation_uploader.py`

 * *Files identical despite different names*

### Comparing `scale-nucleus-0.9b5/nucleus/async_utils.py` & `scale-nucleus-0.9b6/nucleus/async_utils.py`

 * *Files identical despite different names*

### Comparing `scale-nucleus-0.9b5/nucleus/autocurate.py` & `scale-nucleus-0.9b6/nucleus/autocurate.py`

 * *Files identical despite different names*

### Comparing `scale-nucleus-0.9b5/nucleus/connection.py` & `scale-nucleus-0.9b6/nucleus/connection.py`

 * *Files identical despite different names*

### Comparing `scale-nucleus-0.9b5/nucleus/constants.py` & `scale-nucleus-0.9b6/nucleus/constants.py`

 * *Files identical despite different names*

### Comparing `scale-nucleus-0.9b5/nucleus/data_transfer_object/dataset_info.py` & `scale-nucleus-0.9b6/nucleus/data_transfer_object/dataset_info.py`

 * *Files identical despite different names*

### Comparing `scale-nucleus-0.9b5/nucleus/dataset.py` & `scale-nucleus-0.9b6/nucleus/dataset.py`

 * *Files identical despite different names*

### Comparing `scale-nucleus-0.9b5/nucleus/dataset_item.py` & `scale-nucleus-0.9b6/nucleus/dataset_item.py`

 * *Files identical despite different names*

### Comparing `scale-nucleus-0.9b5/nucleus/dataset_item_uploader.py` & `scale-nucleus-0.9b6/nucleus/dataset_item_uploader.py`

 * *Files identical despite different names*

### Comparing `scale-nucleus-0.9b5/nucleus/deprecation_warning.py` & `scale-nucleus-0.9b6/nucleus/deprecation_warning.py`

 * *Files identical despite different names*

### Comparing `scale-nucleus-0.9b5/nucleus/errors.py` & `scale-nucleus-0.9b6/nucleus/errors.py`

 * *Files identical despite different names*

### Comparing `scale-nucleus-0.9b5/nucleus/job.py` & `scale-nucleus-0.9b6/nucleus/job.py`

 * *Files identical despite different names*

### Comparing `scale-nucleus-0.9b5/nucleus/metadata_manager.py` & `scale-nucleus-0.9b6/nucleus/metadata_manager.py`

 * *Files identical despite different names*

### Comparing `scale-nucleus-0.9b5/nucleus/metrics/base.py` & `scale-nucleus-0.9b6/nucleus/metrics/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,18 @@
         self, annotations: AnnotationList, predictions: PredictionList
     ) -> MetricResult:
         annotations = self._filter_annotations(annotations)
         predictions = self._filter_predictions(predictions)
         return self.call_metric(annotations, predictions)
 
     def _filter_annotations(self, annotations: AnnotationList):
-        if self.annotation_filters is None or len(self.annotation_filters) > 0:
+        if (
+            self.annotation_filters is None
+            or len(self.annotation_filters) == 0
+        ):
             return annotations
         annotations.box_annotations = apply_filters(
             annotations.box_annotations, self.annotation_filters
         )
         annotations.line_annotations = apply_filters(
             annotations.line_annotations, self.annotation_filters
         )
@@ -160,15 +163,18 @@
         )
         annotations.segmentation_annotations = apply_filters(
             annotations.segmentation_annotations, self.annotation_filters
         )
         return annotations
 
     def _filter_predictions(self, predictions: PredictionList):
-        if self.prediction_filters is None or len(self.prediction_filters) > 0:
+        if (
+            self.prediction_filters is None
+            or len(self.prediction_filters) == 0
+        ):
             return predictions
         predictions.box_predictions = apply_filters(
             predictions.box_predictions, self.prediction_filters
         )
         predictions.line_predictions = apply_filters(
             predictions.line_predictions, self.prediction_filters
         )
```

### Comparing `scale-nucleus-0.9b5/nucleus/metrics/categorization_metrics.py` & `scale-nucleus-0.9b6/nucleus/metrics/categorization_metrics.py`

 * *Files identical despite different names*

### Comparing `scale-nucleus-0.9b5/nucleus/metrics/cuboid_metrics.py` & `scale-nucleus-0.9b6/nucleus/metrics/cuboid_metrics.py`

 * *Files identical despite different names*

### Comparing `scale-nucleus-0.9b5/nucleus/metrics/cuboid_utils.py` & `scale-nucleus-0.9b6/nucleus/metrics/cuboid_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,37 @@
 from functools import wraps
 from typing import Dict, List, Tuple
 
 import numpy as np
-from shapely.geometry import Polygon
+
+try:
+    from shapely.geometry import Polygon
+except ModuleNotFoundError:
+    import sys
+
+    class Polygon:  # type: ignore
+        def __init__(self, *args, **kwargs):
+            """Object to make sure we only raise errors if actually trying to use shapely"""
+            if sys.platform.startswith("darwin"):
+                platform_specific_msg = (
+                    "Depending on Python environment used GEOS might need to be installed via "
+                    "`brew install geos`."
+                )
+            elif sys.platform.startswith("linux"):
+                platform_specific_msg = (
+                    "Depending on Python environment used GEOS might need to be installed via "
+                    "system package `libgeos-dev`."
+                )
+            else:
+                platform_specific_msg = "GEOS package will need to be installed see (https://trac.osgeo.org/geos/)"
+            raise ModuleNotFoundError(
+                f"Module 'shapely' not found. Install optionally with `scale-nucleus[shapely]` or when developing "
+                f"`poetry install -E shapely`. {platform_specific_msg}"
+            )
+
 
 from nucleus.annotation import CuboidAnnotation
 from nucleus.prediction import CuboidPrediction
 
 from .base import ScalarResult
```

### Comparing `scale-nucleus-0.9b5/nucleus/metrics/filtering.py` & `scale-nucleus-0.9b6/nucleus/metrics/filtering.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import enum
 import functools
+import logging
 from enum import Enum
 from typing import Callable, Iterable, List, NamedTuple, Sequence, Set, Union
 
 from nucleus.annotation import (
     BoxAnnotation,
     CategoryAnnotation,
     CuboidAnnotation,
@@ -137,48 +138,53 @@
     op: Union[FilterOp, str]
     value: FilterableTypes
     allow_missing: bool = False
     type: FilterType = FilterType.METADATA
 
 
 Filter = Union[FieldFilter, MetadataFilter, AnnotationOrPredictionFilter]
-DNFFilters = List[List[Filter]]
-DNFFilters.__doc__ = """\
+OrAndDNFFilters = List[List[Filter]]
+OrAndDNFFilters.__doc__ = """\
 Disjunctive normal form (DNF) filters.
 DNF allows arbitrary boolean logical combinations of single field predicates.
 The innermost structures each describe a single field predicate.
 
 The list of inner predicates is interpreted as a conjunction (AND), forming a more selective and multiple column
 predicate.
 
 Finally, the most outer list combines these filters as a disjunction (OR).
 """
-ListOfOrAndFilters = Union[DNFFilters, List[List[List]]]
-ListOfOrAndFilters.__doc__ = """\
+ListOfOrAndJSONSerialized = List[List[List]]
+ListOfOrAndJSONSerialized.__doc__ = """\
+JSON serialized form of DNFFilters. The innermost list has to be trivially expandable (*list) to a
+:class:`AnnotationOrPredictionFilter`.
+
 Disjunctive normal form (DNF) filters.
 DNF allows arbitrary boolean logical combinations of single field predicates.
 The innermost structures each describe a single field predicate.
     -The list of inner predicates is interpreted as a conjunction (AND), forming a more selective and multiple column
      predicate.
     -Finally, the most outer list combines these filters as a disjunction (OR).
 
-If providing a triple nested list the innermost list has to be trivially expandable (*list) to a
-:class:`AnnotationOrPredictionFilter`
+
 """
-ListOfAndFilters = Union[
-    List[Filter],
-    List[List],
-]
-ListOfAndFilters.__doc__ = """\
+ListOfOrAndFilters = Union[OrAndDNFFilters, ListOfOrAndJSONSerialized]
+ListOfAndJSONSerialized = List[List]
+ListOfAndFilterTuple = List[Filter]
+ListOfAndFilterTuple.__doc__ = """\
 List of AND filters.
 The list of predicates is interpreted as a conjunction (AND), forming a multiple field predicate.
 
 If providing a doubly nested list the innermost list has to be trivially expandable (*list) to a
 :class:`AnnotationOrPredictionFilter`
 """
+ListOfAndFilters = Union[
+    ListOfAndFilterTuple,
+    ListOfAndJSONSerialized,
+]
 
 
 def _attribute_getter(
     field_name: str,
     allow_missing: bool,
     ann_or_pred: Union[AnnotationTypes, PredictionTypes],
 ):
@@ -217,14 +223,28 @@
 
 def _metadata_field_getter(
     field_name: str,
     allow_missing: bool,
     ann_or_pred: Union[AnnotationTypes, PredictionTypes],
 ):
     """Create a function to get a metadata field"""
+    if isinstance(
+        ann_or_pred, (SegmentationAnnotation, SegmentationPrediction)
+    ):
+        if allow_missing:
+            logging.warning(
+                "Trying to filter metadata on SegmentationAnnotation or Prediction. "
+                "This will never work until metadata is supported for this format."
+            )
+            return AlwaysFalseComparison()
+        else:
+            raise RuntimeError(
+                f"{type(ann_or_pred)} doesn't support metadata filtering"
+            )
+
     if allow_missing:
         return (
             ann_or_pred.metadata.get(field_name, AlwaysFalseComparison())
             if ann_or_pred.metadata
             else AlwaysFalseComparison()
         )
     else:
@@ -317,15 +337,15 @@
         for or_conditions in dnf_condition_functions:
             if all(c(item) for c in or_conditions):
                 filtered.append(item)
                 break
     return filtered
 
 
-def ensureDNFFilters(filters) -> DNFFilters:
+def ensureDNFFilters(filters) -> OrAndDNFFilters:
     """JSON encoding creates a triple nested lists from the doubly nested tuples. This function creates the
     tuple form again."""
     if isinstance(filters[0], (MetadataFilter, FieldFilter)):
         # Normalize into DNF
         filters: ListOfOrAndFilters = [filters]  # type: ignore
 
     # NOTE: We have to handle JSON transformed tuples which become two or three layers of lists
```

### Comparing `scale-nucleus-0.9b5/nucleus/metrics/filters.py` & `scale-nucleus-0.9b6/nucleus/metrics/filters.py`

 * *Files identical despite different names*

### Comparing `scale-nucleus-0.9b5/nucleus/metrics/geometry.py` & `scale-nucleus-0.9b6/nucleus/metrics/geometry.py`

 * *Files identical despite different names*

### Comparing `scale-nucleus-0.9b5/nucleus/metrics/metric_utils.py` & `scale-nucleus-0.9b6/nucleus/metrics/metric_utils.py`

 * *Files identical despite different names*

### Comparing `scale-nucleus-0.9b5/nucleus/metrics/polygon_metrics.py` & `scale-nucleus-0.9b6/nucleus/metrics/polygon_metrics.py`

 * *Files identical despite different names*

### Comparing `scale-nucleus-0.9b5/nucleus/metrics/polygon_utils.py` & `scale-nucleus-0.9b6/nucleus/metrics/polygon_utils.py`

 * *Files identical despite different names*

### Comparing `scale-nucleus-0.9b5/nucleus/model.py` & `scale-nucleus-0.9b6/nucleus/model.py`

 * *Files identical despite different names*

### Comparing `scale-nucleus-0.9b5/nucleus/model_run.py` & `scale-nucleus-0.9b6/nucleus/model_run.py`

 * *Files identical despite different names*

### Comparing `scale-nucleus-0.9b5/nucleus/payload_constructor.py` & `scale-nucleus-0.9b6/nucleus/payload_constructor.py`

 * *Files identical despite different names*

### Comparing `scale-nucleus-0.9b5/nucleus/prediction.py` & `scale-nucleus-0.9b6/nucleus/prediction.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,15 +116,15 @@
             mask_url=payload[MASK_URL_KEY],
             annotations=[
                 Segment.from_json(ann)
                 for ann in payload.get(ANNOTATIONS_KEY, [])
             ],
             reference_id=payload[REFERENCE_ID_KEY],
             annotation_id=payload.get(ANNOTATION_ID_KEY, None),
-            metadata=payload.get(METADATA_KEY, None),
+            # metadata=payload.get(METADATA_KEY, None),  # TODO(sc: 422637)
         )
 
 
 class BoxPrediction(BoxAnnotation):
     """Prediction of a bounding box.
 
     Parameters:
```

### Comparing `scale-nucleus-0.9b5/nucleus/pydantic_base.py` & `scale-nucleus-0.9b6/nucleus/pydantic_base.py`

 * *Files identical despite different names*

### Comparing `scale-nucleus-0.9b5/nucleus/scene.py` & `scale-nucleus-0.9b6/nucleus/scene.py`

 * *Files identical despite different names*

### Comparing `scale-nucleus-0.9b5/nucleus/slice.py` & `scale-nucleus-0.9b6/nucleus/slice.py`

 * *Files identical despite different names*

### Comparing `scale-nucleus-0.9b5/nucleus/upload_response.py` & `scale-nucleus-0.9b6/nucleus/upload_response.py`

 * *Files identical despite different names*

### Comparing `scale-nucleus-0.9b5/nucleus/url_utils.py` & `scale-nucleus-0.9b6/nucleus/url_utils.py`

 * *Files identical despite different names*

### Comparing `scale-nucleus-0.9b5/nucleus/utils.py` & `scale-nucleus-0.9b6/nucleus/utils.py`

 * *Files identical despite different names*

### Comparing `scale-nucleus-0.9b5/nucleus/validate/__init__.py` & `scale-nucleus-0.9b6/nucleus/validate/__init__.py`

 * *Files identical despite different names*

### Comparing `scale-nucleus-0.9b5/nucleus/validate/client.py` & `scale-nucleus-0.9b6/nucleus/validate/client.py`

 * *Files identical despite different names*

### Comparing `scale-nucleus-0.9b5/nucleus/validate/constants.py` & `scale-nucleus-0.9b6/nucleus/validate/constants.py`

 * *Files identical despite different names*

### Comparing `scale-nucleus-0.9b5/nucleus/validate/data_transfer_objects/eval_function.py` & `scale-nucleus-0.9b6/nucleus/validate/data_transfer_objects/eval_function.py`

 * *Files identical despite different names*

### Comparing `scale-nucleus-0.9b5/nucleus/validate/data_transfer_objects/scenario_test.py` & `scale-nucleus-0.9b6/nucleus/validate/data_transfer_objects/scenario_test.py`

 * *Files identical despite different names*

### Comparing `scale-nucleus-0.9b5/nucleus/validate/eval_functions/available_eval_functions.py` & `scale-nucleus-0.9b6/nucleus/validate/eval_functions/available_eval_functions.py`

 * *Files identical despite different names*

### Comparing `scale-nucleus-0.9b5/nucleus/validate/eval_functions/base_eval_function.py` & `scale-nucleus-0.9b6/nucleus/validate/eval_functions/base_eval_function.py`

 * *Files identical despite different names*

### Comparing `scale-nucleus-0.9b5/nucleus/validate/scenario_test.py` & `scale-nucleus-0.9b6/nucleus/validate/scenario_test.py`

 * *Files identical despite different names*

### Comparing `scale-nucleus-0.9b5/nucleus/validate/scenario_test_evaluation.py` & `scale-nucleus-0.9b6/nucleus/validate/scenario_test_evaluation.py`

 * *Files identical despite different names*

### Comparing `scale-nucleus-0.9b5/nucleus/validate/scenario_test_metric.py` & `scale-nucleus-0.9b6/nucleus/validate/scenario_test_metric.py`

 * *Files identical despite different names*

### Comparing `scale-nucleus-0.9b5/pyproject.toml` & `scale-nucleus-0.9b6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     | dist
   )/
 )
 '''
 
 [tool.poetry]
 name = "scale-nucleus"
-version = "0.9b5"
+version = "0.9b6"
 description = "The official Python client library for Nucleus, the Data Platform for AI"
 license =  "MIT"
 authors = ["Scale AI Nucleus Team <nucleusapi@scaleapi.com>"]
 readme = "README.md"
 homepage = "https://scale.com/nucleus"
 repository = "https://github.com/scaleapi/nucleus-python-client"
 documentation = "https://dashboard.scale.com/nucleus/docs/api"
@@ -41,15 +41,15 @@
 pydantic = "^1.8.2"
 numpy = "^1.19.5"
 scipy = ">=1.4.1"  # NOTE: COLAB has 1.4.1 and has problems updating
 click = ">=7.1.2,<9.0"  # NOTE: COLAB has 7.1.2 and has problems updating
 rich = "^10.15.2"
 shellingham = "^1.4.0"
 scikit-learn = ">=0.24.0"
-Shapely = "^1.8.1"
+Shapely = { version = ">=1.8.0", optional = true }
 
 [tool.poetry.dev-dependencies]
 poetry = "^1.1.5"
 pytest = "^6.2.3"
 pylint = "^2.7.4"
 black = "^20.8b1"
 flake8 = "^3.9.1"
@@ -64,14 +64,18 @@
 furo = "^2021.10.9"
 sphinx-autoapi = "^1.8.4"
 pytest-xdist = "^2.5.0"
 
 [tool.poetry.scripts]
 nu = "cli.nu:nu"
 
+[tool.poetry.extras]
+shapely = ["Shapely"]
+
+
 [tool.pytest.ini_options]
 markers = [
     "integration: marks tests as slow (deselect with '-m \"not integration\"')",
 ]
 
 
 [build-system]
```

### Comparing `scale-nucleus-0.9b5/setup.py` & `scale-nucleus-0.9b6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,38 +11,38 @@
  'nucleus.validate.data_transfer_objects',
  'nucleus.validate.eval_functions']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['Shapely>=1.8.1,<2.0.0',
- 'aiohttp>=3.7.4,<4.0.0',
+['aiohttp>=3.7.4,<4.0.0',
  'click>=7.1.2,<9.0',
  'nest-asyncio>=1.5.1,<2.0.0',
  'numpy>=1.19.5,<2.0.0',
  'pydantic>=1.8.2,<2.0.0',
  'requests>=2.23.0,<3.0.0',
  'rich>=10.15.2,<11.0.0',
  'scikit-learn>=0.24.0',
  'scipy>=1.4.1',
  'shellingham>=1.4.0,<2.0.0',
  'tqdm>=4.41.0,<5.0.0']
 
 extras_require = \
-{':python_full_version >= "3.6.1" and python_version < "3.7"': ['dataclasses>=0.7,<0.8']}
+{':python_full_version >= "3.6.1" and python_version < "3.7"': ['dataclasses>=0.7,<0.8'],
+ 'shapely': ['Shapely>=1.8.0']}
 
 entry_points = \
 {'console_scripts': ['nu = cli.nu:nu']}
 
 setup_kwargs = {
     'name': 'scale-nucleus',
-    'version': '0.9b5',
+    'version': '0.9b6',
     'description': 'The official Python client library for Nucleus, the Data Platform for AI',
-    'long_description': '# Nucleus\n\nhttps://dashboard.scale.com/nucleus\n\nAggregate metrics in ML are not good enough. To improve production ML, you need to understand their qualitative failure modes, fix them by gathering more data, and curate diverse scenarios.\n\nScale Nucleus helps you:\n\n- Visualize your data\n- Curate interesting slices within your dataset\n- Review and manage annotations\n- Measure and debug your model performance\n\nNucleus is a new way—the right way—to develop ML models, helping us move away from the concept of one dataset and towards a paradigm of collections of scenarios.\n\n## Installation\n\n`$ pip install scale-nucleus`\n\n\n## CLI installation\nWe recommend installing the CLI via `pipx` (https://pypa.github.io/pipx/installation/). This makes sure that\nthe CLI does not interfere with you system packages and is accessible from your favorite terminal.\n\nFor MacOS:\n```bash\nbrew install pipx\npipx ensurepath\npipx install scale-nucleus\n# Optional installation of shell completion (for bash, zsh or fish)\nnu install-completions\n```\n\nOtherwise, install via pip (requires pip 19.0 or later):\n```bash\npython3 -m pip install --user pipx\npython3 -m pipx ensurepath\npython3 -m pipx install scale-nucleus\n# Optional installation of shell completion (for bash, zsh or fish)\nnu install-completions\n```\n\n## Common issues/FAQ\n\n### Outdated Client\n\nNucleus is iterating rapidly and as a result we do not always perfectly preserve backwards compatibility with older versions of the client. If you run into any unexpected error, it\'s a good idea to upgrade your version of the client by running\n```\npip install --upgrade scale-nucleus\n```\n\n## Usage\n\nFor the most up to date documentation, reference: https://dashboard.scale.com/nucleus/docs/api?language=python.\n\n## For Developers\n\nClone from github and install as editable\n\n```\ngit clone git@github.com:scaleapi/nucleus-python-client.git\ncd nucleus-python-client\npip3 install poetry\npoetry install\n```\n\nPlease install the pre-commit hooks by running the following command:\n\n```python\npoetry run pre-commit install\n```\n\nWhen releasing a new version please add release notes to the changelog in `CHANGELOG.md`.\n\n**Best practices for testing:**\n(1). Please run pytest from the root directory of the repo, i.e.\n\n```\npoetry run pytest tests/test_dataset.py\n```\n\n(2) To skip slow integration tests that have to wait for an async job to start.\n\n```\npoetry run pytest -m "not integration"\n```\n\n## Pydantic Models\n\nPrefer using [Pydantic](https://pydantic-docs.helpmanual.io/usage/models/) models rather than creating raw dictionaries \nor dataclasses to send or receive over the wire as JSONs. Pydantic is created with data validation in mind and provides very clear error \nmessages when it encounters a problem with the payload.\n\nThe Pydantic model(s) should mirror the payload to send. To represent a JSON payload that looks like this:\n```json\n{\n  "example_json_with_info": {\n      "metadata": {\n        "frame": 0\n      },\n      "reference_id": "frame0",\n      "url": "s3://example/scale_nucleus/2021/lidar/0038711321865000.json",\n      "type": "pointcloud"\n    },\n  "example_image_with_info": {\n      "metadata": {\n        "author": "Picasso"\n      },\n      "reference_id": "frame0",\n      "url": "s3://bucket/0038711321865000.jpg",\n      "type": "image"\n    },\n}\n```\n\nCould be represented as the following structure. Note that the field names map to the JSON keys and the usage of field \nvalidators (`@validator`).\n\n```python\nimport os.path\nfrom pydantic import BaseModel, validator\nfrom typing import Literal\n\n\nclass JsonWithInfo(BaseModel):\n    metadata: dict  # any dict is valid\n    reference_id: str\n    url: str\n    type: Literal["pointcloud", "recipe"]\n\n    @validator("url")\n    def has_json_extension(cls, v):\n        if not v.endswith(".json"):\n            raise ValueError(f"Expected \'.json\' extension got {v}")\n        return v\n\n\nclass ImageWithInfo(BaseModel):\n    metadata: dict  # any dict is valid\n    reference_id: str\n    url: str\n    type: Literal["image", "mask"]\n\n    @validator("url")\n    def has_valid_extension(cls, v):\n        valid_extensions = {".jpg", ".jpeg", ".png", ".tiff"}\n        _, extension = os.path.splitext(v)\n        if extension not in valid_extensions:\n            raise ValueError(f"Expected extension in {valid_extensions} got {v}")\n        return v\n\n\nclass ExampleNestedModel(BaseModel):\n    example_json_with_info: JsonWithInfo\n    example_image_with_info: ImageWithInfo\n\n# Usage:\nimport requests\npayload = requests.get("/example")\nparsed_model = ExampleNestedModel.parse_obj(payload.json())\nrequests.post("example/post_to", json=parsed_model.dict())\n```\n\n\n### Migrating to Pydantic\n- When migrating an interface from a dictionary use `nucleus.pydantic_base.DictCompatibleModel`. That allows you to get\nthe benefits of Pydantic but maintaints backwards compatibility with a Python dictionary by delegating `__getitem__` to \nfields.\n- When migrating a frozen dataclass use `nucleus.pydantic_base.ImmutableModel`. That is a base class set up to be \nimmutable after initialization.\n\n**Updating documentation:**\nWe use [Sphinx](https://www.sphinx-doc.org/en/master/) to autogenerate our API Reference from docstrings.\n\nTo test your local docstring changes, run the following commands from the repository\'s root directory:\n```\npoetry shell\ncd docs\nsphinx-autobuild . ./_build/html --watch ../nucleus\n```\n`sphinx-autobuild` will spin up a server on localhost (port 8000 by default) that will watch for and automatically rebuild a version of the API reference based on your local docstring changes.\n',
+    'long_description': '# Nucleus\n\nhttps://dashboard.scale.com/nucleus\n\nAggregate metrics in ML are not good enough. To improve production ML, you need to understand their qualitative failure modes, fix them by gathering more data, and curate diverse scenarios.\n\nScale Nucleus helps you:\n\n- Visualize your data\n- Curate interesting slices within your dataset\n- Review and manage annotations\n- Measure and debug your model performance\n\nNucleus is a new way—the right way—to develop ML models, helping us move away from the concept of one dataset and towards a paradigm of collections of scenarios.\n\n## Installation\n\n`$ pip install scale-nucleus`\n\n\n## CLI installation\nWe recommend installing the CLI via `pipx` (https://pypa.github.io/pipx/installation/). This makes sure that\nthe CLI does not interfere with you system packages and is accessible from your favorite terminal.\n\nFor MacOS:\n```bash\nbrew install pipx\npipx ensurepath\npipx install scale-nucleus\n# Optional installation of shell completion (for bash, zsh or fish)\nnu install-completions\n```\n\nOtherwise, install via pip (requires pip 19.0 or later):\n```bash\npython3 -m pip install --user pipx\npython3 -m pipx ensurepath\npython3 -m pipx install scale-nucleus\n# Optional installation of shell completion (for bash, zsh or fish)\nnu install-completions\n```\n\n## Common issues/FAQ\n\n### Outdated Client\n\nNucleus is iterating rapidly and as a result we do not always perfectly preserve backwards compatibility with older versions of the client. If you run into any unexpected error, it\'s a good idea to upgrade your version of the client by running\n```\npip install --upgrade scale-nucleus\n```\n\n## Usage\n\nFor the most up to date documentation, reference: https://dashboard.scale.com/nucleus/docs/api?language=python.\n\n## For Developers\n\nClone from github and install as editable\n\n```\ngit clone git@github.com:scaleapi/nucleus-python-client.git\ncd nucleus-python-client\npip3 install poetry\npoetry install\n```\n\nPlease install the pre-commit hooks by running the following command:\n\n```python\npoetry run pre-commit install\n```\n\nWhen releasing a new version please add release notes to the changelog in `CHANGELOG.md`.\n\n**Best practices for testing:**\n(1). Please run pytest from the root directory of the repo, i.e.\n\n```\npoetry run pytest tests/test_dataset.py\n```\n\n(2) To skip slow integration tests that have to wait for an async job to start.\n\n```\npoetry run pytest -m "not integration"\n```\n\n## Pydantic Models\n\nPrefer using [Pydantic](https://pydantic-docs.helpmanual.io/usage/models/) models rather than creating raw dictionaries \nor dataclasses to send or receive over the wire as JSONs. Pydantic is created with data validation in mind and provides very clear error \nmessages when it encounters a problem with the payload.\n\nThe Pydantic model(s) should mirror the payload to send. To represent a JSON payload that looks like this:\n```json\n{\n  "example_json_with_info": {\n      "metadata": {\n        "frame": 0\n      },\n      "reference_id": "frame0",\n      "url": "s3://example/scale_nucleus/2021/lidar/0038711321865000.json",\n      "type": "pointcloud"\n    },\n  "example_image_with_info": {\n      "metadata": {\n        "author": "Picasso"\n      },\n      "reference_id": "frame0",\n      "url": "s3://bucket/0038711321865000.jpg",\n      "type": "image"\n    },\n}\n```\n\nCould be represented as the following structure. Note that the field names map to the JSON keys and the usage of field \nvalidators (`@validator`).\n\n```python\nimport os.path\nfrom pydantic import BaseModel, validator\nfrom typing import Literal\n\n\nclass JsonWithInfo(BaseModel):\n    metadata: dict  # any dict is valid\n    reference_id: str\n    url: str\n    type: Literal["pointcloud", "recipe"]\n\n    @validator("url")\n    def has_json_extension(cls, v):\n        if not v.endswith(".json"):\n            raise ValueError(f"Expected \'.json\' extension got {v}")\n        return v\n\n\nclass ImageWithInfo(BaseModel):\n    metadata: dict  # any dict is valid\n    reference_id: str\n    url: str\n    type: Literal["image", "mask"]\n\n    @validator("url")\n    def has_valid_extension(cls, v):\n        valid_extensions = {".jpg", ".jpeg", ".png", ".tiff"}\n        _, extension = os.path.splitext(v)\n        if extension not in valid_extensions:\n            raise ValueError(f"Expected extension in {valid_extensions} got {v}")\n        return v\n\n\nclass ExampleNestedModel(BaseModel):\n    example_json_with_info: JsonWithInfo\n    example_image_with_info: ImageWithInfo\n\n# Usage:\nimport requests\npayload = requests.get("/example")\nparsed_model = ExampleNestedModel.parse_obj(payload.json())\nrequests.post("example/post_to", json=parsed_model.dict())\n```\n\n\n### Migrating to Pydantic\n- When migrating an interface from a dictionary use `nucleus.pydantic_base.DictCompatibleModel`. That allows you to get\nthe benefits of Pydantic but maintaints backwards compatibility with a Python dictionary by delegating `__getitem__` to \nfields.\n- When migrating a frozen dataclass use `nucleus.pydantic_base.ImmutableModel`. That is a base class set up to be \nimmutable after initialization.\n\n**Updating documentation:**\nWe use [Sphinx](https://www.sphinx-doc.org/en/master/) to autogenerate our API Reference from docstrings.\n\nTo test your local docstring changes, run the following commands from the repository\'s root directory:\n```\npoetry shell\ncd docs\nsphinx-autobuild . ./_build/html --watch ../nucleus\n```\n`sphinx-autobuild` will spin up a server on localhost (port 8000 by default) that will watch for and automatically rebuild a version of the API reference based on your local docstring changes.\n\n\n## Custom Metrics used in Scale Validate\n\nTo install the availalbe metrics for Scale Validate add the optional `metrics` extra.\nNote that you might need to install a local GEOS package.\n\n```bash\n#Mac OS\nbrew install geos\n# Ubuntu/Debian flavors\napt-get install libgeos-dev\n```\n\n`pip install scale-nucleus[metrics]`\n\nTo develop it locally use\n\n`poetry install --extra metrics`\n',
     'author': 'Scale AI Nucleus Team',
     'author_email': 'nucleusapi@scaleapi.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://scale.com/nucleus',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `scale-nucleus-0.9b5/PKG-INFO` & `scale-nucleus-0.9b6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: scale-nucleus
-Version: 0.9b5
+Version: 0.9b6
 Summary: The official Python client library for Nucleus, the Data Platform for AI
 Home-page: https://scale.com/nucleus
 License: MIT
 Author: Scale AI Nucleus Team
 Author-email: nucleusapi@scaleapi.com
 Requires-Python: >=3.6.2,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: Shapely (>=1.8.1,<2.0.0)
+Provides-Extra: shapely
+Requires-Dist: Shapely (>=1.8.0); extra == "shapely"
 Requires-Dist: aiohttp (>=3.7.4,<4.0.0)
 Requires-Dist: click (>=7.1.2,<9.0)
 Requires-Dist: dataclasses (>=0.7,<0.8); python_full_version >= "3.6.1" and python_version < "3.7"
 Requires-Dist: nest-asyncio (>=1.5.1,<2.0.0)
 Requires-Dist: numpy (>=1.19.5,<2.0.0)
 Requires-Dist: pydantic (>=1.8.2,<2.0.0)
 Requires-Dist: requests (>=2.23.0,<3.0.0)
@@ -208,7 +209,26 @@
 ```
 poetry shell
 cd docs
 sphinx-autobuild . ./_build/html --watch ../nucleus
 ```
 `sphinx-autobuild` will spin up a server on localhost (port 8000 by default) that will watch for and automatically rebuild a version of the API reference based on your local docstring changes.
 
+
+## Custom Metrics used in Scale Validate
+
+To install the availalbe metrics for Scale Validate add the optional `metrics` extra.
+Note that you might need to install a local GEOS package.
+
+```bash
+#Mac OS
+brew install geos
+# Ubuntu/Debian flavors
+apt-get install libgeos-dev
+```
+
+`pip install scale-nucleus[metrics]`
+
+To develop it locally use
+
+`poetry install --extra metrics`
+
```

