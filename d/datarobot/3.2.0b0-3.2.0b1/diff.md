# Comparing `tmp/datarobot-3.2.0b0.tar.gz` & `tmp/datarobot-3.2.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datarobot-3.2.0b0.tar", last modified: Mon Jun 12 17:35:34 2023, max compression
+gzip compressed data, was "datarobot-3.2.0b1.tar", last modified: Fri Jun 23 19:56:07 2023, max compression
```

## Comparing `datarobot-3.2.0b0.tar` & `datarobot-3.2.0b1.tar`

### file list

```diff
@@ -1,153 +1,155 @@
-drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-06-12 17:35:34.803885 datarobot-3.2.0b0/
--rw-r--r--   0 andrew.levan   (504) staff       (20)   173551 2023-06-12 17:23:01.000000 datarobot-3.2.0b0/CHANGES.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)     7555 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/LICENSE.txt
--rw-r--r--   0 andrew.levan   (504) staff       (20)      421 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/MANIFEST.in
--rw-r--r--   0 andrew.levan   (504) staff       (20)     3389 2023-06-12 17:35:34.804173 datarobot-3.2.0b0/PKG-INFO
--rw-r--r--   0 andrew.levan   (504) staff       (20)     8911 2023-05-24 20:04:06.000000 datarobot-3.2.0b0/README.md
--rw-r--r--   0 andrew.levan   (504) staff       (20)     5678 2023-05-15 20:05:42.000000 datarobot-3.2.0b0/common_setup.py
-drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-06-12 17:35:34.683410 datarobot-3.2.0b0/datarobot/
--rw-r--r--   0 andrew.levan   (504) staff       (20)     2257 2023-06-12 17:23:01.000000 datarobot-3.2.0b0/datarobot/__init__.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)      687 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/_compat.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)      313 2023-05-15 20:05:42.000000 datarobot-3.2.0b0/datarobot/_version.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    18879 2023-06-12 17:23:01.000000 datarobot-3.2.0b0/datarobot/client.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     3126 2023-06-12 17:23:01.000000 datarobot-3.2.0b0/datarobot/context.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    25285 2023-05-22 13:05:29.000000 datarobot-3.2.0b0/datarobot/enums.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     8680 2023-06-07 13:50:47.000000 datarobot-3.2.0b0/datarobot/errors.py
-drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-06-12 17:35:34.690327 datarobot-3.2.0b0/datarobot/helpers/
--rw-r--r--   0 andrew.levan   (504) staff       (20)    22432 2023-06-01 15:04:06.000000 datarobot-3.2.0b0/datarobot/helpers/__init__.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    13002 2023-03-13 20:20:37.000000 datarobot-3.2.0b0/datarobot/helpers/binary_data_utils.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     1156 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/helpers/eligibility_result.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    14350 2023-05-11 14:05:28.000000 datarobot-3.2.0b0/datarobot/helpers/feature_discovery.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     8696 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/helpers/image_utils.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)   101561 2023-05-22 13:04:57.000000 datarobot-3.2.0b0/datarobot/helpers/partitioning_methods.py
-drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-06-12 17:35:34.692712 datarobot-3.2.0b0/datarobot/mixins/
--rw-r--r--   0 andrew.levan   (504) staff       (20)        0 2023-06-01 15:04:06.000000 datarobot-3.2.0b0/datarobot/mixins/__init__.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     1134 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/mixins/browser_mixin.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     1112 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/mixins/update_attributes_mixin.py
-drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-06-12 17:35:34.760349 datarobot-3.2.0b0/datarobot/models/
--rw-r--r--   0 andrew.levan   (504) staff       (20)     4012 2023-06-01 15:10:47.000000 datarobot-3.2.0b0/datarobot/models/__init__.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     9166 2023-05-24 18:13:09.000000 datarobot-3.2.0b0/datarobot/models/advanced_tuning.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    27075 2023-05-15 20:05:42.000000 datarobot-3.2.0b0/datarobot/models/anomaly_assessment.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     2925 2023-05-15 20:05:42.000000 datarobot-3.2.0b0/datarobot/models/api_object.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     8859 2023-05-22 13:04:57.000000 datarobot-3.2.0b0/datarobot/models/application.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    15447 2023-05-15 20:05:42.000000 datarobot-3.2.0b0/datarobot/models/automated_documentation.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    23047 2023-05-23 15:25:49.000000 datarobot-3.2.0b0/datarobot/models/batch_monitoring_job.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    83098 2023-05-15 20:05:42.000000 datarobot-3.2.0b0/datarobot/models/batch_prediction_job.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    11096 2023-06-07 13:50:47.000000 datarobot-3.2.0b0/datarobot/models/blueprint.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    23822 2023-05-11 14:05:22.000000 datarobot-3.2.0b0/datarobot/models/calendar_file.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    13301 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/models/change_request.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     3978 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/models/cluster.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     7233 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/models/cluster_insight.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    12910 2023-05-15 20:05:42.000000 datarobot-3.2.0b0/datarobot/models/compliance_doc_template.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     4887 2023-05-15 20:05:42.000000 datarobot-3.2.0b0/datarobot/models/confusion_chart.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     6953 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/models/connector.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    11955 2023-06-12 17:23:01.000000 datarobot-3.2.0b0/datarobot/models/credential.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    32642 2023-06-07 13:50:47.000000 datarobot-3.2.0b0/datarobot/models/custom_model.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    11963 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/models/custom_model_test.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    59153 2023-06-07 13:50:47.000000 datarobot-3.2.0b0/datarobot/models/custom_model_version.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    15411 2023-05-22 13:05:29.000000 datarobot-3.2.0b0/datarobot/models/custom_task.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    21102 2023-05-15 20:05:42.000000 datarobot-3.2.0b0/datarobot/models/custom_task_version.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     2315 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/models/custom_task_version_dependency_build.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    17613 2023-03-13 20:20:37.000000 datarobot-3.2.0b0/datarobot/models/data_engine_query_generator.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    16402 2023-05-11 14:05:28.000000 datarobot-3.2.0b0/datarobot/models/data_source.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    13812 2023-05-11 14:05:28.000000 datarobot-3.2.0b0/datarobot/models/data_store.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    58123 2023-05-22 13:05:29.000000 datarobot-3.2.0b0/datarobot/models/dataset.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    30524 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/models/datetime_trend_plots.py
-drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-06-12 17:35:34.768900 datarobot-3.2.0b0/datarobot/models/deployment/
--rw-r--r--   0 andrew.levan   (504) staff       (20)      387 2023-06-01 15:04:09.000000 datarobot-3.2.0b0/datarobot/models/deployment/__init__.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    12535 2023-05-15 20:05:42.000000 datarobot-3.2.0b0/datarobot/models/deployment/accuracy.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     5688 2023-06-07 13:50:47.000000 datarobot-3.2.0b0/datarobot/models/deployment/bias_and_fairness.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    12650 2023-05-15 20:05:42.000000 datarobot-3.2.0b0/datarobot/models/deployment/data_drift.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    93319 2023-05-15 20:05:42.000000 datarobot-3.2.0b0/datarobot/models/deployment/deployment.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     1131 2023-05-15 20:05:42.000000 datarobot-3.2.0b0/datarobot/models/deployment/mixins.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    10065 2023-05-15 20:05:42.000000 datarobot-3.2.0b0/datarobot/models/deployment/service_stats.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     3450 2023-05-15 20:05:42.000000 datarobot-3.2.0b0/datarobot/models/deployment/sharing.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     6583 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/models/driver.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     9411 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/models/execution_environment.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    11344 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/models/execution_environment_version.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     5374 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/models/external_baseline_validation.py
-drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-06-12 17:35:34.776507 datarobot-3.2.0b0/datarobot/models/external_dataset_scores_insights/
--rw-r--r--   0 andrew.levan   (504) staff       (20)      355 2023-06-01 15:04:09.000000 datarobot-3.2.0b0/datarobot/models/external_dataset_scores_insights/__init__.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     6403 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     4915 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     4523 2023-05-11 14:05:28.000000 datarobot-3.2.0b0/datarobot/models/external_dataset_scores_insights/external_lift_chart.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     5208 2023-05-11 14:05:28.000000 datarobot-3.2.0b0/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     4521 2023-05-15 20:05:42.000000 datarobot-3.2.0b0/datarobot/models/external_dataset_scores_insights/external_roc_curve.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     6789 2023-05-11 14:05:28.000000 datarobot-3.2.0b0/datarobot/models/external_dataset_scores_insights/external_scores.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    53938 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/models/feature.py
-drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-06-12 17:35:34.780766 datarobot-3.2.0b0/datarobot/models/feature_association_matrix/
--rw-r--r--   0 andrew.levan   (504) staff       (20)      237 2023-06-01 15:04:09.000000 datarobot-3.2.0b0/datarobot/models/feature_association_matrix/__init__.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     2600 2023-05-11 14:05:28.000000 datarobot-3.2.0b0/datarobot/models/feature_association_matrix/feature_association_featurelists.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     6177 2023-05-11 14:05:28.000000 datarobot-3.2.0b0/datarobot/models/feature_association_matrix/feature_association_matrix.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     4753 2023-05-11 14:05:28.000000 datarobot-3.2.0b0/datarobot/models/feature_association_matrix/feature_association_matrix_details.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    16683 2023-05-15 20:05:42.000000 datarobot-3.2.0b0/datarobot/models/feature_effect.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    17463 2023-05-11 14:05:28.000000 datarobot-3.2.0b0/datarobot/models/featurelist.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     7336 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/models/imported_model.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    21038 2023-05-15 20:05:42.000000 datarobot-3.2.0b0/datarobot/models/job.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     2370 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/models/lift_chart.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     5468 2023-05-11 14:05:28.000000 datarobot-3.2.0b0/datarobot/models/missing_report.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)   256455 2023-06-07 13:50:47.000000 datarobot-3.2.0b0/datarobot/models/model.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     7215 2023-03-13 20:20:37.000000 datarobot-3.2.0b0/datarobot/models/modeljob.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    14320 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/models/pairwise_statistics.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     5438 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/models/pareto_front.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     8726 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/models/payoff_matrix.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     7403 2023-03-13 20:20:37.000000 datarobot-3.2.0b0/datarobot/models/predict_job.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    10218 2023-05-15 20:05:42.000000 datarobot-3.2.0b0/datarobot/models/prediction_dataset.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    34744 2023-05-15 20:05:42.000000 datarobot-3.2.0b0/datarobot/models/prediction_explanations.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     2426 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/models/prediction_server.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    15940 2023-05-11 14:05:28.000000 datarobot-3.2.0b0/datarobot/models/predictions.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     2655 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/models/prime_file.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)   215251 2023-05-31 16:21:11.000000 datarobot-3.2.0b0/datarobot/models/project.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    55519 2023-05-22 13:04:57.000000 datarobot-3.2.0b0/datarobot/models/project_options.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     8774 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/models/rating_table.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     4337 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/models/recommended_model.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    19064 2023-03-13 20:20:37.000000 datarobot-3.2.0b0/datarobot/models/relationships_configuration.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     2831 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/models/residuals.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     4524 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/models/restore_discarded_features.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     7730 2023-05-15 20:05:42.000000 datarobot-3.2.0b0/datarobot/models/roc_curve.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     2927 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/models/ruleset.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    19381 2023-05-11 14:05:28.000000 datarobot-3.2.0b0/datarobot/models/secondary_dataset.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    14217 2023-05-11 14:05:28.000000 datarobot-3.2.0b0/datarobot/models/segmentation.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     4070 2023-05-11 14:05:28.000000 datarobot-3.2.0b0/datarobot/models/shap_impact.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     7057 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/models/shap_matrix.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     2645 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/models/shap_matrix_job.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     6340 2023-05-22 13:05:29.000000 datarobot-3.2.0b0/datarobot/models/sharing.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     1431 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/models/trafarets.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    28260 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/models/training_predictions.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     1822 2023-05-15 20:05:42.000000 datarobot-3.2.0b0/datarobot/models/types.py
-drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-06-12 17:35:34.784473 datarobot-3.2.0b0/datarobot/models/use_cases/
--rw-r--r--   0 andrew.levan   (504) staff       (20)      262 2023-06-01 15:04:06.000000 datarobot-3.2.0b0/datarobot/models/use_cases/__init__.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    24565 2023-06-07 13:50:47.000000 datarobot-3.2.0b0/datarobot/models/use_cases/use_case.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     8680 2023-06-07 13:50:47.000000 datarobot-3.2.0b0/datarobot/models/use_cases/utils.py
-drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-06-12 17:35:34.789528 datarobot-3.2.0b0/datarobot/models/user_blueprints/
--rw-r--r--   0 andrew.levan   (504) staff       (20)       49 2023-06-01 15:04:09.000000 datarobot-3.2.0b0/datarobot/models/user_blueprints/__init__.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    69649 2023-05-15 20:05:42.000000 datarobot-3.2.0b0/datarobot/models/user_blueprints/models.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     8758 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/models/user_blueprints/trafarets.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     2668 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/models/validators.py
-drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-06-12 17:35:34.794571 datarobot-3.2.0b0/datarobot/models/visualai/
--rw-r--r--   0 andrew.levan   (504) staff       (20)      226 2023-06-01 15:04:09.000000 datarobot-3.2.0b0/datarobot/models/visualai/__init__.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    18528 2023-05-11 14:04:17.000000 datarobot-3.2.0b0/datarobot/models/visualai/augmentation.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    10521 2023-05-15 20:05:42.000000 datarobot-3.2.0b0/datarobot/models/visualai/images.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    13615 2023-05-15 20:05:42.000000 datarobot-3.2.0b0/datarobot/models/visualai/insights.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     4936 2023-05-11 14:05:28.000000 datarobot-3.2.0b0/datarobot/models/word_cloud.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)        0 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/py.typed
--rw-r--r--   0 andrew.levan   (504) staff       (20)    17330 2023-06-12 17:23:01.000000 datarobot-3.2.0b0/datarobot/rest.py
-drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-06-12 17:35:34.802841 datarobot-3.2.0b0/datarobot/utils/
--rw-r--r--   0 andrew.levan   (504) staff       (20)    15590 2023-06-01 15:11:07.000000 datarobot-3.2.0b0/datarobot/utils/__init__.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     2997 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/utils/deprecation.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)      495 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/utils/logger.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     1200 2023-04-18 15:18:29.000000 datarobot-3.2.0b0/datarobot/utils/pagination.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     1461 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/utils/retry.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     1282 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/utils/source.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     4109 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/utils/sourcedata.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     4061 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/utils/waiters.py
-drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-06-12 17:35:34.685978 datarobot-3.2.0b0/datarobot.egg-info/
--rw-r--r--   0 andrew.levan   (504) staff       (20)     3389 2023-06-12 17:35:34.000000 datarobot-3.2.0b0/datarobot.egg-info/PKG-INFO
--rw-r--r--   0 andrew.levan   (504) staff       (20)     5016 2023-06-12 17:35:34.000000 datarobot-3.2.0b0/datarobot.egg-info/SOURCES.txt
--rw-r--r--   0 andrew.levan   (504) staff       (20)        1 2023-06-12 17:35:34.000000 datarobot-3.2.0b0/datarobot.egg-info/dependency_links.txt
--rw-r--r--   0 andrew.levan   (504) staff       (20)     1080 2023-06-12 17:35:34.000000 datarobot-3.2.0b0/datarobot.egg-info/requires.txt
--rw-r--r--   0 andrew.levan   (504) staff       (20)       10 2023-06-12 17:35:34.000000 datarobot-3.2.0b0/datarobot.egg-info/top_level.txt
--rw-r--r--   0 andrew.levan   (504) staff       (20)     3066 2023-06-07 13:50:47.000000 datarobot-3.2.0b0/pyproject.toml
--rw-r--r--   0 andrew.levan   (504) staff       (20)      123 2023-06-12 17:35:34.805137 datarobot-3.2.0b0/setup.cfg
--rw-r--r--   0 andrew.levan   (504) staff       (20)      965 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/setup.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     1225 2023-06-12 17:34:54.000000 datarobot-3.2.0b0/setup_major.py
+drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-06-23 19:56:07.177518 datarobot-3.2.0b1/
+-rw-r--r--   0 andrew.levan   (504) staff       (20)   174746 2023-06-23 19:44:09.000000 datarobot-3.2.0b1/CHANGES.rst
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     7555 2023-03-10 16:03:09.000000 datarobot-3.2.0b1/LICENSE.txt
+-rw-r--r--   0 andrew.levan   (504) staff       (20)      421 2023-03-10 16:03:09.000000 datarobot-3.2.0b1/MANIFEST.in
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     3389 2023-06-23 19:56:07.177680 datarobot-3.2.0b1/PKG-INFO
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     8911 2023-05-24 20:04:06.000000 datarobot-3.2.0b1/README.md
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     5678 2023-06-23 19:39:37.000000 datarobot-3.2.0b1/common_setup.py
+drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-06-23 19:56:07.066842 datarobot-3.2.0b1/datarobot/
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     2257 2023-06-23 19:39:37.000000 datarobot-3.2.0b1/datarobot/__init__.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)      687 2023-03-10 16:03:09.000000 datarobot-3.2.0b1/datarobot/_compat.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)      313 2023-06-23 19:39:37.000000 datarobot-3.2.0b1/datarobot/_version.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    18879 2023-06-23 19:39:37.000000 datarobot-3.2.0b1/datarobot/client.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     3583 2023-06-23 19:44:09.000000 datarobot-3.2.0b1/datarobot/context.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    25769 2023-06-23 19:44:09.000000 datarobot-3.2.0b1/datarobot/enums.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     8984 2023-06-23 19:44:09.000000 datarobot-3.2.0b1/datarobot/errors.py
+drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-06-23 19:56:07.074044 datarobot-3.2.0b1/datarobot/helpers/
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    22432 2023-06-01 15:04:06.000000 datarobot-3.2.0b1/datarobot/helpers/__init__.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    13002 2023-03-13 20:20:37.000000 datarobot-3.2.0b1/datarobot/helpers/binary_data_utils.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     1156 2023-03-10 16:03:09.000000 datarobot-3.2.0b1/datarobot/helpers/eligibility_result.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    14350 2023-05-11 14:05:28.000000 datarobot-3.2.0b1/datarobot/helpers/feature_discovery.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     8696 2023-03-10 16:03:09.000000 datarobot-3.2.0b1/datarobot/helpers/image_utils.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)   101561 2023-05-22 13:04:57.000000 datarobot-3.2.0b1/datarobot/helpers/partitioning_methods.py
+drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-06-23 19:56:07.077009 datarobot-3.2.0b1/datarobot/mixins/
+-rw-r--r--   0 andrew.levan   (504) staff       (20)        0 2023-06-01 15:04:06.000000 datarobot-3.2.0b1/datarobot/mixins/__init__.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     1134 2023-03-10 16:03:09.000000 datarobot-3.2.0b1/datarobot/mixins/browser_mixin.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     1112 2023-03-10 16:03:09.000000 datarobot-3.2.0b1/datarobot/mixins/update_attributes_mixin.py
+drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-06-23 19:56:07.145380 datarobot-3.2.0b1/datarobot/models/
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     4087 2023-06-23 19:44:09.000000 datarobot-3.2.0b1/datarobot/models/__init__.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     9166 2023-05-24 18:13:09.000000 datarobot-3.2.0b1/datarobot/models/advanced_tuning.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    27075 2023-05-15 20:05:42.000000 datarobot-3.2.0b1/datarobot/models/anomaly_assessment.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     2925 2023-05-15 20:05:42.000000 datarobot-3.2.0b1/datarobot/models/api_object.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     8859 2023-05-22 13:04:57.000000 datarobot-3.2.0b1/datarobot/models/application.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    15447 2023-05-15 20:05:42.000000 datarobot-3.2.0b1/datarobot/models/automated_documentation.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    19691 2023-06-23 19:44:09.000000 datarobot-3.2.0b1/datarobot/models/batch_job.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    37053 2023-06-23 19:44:09.000000 datarobot-3.2.0b1/datarobot/models/batch_monitoring_job.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    66977 2023-06-23 19:44:09.000000 datarobot-3.2.0b1/datarobot/models/batch_prediction_job.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    11096 2023-06-07 13:50:47.000000 datarobot-3.2.0b1/datarobot/models/blueprint.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    23822 2023-05-11 14:05:22.000000 datarobot-3.2.0b1/datarobot/models/calendar_file.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    13301 2023-03-10 16:03:09.000000 datarobot-3.2.0b1/datarobot/models/change_request.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     3978 2023-03-10 16:03:09.000000 datarobot-3.2.0b1/datarobot/models/cluster.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     7233 2023-03-10 16:03:09.000000 datarobot-3.2.0b1/datarobot/models/cluster_insight.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    12910 2023-05-15 20:05:42.000000 datarobot-3.2.0b1/datarobot/models/compliance_doc_template.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     4887 2023-05-15 20:05:42.000000 datarobot-3.2.0b1/datarobot/models/confusion_chart.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     6953 2023-03-10 16:03:09.000000 datarobot-3.2.0b1/datarobot/models/connector.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    13004 2023-06-23 19:44:09.000000 datarobot-3.2.0b1/datarobot/models/credential.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    32642 2023-06-23 19:39:37.000000 datarobot-3.2.0b1/datarobot/models/custom_model.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    11963 2023-06-23 19:39:37.000000 datarobot-3.2.0b1/datarobot/models/custom_model_test.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    59153 2023-06-23 19:39:37.000000 datarobot-3.2.0b1/datarobot/models/custom_model_version.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    15411 2023-05-22 13:05:29.000000 datarobot-3.2.0b1/datarobot/models/custom_task.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    21102 2023-05-15 20:05:42.000000 datarobot-3.2.0b1/datarobot/models/custom_task_version.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     2315 2023-03-10 16:03:09.000000 datarobot-3.2.0b1/datarobot/models/custom_task_version_dependency_build.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    17613 2023-03-13 20:20:37.000000 datarobot-3.2.0b1/datarobot/models/data_engine_query_generator.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    16402 2023-05-11 14:05:28.000000 datarobot-3.2.0b1/datarobot/models/data_source.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    14952 2023-06-23 19:44:09.000000 datarobot-3.2.0b1/datarobot/models/data_store.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    58123 2023-06-23 19:39:37.000000 datarobot-3.2.0b1/datarobot/models/dataset.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    30524 2023-03-10 16:03:09.000000 datarobot-3.2.0b1/datarobot/models/datetime_trend_plots.py
+drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-06-23 19:56:07.152651 datarobot-3.2.0b1/datarobot/models/deployment/
+-rw-r--r--   0 andrew.levan   (504) staff       (20)      387 2023-06-01 15:04:09.000000 datarobot-3.2.0b1/datarobot/models/deployment/__init__.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    12535 2023-05-15 20:05:42.000000 datarobot-3.2.0b1/datarobot/models/deployment/accuracy.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     5688 2023-06-07 13:50:47.000000 datarobot-3.2.0b1/datarobot/models/deployment/bias_and_fairness.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    12650 2023-05-15 20:05:42.000000 datarobot-3.2.0b1/datarobot/models/deployment/data_drift.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    96313 2023-06-23 19:44:09.000000 datarobot-3.2.0b1/datarobot/models/deployment/deployment.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     1131 2023-05-15 20:05:42.000000 datarobot-3.2.0b1/datarobot/models/deployment/mixins.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    10065 2023-05-15 20:05:42.000000 datarobot-3.2.0b1/datarobot/models/deployment/service_stats.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     3450 2023-05-15 20:05:42.000000 datarobot-3.2.0b1/datarobot/models/deployment/sharing.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     6583 2023-03-10 16:03:09.000000 datarobot-3.2.0b1/datarobot/models/driver.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     9411 2023-03-10 16:03:09.000000 datarobot-3.2.0b1/datarobot/models/execution_environment.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    11344 2023-03-10 16:03:09.000000 datarobot-3.2.0b1/datarobot/models/execution_environment_version.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     5374 2023-03-10 16:03:09.000000 datarobot-3.2.0b1/datarobot/models/external_baseline_validation.py
+drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-06-23 19:56:07.158137 datarobot-3.2.0b1/datarobot/models/external_dataset_scores_insights/
+-rw-r--r--   0 andrew.levan   (504) staff       (20)      355 2023-06-01 15:04:09.000000 datarobot-3.2.0b1/datarobot/models/external_dataset_scores_insights/__init__.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     6403 2023-03-10 16:03:09.000000 datarobot-3.2.0b1/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     4915 2023-03-10 16:03:09.000000 datarobot-3.2.0b1/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     4523 2023-05-11 14:05:28.000000 datarobot-3.2.0b1/datarobot/models/external_dataset_scores_insights/external_lift_chart.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     5208 2023-05-11 14:05:28.000000 datarobot-3.2.0b1/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     4521 2023-05-15 20:05:42.000000 datarobot-3.2.0b1/datarobot/models/external_dataset_scores_insights/external_roc_curve.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     6789 2023-05-11 14:05:28.000000 datarobot-3.2.0b1/datarobot/models/external_dataset_scores_insights/external_scores.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    53938 2023-03-10 16:03:09.000000 datarobot-3.2.0b1/datarobot/models/feature.py
+drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-06-23 19:56:07.161378 datarobot-3.2.0b1/datarobot/models/feature_association_matrix/
+-rw-r--r--   0 andrew.levan   (504) staff       (20)      237 2023-06-01 15:04:09.000000 datarobot-3.2.0b1/datarobot/models/feature_association_matrix/__init__.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     2600 2023-05-11 14:05:28.000000 datarobot-3.2.0b1/datarobot/models/feature_association_matrix/feature_association_featurelists.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     6177 2023-05-11 14:05:28.000000 datarobot-3.2.0b1/datarobot/models/feature_association_matrix/feature_association_matrix.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     4753 2023-05-11 14:05:28.000000 datarobot-3.2.0b1/datarobot/models/feature_association_matrix/feature_association_matrix_details.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    16683 2023-06-23 19:39:37.000000 datarobot-3.2.0b1/datarobot/models/feature_effect.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    17463 2023-05-11 14:05:28.000000 datarobot-3.2.0b1/datarobot/models/featurelist.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     7336 2023-03-10 16:03:09.000000 datarobot-3.2.0b1/datarobot/models/imported_model.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    21038 2023-05-15 20:05:42.000000 datarobot-3.2.0b1/datarobot/models/job.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     2370 2023-06-23 19:39:37.000000 datarobot-3.2.0b1/datarobot/models/lift_chart.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     5468 2023-05-11 14:05:28.000000 datarobot-3.2.0b1/datarobot/models/missing_report.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)   256455 2023-06-23 19:39:37.000000 datarobot-3.2.0b1/datarobot/models/model.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     7215 2023-03-13 20:20:37.000000 datarobot-3.2.0b1/datarobot/models/modeljob.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    14320 2023-03-10 16:03:09.000000 datarobot-3.2.0b1/datarobot/models/pairwise_statistics.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     5438 2023-03-10 16:03:09.000000 datarobot-3.2.0b1/datarobot/models/pareto_front.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     8726 2023-03-10 16:03:09.000000 datarobot-3.2.0b1/datarobot/models/payoff_matrix.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     7403 2023-03-13 20:20:37.000000 datarobot-3.2.0b1/datarobot/models/predict_job.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    10218 2023-05-15 20:05:42.000000 datarobot-3.2.0b1/datarobot/models/prediction_dataset.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    34744 2023-05-15 20:05:42.000000 datarobot-3.2.0b1/datarobot/models/prediction_explanations.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     2426 2023-03-10 16:03:09.000000 datarobot-3.2.0b1/datarobot/models/prediction_server.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    15940 2023-05-11 14:05:28.000000 datarobot-3.2.0b1/datarobot/models/predictions.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     2655 2023-03-10 16:03:09.000000 datarobot-3.2.0b1/datarobot/models/prime_file.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)   215251 2023-06-14 14:49:27.000000 datarobot-3.2.0b1/datarobot/models/project.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    55519 2023-05-22 13:04:57.000000 datarobot-3.2.0b1/datarobot/models/project_options.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     8774 2023-03-10 16:03:09.000000 datarobot-3.2.0b1/datarobot/models/rating_table.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     4337 2023-03-10 16:03:09.000000 datarobot-3.2.0b1/datarobot/models/recommended_model.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    19064 2023-03-13 20:20:37.000000 datarobot-3.2.0b1/datarobot/models/relationships_configuration.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     2831 2023-06-23 19:39:37.000000 datarobot-3.2.0b1/datarobot/models/residuals.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     4524 2023-03-10 16:03:09.000000 datarobot-3.2.0b1/datarobot/models/restore_discarded_features.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     7730 2023-05-15 20:05:42.000000 datarobot-3.2.0b1/datarobot/models/roc_curve.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     2927 2023-03-10 16:03:09.000000 datarobot-3.2.0b1/datarobot/models/ruleset.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    19381 2023-05-11 14:05:28.000000 datarobot-3.2.0b1/datarobot/models/secondary_dataset.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    14217 2023-05-11 14:05:28.000000 datarobot-3.2.0b1/datarobot/models/segmentation.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     4070 2023-05-11 14:05:28.000000 datarobot-3.2.0b1/datarobot/models/shap_impact.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     7057 2023-03-10 16:03:09.000000 datarobot-3.2.0b1/datarobot/models/shap_matrix.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     2645 2023-03-10 16:03:09.000000 datarobot-3.2.0b1/datarobot/models/shap_matrix_job.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     6340 2023-06-23 19:39:37.000000 datarobot-3.2.0b1/datarobot/models/sharing.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     4554 2023-06-23 19:44:09.000000 datarobot-3.2.0b1/datarobot/models/status_check_job.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     1431 2023-03-10 16:03:09.000000 datarobot-3.2.0b1/datarobot/models/trafarets.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    28260 2023-03-10 16:03:09.000000 datarobot-3.2.0b1/datarobot/models/training_predictions.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     1822 2023-05-15 20:05:42.000000 datarobot-3.2.0b1/datarobot/models/types.py
+drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-06-23 19:56:07.163565 datarobot-3.2.0b1/datarobot/models/use_cases/
+-rw-r--r--   0 andrew.levan   (504) staff       (20)      262 2023-06-01 15:04:06.000000 datarobot-3.2.0b1/datarobot/models/use_cases/__init__.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    24375 2023-06-23 19:44:09.000000 datarobot-3.2.0b1/datarobot/models/use_cases/use_case.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    12298 2023-06-23 19:44:09.000000 datarobot-3.2.0b1/datarobot/models/use_cases/utils.py
+drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-06-23 19:56:07.166743 datarobot-3.2.0b1/datarobot/models/user_blueprints/
+-rw-r--r--   0 andrew.levan   (504) staff       (20)       49 2023-06-01 15:04:09.000000 datarobot-3.2.0b1/datarobot/models/user_blueprints/__init__.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    69649 2023-05-15 20:05:42.000000 datarobot-3.2.0b1/datarobot/models/user_blueprints/models.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     8758 2023-03-10 16:03:09.000000 datarobot-3.2.0b1/datarobot/models/user_blueprints/trafarets.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     2668 2023-03-10 16:03:09.000000 datarobot-3.2.0b1/datarobot/models/validators.py
+drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-06-23 19:56:07.170652 datarobot-3.2.0b1/datarobot/models/visualai/
+-rw-r--r--   0 andrew.levan   (504) staff       (20)      226 2023-06-01 15:04:09.000000 datarobot-3.2.0b1/datarobot/models/visualai/__init__.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    18528 2023-05-11 14:04:17.000000 datarobot-3.2.0b1/datarobot/models/visualai/augmentation.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    10521 2023-05-15 20:05:42.000000 datarobot-3.2.0b1/datarobot/models/visualai/images.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    13615 2023-05-15 20:05:42.000000 datarobot-3.2.0b1/datarobot/models/visualai/insights.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     4936 2023-05-11 14:05:28.000000 datarobot-3.2.0b1/datarobot/models/word_cloud.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)        0 2023-03-10 16:03:09.000000 datarobot-3.2.0b1/datarobot/py.typed
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    17330 2023-06-23 19:39:37.000000 datarobot-3.2.0b1/datarobot/rest.py
+drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-06-23 19:56:07.177019 datarobot-3.2.0b1/datarobot/utils/
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    15590 2023-06-01 15:11:07.000000 datarobot-3.2.0b1/datarobot/utils/__init__.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     2997 2023-03-10 16:03:09.000000 datarobot-3.2.0b1/datarobot/utils/deprecation.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)      495 2023-03-10 16:03:09.000000 datarobot-3.2.0b1/datarobot/utils/logger.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     1200 2023-04-18 15:18:29.000000 datarobot-3.2.0b1/datarobot/utils/pagination.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     1461 2023-03-10 16:03:09.000000 datarobot-3.2.0b1/datarobot/utils/retry.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     1282 2023-03-10 16:03:09.000000 datarobot-3.2.0b1/datarobot/utils/source.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     4109 2023-03-10 16:03:09.000000 datarobot-3.2.0b1/datarobot/utils/sourcedata.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     4061 2023-03-10 16:03:09.000000 datarobot-3.2.0b1/datarobot/utils/waiters.py
+drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-06-23 19:56:07.069114 datarobot-3.2.0b1/datarobot.egg-info/
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     3389 2023-06-23 19:56:06.000000 datarobot-3.2.0b1/datarobot.egg-info/PKG-INFO
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     5083 2023-06-23 19:56:06.000000 datarobot-3.2.0b1/datarobot.egg-info/SOURCES.txt
+-rw-r--r--   0 andrew.levan   (504) staff       (20)        1 2023-06-23 19:56:06.000000 datarobot-3.2.0b1/datarobot.egg-info/dependency_links.txt
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     1080 2023-06-23 19:56:06.000000 datarobot-3.2.0b1/datarobot.egg-info/requires.txt
+-rw-r--r--   0 andrew.levan   (504) staff       (20)       10 2023-06-23 19:56:06.000000 datarobot-3.2.0b1/datarobot.egg-info/top_level.txt
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     3066 2023-06-07 13:50:47.000000 datarobot-3.2.0b1/pyproject.toml
+-rw-r--r--   0 andrew.levan   (504) staff       (20)      123 2023-06-23 19:56:07.178250 datarobot-3.2.0b1/setup.cfg
+-rw-r--r--   0 andrew.levan   (504) staff       (20)      965 2023-03-10 16:03:09.000000 datarobot-3.2.0b1/setup.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     1215 2023-06-23 19:56:03.000000 datarobot-3.2.0b1/setup_major.py
```

### Comparing `datarobot-3.2.0b0/CHANGES.rst` & `datarobot-3.2.0b1/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,29 @@
 #########
 Changelog
 #########
+3.2.0b1
+========
+
+New Features
+************
+- Added :meth:`Credential.update <datarobot.models.Credential.update>` which allows you to update existing credential resources.
+- Added :meth:`Deployment.submit_actuals_from_catalog_async<datarobot.models.Deployment.submit_actuals_from_catalog_async>` to submit actuals from the AI Catalog.
+- Added a new class :class:`StatusCheckJob <datarobot.models.StatusCheckJob>` which represents a job for a status check of submitted async jobs.
+- Added a new class :class:`JobStatusResult <datarobot.models.JobStatusResult>` represents the result for a status check job of a submitted async task.
+- Added new methods to trigger batch monitoring jobs without providing a job definition.
+  :meth:`BatchMonitoringJob.run <datarobot.models.BatchMonitoringJob.run>`
+  :meth:`BatchMonitoringJob.get_status <datarobot.models.BatchMonitoringJob.get_status>`
+  :meth:`BatchMonitoringJob.cancel <datarobot.models.BatchMonitoringJob.cancel>`
+  :meth:`BatchMonitoringJob.download <datarobot.models.BatchMonitoringJob.download>`
+
+Bugfixes
+********
+- Fixed a bug that resulted in a duplicate item error when certain methods tried to add the same object to a UseCase twice
+
 3.2.0b0
 ========
 
 New Features
 ************
 - Added :meth:`DatetimePartitioning.datetime_partitioning_log_retrieve <datarobot.DatetimePartitioning.datetime_partitioning_log_retrieve>` to download the datetime partitioning log.
 - Added method :meth:`DatetimePartitioning.datetime_partitioning_log_list <datarobot.DatetimePartitioning.datetime_partitioning_log_list>` to list the datetime partitioning log.
```

### Comparing `datarobot-3.2.0b0/LICENSE.txt` & `datarobot-3.2.0b1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/PKG-INFO` & `datarobot-3.2.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datarobot
-Version: 3.2.0b0
+Version: 3.2.0b1
 Summary: This client library is designed to support the DataRobot API.
 Home-page: https://datarobot.com
 Author: datarobot
 Author-email: support@datarobot.com
 Maintainer: datarobot
 Maintainer-email: info@datarobot.com
 License: DataRobot Tool and Utility Agreement
```

### Comparing `datarobot-3.2.0b0/README.md` & `datarobot-3.2.0b1/README.md`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/common_setup.py` & `datarobot-3.2.0b1/common_setup.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/__init__.py` & `datarobot-3.2.0b1/datarobot/__init__.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/_compat.py` & `datarobot-3.2.0b1/datarobot/_compat.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/client.py` & `datarobot-3.2.0b1/datarobot/client.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/enums.py` & `datarobot-3.2.0b1/datarobot/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -931,7 +931,30 @@
     CAN_VIEW = "CAN_VIEW"
 
 
 class CredentialTypes(str, Enum):
     BASIC = "basic"
     OAUTH = "oauth"
     S3 = "s3"
+
+
+class IntakeAdapters(str, Enum, metaclass=StrEnum):
+    LOCAL_FILE = "localFile"
+    AZURE = "azure"
+    GCP = "gcp"
+    S3 = "s3"
+    JDBC = "jdbc"
+    DATASET = "dataset"
+    SNOWFLAKE = "snowflake"
+    SYNAPSE = "synapse"
+    BIG_QUERY = "bigquery"
+
+
+class OutputAdapters(str, Enum, metaclass=StrEnum):
+    LOCAL_FILE = "localFile"
+    AZURE = "azure"
+    GCP = "gcp"
+    S3 = "s3"
+    JDBC = "jdbc"
+    SNOWFLAKE = "snowflake"
+    SYNAPSE = "synapse"
+    BIG_QUERY = "bigquery"
```

### Comparing `datarobot-3.2.0b0/datarobot/errors.py` & `datarobot-3.2.0b1/datarobot/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -276,11 +276,20 @@
 
     See Also
     --------
     DataRobotDeprecationWarning
     """
 
 
+class MultipleUseCasesNotAllowed(UserWarning):
+    """
+    Raised when a method decorated with add_to_use_case(allow_multiple=True) calls a method
+    decorated with add_to_use_case(allow_multiple=False) with multiple UseCases passed
+    """
+
+    message = "Entity can't be added to multiple UseCases"
+
+
 warnings.filterwarnings("default", category=DataRobotDeprecationWarning)
 warnings.filterwarnings("always", category=PlatformDeprecationWarning)
 warnings.filterwarnings("always", category=InvalidRatingTableWarning)
 warnings.filterwarnings("always", category=ParentModelInsightFallbackWarning)
```

### Comparing `datarobot-3.2.0b0/datarobot/helpers/__init__.py` & `datarobot-3.2.0b1/datarobot/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/helpers/binary_data_utils.py` & `datarobot-3.2.0b1/datarobot/helpers/binary_data_utils.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/helpers/eligibility_result.py` & `datarobot-3.2.0b1/datarobot/helpers/eligibility_result.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/helpers/feature_discovery.py` & `datarobot-3.2.0b1/datarobot/helpers/feature_discovery.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/helpers/image_utils.py` & `datarobot-3.2.0b1/datarobot/helpers/image_utils.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/helpers/partitioning_methods.py` & `datarobot-3.2.0b1/datarobot/helpers/partitioning_methods.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/mixins/browser_mixin.py` & `datarobot-3.2.0b1/datarobot/mixins/browser_mixin.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/mixins/update_attributes_mixin.py` & `datarobot-3.2.0b1/datarobot/mixins/update_attributes_mixin.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/__init__.py` & `datarobot-3.2.0b1/datarobot/models/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -99,15 +99,16 @@
 from .relationships_configuration import RelationshipsConfiguration
 from .ruleset import Ruleset
 from .secondary_dataset import SecondaryDatasetConfigurations
 from .segmentation import SegmentationTask, SegmentInfo
 from .shap_impact import ShapImpact
 from .shap_matrix import ShapMatrix
 from .shap_matrix_job import ShapMatrixJob
-from .sharing import SharingAccess
+from .sharing import SharingAccess, SharingRole
+from .status_check_job import JobStatusResult, StatusCheckJob
 from .training_predictions import TrainingPredictions
 from .types import (
     AnomalyAssessmentDataPoint,
     AnomalyAssessmentPreviewBin,
     AnomalyAssessmentRecordMetadata,
     RegionExplanationsData,
     RocCurveEstimatedMetric,
```

### Comparing `datarobot-3.2.0b0/datarobot/models/advanced_tuning.py` & `datarobot-3.2.0b1/datarobot/models/advanced_tuning.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/anomaly_assessment.py` & `datarobot-3.2.0b1/datarobot/models/anomaly_assessment.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/api_object.py` & `datarobot-3.2.0b1/datarobot/models/api_object.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/application.py` & `datarobot-3.2.0b1/datarobot/models/application.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/automated_documentation.py` & `datarobot-3.2.0b1/datarobot/models/automated_documentation.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/batch_prediction_job.py` & `datarobot-3.2.0b1/datarobot/models/batch_prediction_job.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,123 +11,63 @@
 # Released under the terms of DataRobot Tool and Utility Agreement.
 # pylint: disable=too-many-lines
 from __future__ import annotations
 
 import csv
 import datetime
 import io
-import os
-import threading
-import time
-from typing import Any, cast, Dict, List, Optional, Tuple, TYPE_CHECKING, Union
+from typing import cast, Dict, List, Optional, Tuple, TYPE_CHECKING, Union
 
 import pandas as pd
-import requests
 import trafaret as t
 
 from datarobot import errors
 from datarobot._compat import Int, String
+from datarobot.models.batch_job import (
+    AbstractBatchJob,
+    CsvSettings,
+    IntakeSettings,
+    OutputSettings,
+    recognize_sourcedata,
+    Schedule,
+)
 from datarobot.models.credential import Credential
 from datarobot.models.dataset import Dataset
-from datarobot.models.job import AbstractSpecificJob
 from datarobot.models.prediction_explanations import PredictionExplanationsMode
 from datarobot.models.project import Project
-from datarobot.utils import get_id_from_response, pagination
-from datarobot.utils import recognize_sourcedata as orig_recognize_sourcedata
-from datarobot.utils import to_api
+from datarobot.utils import get_id_from_response, pagination, to_api
 
-from ..enums import AVAILABLE_STATEMENT_TYPES, DEFAULT_TIMEOUT, JOB_TYPE, QUEUE_STATUS
+from ..enums import DEFAULT_TIMEOUT, JOB_TYPE, QUEUE_STATUS
 from ..utils import logger, parse_time
 from .api_object import APIObject
 
 LOG = logger.get_logger(__name__)
 
 if TYPE_CHECKING:
     from mypy_extensions import TypedDict
 
     from datarobot.models.deployment import Deployment
 
     DeploymentType = Union[str, Deployment]
 
-    class IntakeSettings(TypedDict, total=False):
-        """Intake settings typed dict"""
-
-        type: str
-        file: Optional[Union[str, pd.DataFrame, io.IOBase]]
-        url: Optional[str]
-        credential_id: Optional[str]
-        data_store_id: Optional[str]
-        query: Optional[str]
-        table: Optional[str]
-        schema: Optional[str]
-        catalog: Optional[str]
-        fetch_size: Optional[int]
-        format: Optional[str]
-        endpoint_url: Optional[str]
-
-    class OutputSettings(TypedDict, total=False):
-        """Output settings typed dict"""
-
-        type: str
-        path: Optional[str]
-        url: Optional[str]
-        credential_id: Optional[str]
-        data_store_id: Optional[str]
-        table: Optional[str]
-        schema: Optional[str]
-        catalog: Optional[str]
-        statement_type: Optional[str]
-        update_columns: Optional[List[str]]
-        where_columns: Optional[List[str]]
-        create_table_if_not_exists: Optional[bool]
-
-    class CsvSettings(TypedDict):
-        delimiter: Optional[str]
-        quotechar: Optional[str]
-        encoding: Optional[str]
-
     class TimeSeriesSettings(TypedDict, total=False):
         type: str
         forecast_point: Optional[datetime.datetime]
         predictions_start_date: Optional[datetime.datetime]
         predictions_end_date: Optional[datetime.datetime]
         relax_known_in_advance_features_check: bool
 
     class PredictionInstance(TypedDict):
         hostName: str
         sslEnabled: Optional[bool]
         datarobotKey: Optional[str]
         apiKey: Optional[str]
 
-    class Schedule(TypedDict):
-        day_of_week: List[Union[int, str]]
-        month: List[Union[int, str]]
-        hour: List[Union[int, str]]
-        minute: List[Union[int, str]]
-        day_of_month: List[Union[int, str]]
-
-
-def recognize_sourcedata(sourcedata: Any, default_fname: str) -> Dict[str, Any]:
-    """Override the default recognize_sourcedata with one that converts
-    DataFrame to io.BytesIO"""
-    if not isinstance(sourcedata, pd.DataFrame):
-        return orig_recognize_sourcedata(sourcedata, default_fname)
-    # The original recognize_sourcedata will encode dataframes into StringIO
-    # To pass this to requests.put, we need BytesIO - otherwise, requests will
-    # try to encode it using latin-1 encoding (the default HTTP encoding),
-    # which will crash when a charater not contained in latin-1 is used
-    #
-    # https://github.com/python/cpython/blob/b9797417315cc2d1700cb2d427685016d3380711/Lib/http/client.py#L1046
-    buf = io.BytesIO()
-    sourcedata.to_csv(buf, encoding="utf-8", index=False, quoting=csv.QUOTE_ALL)
-    buf.seek(0)
-    return {"filelike": buf, "fname": default_fname}
-
 
-class BatchPredictionJob(AbstractSpecificJob):
+class BatchPredictionJob(AbstractBatchJob):
     """
     A Batch Prediction Job is used to score large data sets on
     prediction servers using the Batch Prediction API.
 
     Attributes
     ----------
     id : str
@@ -176,74 +116,14 @@
                 "FAILED",
             ),
             t.Key("project_id", optional=True): String,
             t.Key("is_blocked", optional=True): t.Bool,
         }
     )
 
-    _s3_settings = t.Dict(
-        {
-            t.Key("url"): String(),
-            t.Key("credential_id", optional=True): String(),
-            t.Key("endpoint_url", optional=True): String(),
-            t.Key("format", optional=True): String(),
-        }
-    )
-
-    _gcp_settings = t.Dict(
-        {
-            t.Key("url"): String(),
-            t.Key("credential_id", optional=True): String(),
-            t.Key("format", optional=True): String(),
-        }
-    )
-
-    _azure_settings = t.Dict(
-        {
-            t.Key("url"): String(),
-            t.Key("credential_id", optional=True): String(),
-            t.Key("format", optional=True): String(),
-        }
-    )
-
-    _dataset_intake_settings = t.Dict(
-        {t.Key("dataset"): t.Type(Dataset), t.Key("dataset_version_id", optional=True): String()}
-    )
-
-    _jdbc_intake_settings = t.Dict(
-        {
-            t.Key("data_store_id"): String(),
-            t.Key("query", optional=True): String(),
-            t.Key("table", optional=True): String(),
-            t.Key("schema", optional=True): String(),
-            t.Key("catalog", optional=True): String(),
-            t.Key("fetch_size", optional=True): Int(),
-            t.Key("credential_id", optional=True): String(),
-        }
-    )
-
-    _jdbc_output_settings = t.Dict(
-        {
-            t.Key("data_store_id"): String(),
-            t.Key("table"): String(),
-            t.Key("schema", optional=True): String(),
-            t.Key("catalog", optional=True): String(),
-            t.Key("statement_type"): t.Enum(
-                AVAILABLE_STATEMENT_TYPES.INSERT,
-                AVAILABLE_STATEMENT_TYPES.UPDATE,
-                AVAILABLE_STATEMENT_TYPES.INSERT_UPDATE,
-                AVAILABLE_STATEMENT_TYPES.CREATE_TABLE,
-            ),
-            t.Key("update_columns", optional=True): t.List(String),
-            t.Key("where_columns", optional=True): t.List(String),
-            t.Key("credential_id", optional=True): String(),
-            t.Key("create_table_if_not_exists", optional=True): t.Bool(),
-        }
-    )
-
     _timeseries_settings = t.Dict(
         {
             t.Key("type"): t.Atom("forecast"),
             t.Key("forecast_point", optional=True): parse_time,
             t.Key("relax_known_in_advance_features_check", optional=True): t.Bool(),
         }
     ) | t.Dict(
@@ -251,22 +131,14 @@
             t.Key("type"): t.Atom("historical"),
             t.Key("predictions_start_date", optional=True): parse_time,
             t.Key("predictions_end_date", optional=True): parse_time,
             t.Key("relax_known_in_advance_features_check", optional=True): t.Bool(),
         }
     )
 
-    _csv_settings = t.Dict(
-        {
-            t.Key("delimiter", optional=True): t.Atom("tab") | String(min_length=1, max_length=1),
-            t.Key("quotechar", optional=True): String(),
-            t.Key("encoding", optional=True): String(),
-        }
-    )
-
     _prediction_instance = t.Dict(
         {
             t.Key("hostName"): String(),
             t.Key("sslEnabled", optional=True): t.Bool(),
             t.Key("datarobotKey", optional=True): String(),
             t.Key("apiKey", optional=True): String(),
         }
@@ -282,17 +154,17 @@
     def _jobs_path(cls) -> str:
         return "batchPredictions/"
 
     @classmethod
     def _job_path(  # pylint: disable=arguments-renamed
         cls,
         project_id: str,
-        batch_prediction_job_id: str,
+        job_id: str,
     ) -> str:
-        return f"batchPredictions/{batch_prediction_job_id}/"
+        return f"batchPredictions/{job_id}/"
 
     @classmethod
     def _from_existing_path(cls) -> str:
         return "batchPredictions/fromExisting/"
 
     @classmethod
     def score(
@@ -677,298 +549,48 @@
                 if forecast_point and not isinstance(forecast_point, datetime.datetime):
                     raise ValueError(
                         "The value provided for forecast_point was not a valid format."
                     )
 
             job_data["timeseriesSettings"] = to_api(timeseries_settings)
 
-        if intake_settings is None:
-            intake_settings = {"type": "localFile"}
-        else:
-            # avoid mutating the input argument
-            intake_settings = dict(intake_settings)
-
+        # validate input settings, return a copy not original
+        intake_settings = cls.validate_intake_settings(intake_settings)
         intake_file = None
-
-        # Validate the intake settings
-
-        if intake_settings.get("type") not in (
-            "localFile",
-            "azure",
-            "gcp",
-            "s3",
-            "jdbc",
-            "dataset",
-            "snowflake",
-            "synapse",
-            "bigquery",
-        ):
-            raise ValueError(
-                "Unsupported type parameter for intake_settings: {}".format(
-                    intake_settings.get("type")
-                )
-            )
-
-        elif intake_settings["type"] == "localFile":
-
-            # This intake option requires us to upload the source
-            # data ourselves
-
-            if intake_settings.get("file") is None:
-                raise ValueError(
-                    "Missing source data. Either supply the `file` "
-                    "parameter or switch to an intake option that does not "
-                    "require it."
-                )
-
+        if intake_settings["type"] == "localFile":
             intake_file = recognize_sourcedata(intake_settings.pop("file"), "prediction.csv")
-
-        elif intake_settings["type"] == "s3":
-
-            del intake_settings["type"]
-            intake_settings = cls._s3_settings.check(intake_settings)
-            intake_settings["type"] = "s3"
-
-        elif intake_settings["type"] == "gcp":
-
-            del intake_settings["type"]
-            intake_settings = cls._gcp_settings.check(intake_settings)
-            intake_settings["type"] = "gcp"
-
-        elif intake_settings["type"] == "azure":
-
-            del intake_settings["type"]
-            intake_settings = cls._azure_settings.check(intake_settings)
-            intake_settings["type"] = "azure"
-
-        elif intake_settings["type"] == "jdbc":
-
-            del intake_settings["type"]
-            intake_settings = cls._jdbc_intake_settings.check(intake_settings)
-            intake_settings["type"] = "jdbc"
-
-        elif intake_settings["type"] == "dataset":
-
-            del intake_settings["type"]
-            intake_settings = cls._dataset_intake_settings.check(intake_settings)
-            intake_settings["type"] = "dataset"
-
-            dataset = intake_settings["dataset"]
-            intake_settings["dataset_id"] = dataset.id
-            if "dataset_version_id" not in intake_settings:
-                intake_settings["dataset_version_id"] = dataset.version_id
-
-            del intake_settings["dataset"]
-
         job_data["intakeSettings"] = to_api(intake_settings)
 
-        if output_settings is None:
-            output_settings = {"type": "localFile"}
-        else:
-            output_settings = dict(output_settings)
-
         output_file = None
 
         # Validate the output settings
 
-        if output_settings.get("type") not in (
-            "localFile",
-            "azure",
-            "gcp",
-            "s3",
-            "jdbc",
-            "snowflake",
-            "synapse",
-            "bigquery",
-        ):
-            raise ValueError(
-                "Unsupported type parameter for output_settings: {}".format(
-                    output_settings.get("type")
-                )
-            )
-
-        elif output_settings["type"] == "localFile":
-
+        output_settings = cls.validate_output_settings(output_settings)
+        if output_settings["type"] == "localFile":
             if output_settings.get("path") is not None:
                 output_file = open(  # pylint: disable=consider-using-with
                     output_settings.pop("path"), "wb"
                 )
-
-        elif output_settings["type"] == "s3":
-
-            del output_settings["type"]
-            output_settings = cls._s3_settings.check(output_settings)
-            output_settings["type"] = "s3"
-
-        elif output_settings["type"] == "gcp":
-
-            del output_settings["type"]
-            output_settings = cls._gcp_settings.check(output_settings)
-            output_settings["type"] = "gcp"
-
-        elif output_settings["type"] == "azure":
-
-            del output_settings["type"]
-            output_settings = cls._azure_settings.check(output_settings)
-            output_settings["type"] = "azure"
-
-        elif output_settings["type"] == "jdbc":
-
-            del output_settings["type"]
-            output_settings = cls._jdbc_output_settings.check(output_settings)
-            output_settings["type"] = "jdbc"
-
         job_data["outputSettings"] = to_api(output_settings)
 
         if csv_settings is not None:
             cls._csv_settings.check(csv_settings)
             job_data["csvSettings"] = to_api(csv_settings)
 
         response = cls._client.post(url=cls._jobs_path(), json=job_data)
 
         job_response = response.json()
         job_id = get_id_from_response(response)
 
         upload_thread = None
 
         if intake_file is not None:
-
-            # There is source data to upload, so spin up a thread to handle
-            # the upload concurrently and for thread safety issues, make
-            # a copy of the REST client object
-
-            _upload_client = cls._client.copy()
-            job_csv_settings = job_response.get("jobSpec", {}).get("csvSettings", {})
-
-            def _get_file_size(fileobj):
-                # To cover both files and filelike obj utilize .tell
-                cur = fileobj.tell()
-                fileobj.seek(0, os.SEEK_END)
-                file_size = fileobj.tell()
-                fileobj.seek(cur)
-
-                return file_size
-
-            # pylint: disable-next=unused-argument
-            def _create_csv_chunk(header, reader, max_size, delimiter, encoding, quotechar):
-                chunk = io.StringIO()
-                bytes_written = 0
-                writer = csv.writer(chunk, delimiter=delimiter, quotechar=quotechar)
-                writer.writerow(header)
-                while bytes_written < max_size:
-                    try:
-                        csv_chunk_content = next(reader)
-                        written = writer.writerow(csv_chunk_content)
-                        bytes_written += written
-                    except (StopIteration):
-                        break
-
-                return chunk, bytes_written
-
-            def _fileobj_to_csv_stream(fileobj, encoding):
-                stream = io.TextIOWrapper(fileobj, encoding=encoding)
-
-                yield from csv.reader(stream)
-
-                stream.close()
-
-            def _upload_multipart(fileobj, base_upload_url):
-                is_async = intake_settings.get("async", True)
-                MAX_RETRY = 1 if is_async else 3
-                MB_PER_CHUNK = 5
-                CHUNK_MAX_SIZE = MB_PER_CHUNK * 1024 * 1024
-
-                delimiter = job_csv_settings.get("delimiter", ",")
-                encoding = job_csv_settings.get("encoding", "utf-8")
-                quotechar = job_csv_settings.get("quotechar", '"')
-
-                file_size = _get_file_size(fileobj)
-                csv_stream = _fileobj_to_csv_stream(fileobj, encoding)
-
-                # grab the header so it can be added on all parts
-                header = next(csv_stream)
-
-                part_number = 0
-                bytes_written = 0
-                while bytes_written <= file_size:
-                    part_upload_url = f"{base_upload_url}part/{part_number}"
-
-                    # Read the inputfile in chunks of CHUNK_MAX_SIZE
-                    # Then call put multiple times increasing the part_number each time
-                    chunk, chunk_bytes = _create_csv_chunk(
-                        header, csv_stream, CHUNK_MAX_SIZE, delimiter, encoding, quotechar
-                    )
-                    bytes_written += chunk_bytes
-                    if chunk_bytes == 0:
-                        break
-
-                    for attempts in range(MAX_RETRY):
-                        try:
-                            chunk.seek(0)
-                            response = _upload_client.put(
-                                url=part_upload_url,
-                                data=chunk,
-                                headers={"content-type": "text/csv"},
-                                timeout=(_upload_client.connect_timeout, upload_read_timeout),
-                            )
-
-                            # Success! don't retry
-                            if response.status_code == 202:
-                                chunk.close()
-                                break
-                        except (requests.exceptions.ConnectionError, requests.exceptions.Timeout):
-                            attempts += 1
-                            if attempts == MAX_RETRY:
-                                raise
-
-                    part_number += 1
-
-                # finalize the upload to indicate no more data is arriving
-                _upload_client.post(url=f"{base_upload_url}finalizeMultipart")
-
-            def _uploader() -> None:
-                upload_url = job_response["links"]["csvUpload"]
-
-                if "file_path" in intake_file:
-                    fileobj = open(  # pylint: disable=consider-using-with
-                        intake_file["file_path"], "rb"
-                    )
-                else:
-                    fileobj = intake_file["filelike"]
-                    fileobj.seek(0)
-
-                try:
-                    if intake_settings.get("multipart"):
-                        _upload_multipart(fileobj, upload_url)
-
-                    else:
-                        _upload_client.put(
-                            url=upload_url,
-                            data=fileobj,
-                            headers={"content-type": "text/csv"},
-                            timeout=(_upload_client.connect_timeout, upload_read_timeout),
-                        )
-                finally:
-                    if hasattr(fileobj, "close"):
-                        fileobj.close()
-
-            if output_file is not None:
-
-                # If output_file is specified, we upload and download
-                # concurrently
-
-                upload_thread = threading.Thread(target=_uploader)
-                upload_thread.setDaemon(True)
-                upload_thread.start()
-
-            else:
-
-                # Otherwise, upload is synchronous
-
-                _uploader()
+            upload_thread = cls._upload_intake_file(
+                intake_file, intake_settings, job_response, upload_read_timeout, output_file
+            )
 
         job = BatchPredictionJob.get(job_id)
 
         if output_file is not None:
 
             # We must download the result to `output_file`
             # And clean up any thread we spawned during uploading
@@ -1606,99 +1228,32 @@
             Set to -1 to wait infinitely.
 
         read_timeout : int (optional, default 660)
             .. versionadded:: 2.22
 
             Seconds to wait for the server to respond between chunks.
         """
-        status = self._wait_for_download(timeout=timeout)
-        download_iter = self._client.get(
-            status["links"]["download"],
-            stream=True,
-            timeout=read_timeout,
-        ).iter_content(chunk_size=8192)
-
-        for chunk in download_iter:
-            if chunk:
-                fileobj.write(chunk)
-
-        # Check if job was aborted during download (and the download is incomplete)
-        status = self.get_status()
-        if status["status"] in ("ABORTED", "FAILED"):
-            raise RuntimeError("Job {} was aborted: {}".format(self.id, status["status_details"]))
-
-    def _wait_for_download(self, timeout: int = 120):
-        """Waits for download to become available"""
-        start = time.time()
-        status = None
-        while True:
-            status = self.get_status()
-
-            output_adapter_type = status["job_spec"].get("output_settings", {}).get("type")
-            if output_adapter_type and not output_adapter_type == "localFile":
-                raise RuntimeError(
-                    (
-                        "You cannot download predictions from jobs that did not use local_file as "
-                        "the output adapter. Job with ID {} had the output adapter defined as {}."
-                    ).format(self.id, output_adapter_type)
-                )
-
-            if status["status"] in ("ABORTED", "FAILED"):
-                raise RuntimeError(
-                    "Job {} was aborted: {}".format(self.id, status["status_details"])
-                )
-
-            if "download" in status["links"]:
-                break
-
-            if timeout >= 0 and time.time() - start > timeout:  # pylint: disable=chained-comparison
-                break
-
-            time.sleep(1)
-
-        if "download" not in status["links"]:
-            # Ignore 404 errors here if the job never started - then we can't abort it
-            self.delete(ignore_404_errors=True)
-            raise RuntimeError(
-                (
-                    "Timed out waiting for download to become available for job ID {}. "
-                    "Other jobs may be occupying the queue. Consider raising the timeout."
-                ).format(self.id)
-            )
-
-        return status
+        self._download(fileobj, timeout, read_timeout)
 
     def delete(self, ignore_404_errors: bool = False) -> None:
         """
         Cancel this job. If this job has not finished running, it will be
         removed and canceled.
         """
-        status = self.get_status()
-
-        prediction_job_id = status["links"]["self"].split("/")[-2]
-        try:
-            self._client.delete(self._job_path(None, prediction_job_id))
-        except errors.ClientError as exc:
-            if exc.status_code == 404 and ignore_404_errors:
-                return
-            raise
+        self._delete(ignore_404_errors)
 
     def get_status(self):
         """Get status of batch prediction job
 
         Returns
         -------
         BatchPredictionJob status data
             Dict with job status
         """
-
-        batch_job = super().get(None, self.id)
-        batch_job.id = self.id
-
-        return batch_job._safe_data
+        return self._get_status()
 
     @classmethod
     def list_by_status(cls, statuses: Optional[List[str]] = None) -> List[BatchPredictionJob]:
         """Get jobs collection for specific set of statuses
 
         Attributes
         ----------
```

### Comparing `datarobot-3.2.0b0/datarobot/models/blueprint.py` & `datarobot-3.2.0b1/datarobot/models/blueprint.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/calendar_file.py` & `datarobot-3.2.0b1/datarobot/models/calendar_file.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/change_request.py` & `datarobot-3.2.0b1/datarobot/models/change_request.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/cluster.py` & `datarobot-3.2.0b1/datarobot/models/cluster.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/cluster_insight.py` & `datarobot-3.2.0b1/datarobot/models/cluster_insight.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/compliance_doc_template.py` & `datarobot-3.2.0b1/datarobot/models/compliance_doc_template.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/confusion_chart.py` & `datarobot-3.2.0b1/datarobot/models/confusion_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/connector.py` & `datarobot-3.2.0b1/datarobot/models/connector.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/credential.py` & `datarobot-3.2.0b1/datarobot/models/credential.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # affiliates.
 #
 # Released under the terms of DataRobot Tool and Utility Agreement.
 from __future__ import annotations
 
 from datetime import datetime
 import json
-from typing import Dict, List, Optional, Union
+from typing import Any, Dict, List, Optional, Union
 
 import trafaret as t
 from trafaret.contrib.rfc_3339 import DateTime
 
 from datarobot._compat import String
 from datarobot.models.api_object import APIObject
 from datarobot.utils import pagination, rawdict
@@ -377,14 +377,42 @@
             "name": name,
             "credentialType": "gcp",
             "gcpKey": rawdict(gcp_key),  # type: ignore[arg-type]
             "description": description,
         }
         return cls.from_server_data(cls._client.post(cls._path, data=payload).json())
 
+    def update(
+        self, name: Optional[str] = None, description: Optional[str] = None, **kwargs: Any
+    ) -> None:
+        """Update the credential values of an existing credential. Updates this object in place.
+
+        .. versionadded:: v3.2
+
+        Parameters
+        ----------
+        name : str
+            The name to use for this set of credentials.
+        description : str, optional
+            The description to use for this set of credentials; if omitted, and name is not
+            omitted, then it clears any previous description for that name.
+        kwargs : Keyword arguments specific to the given credential_type that should be updated.
+        """
+        if name is not None:
+            kwargs["name"] = name
+        if description is not None:
+            kwargs["description"] = description
+
+        self._client.patch(f"{self._path}{self.credential_id}/", data=kwargs)
+
+        if name is not None:
+            self.name = name
+        if description is not None:
+            self.description = description
+
 
 BasicCredentialsSchema = t.Dict(
     {
         t.Key("credentialType"): t.Atom("basic"),
         t.Key("user"): String(),
         t.Key("password"): String(),
     }
```

### Comparing `datarobot-3.2.0b0/datarobot/models/custom_model.py` & `datarobot-3.2.0b1/datarobot/models/custom_model.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/custom_model_test.py` & `datarobot-3.2.0b1/datarobot/models/custom_model_test.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/custom_model_version.py` & `datarobot-3.2.0b1/datarobot/models/custom_model_version.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/custom_task.py` & `datarobot-3.2.0b1/datarobot/models/custom_task.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/custom_task_version.py` & `datarobot-3.2.0b1/datarobot/models/custom_task_version.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/custom_task_version_dependency_build.py` & `datarobot-3.2.0b1/datarobot/models/custom_task_version_dependency_build.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/data_engine_query_generator.py` & `datarobot-3.2.0b1/datarobot/models/data_engine_query_generator.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/data_source.py` & `datarobot-3.2.0b1/datarobot/models/data_source.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/data_store.py` & `datarobot-3.2.0b1/datarobot/models/data_store.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,16 +15,17 @@
 from typing import Dict, List, Optional, TYPE_CHECKING
 
 import trafaret as t
 
 from datarobot._compat import String
 from datarobot.enums import DATA_STORE_TABLE_TYPE
 from datarobot.models.api_object import APIObject, ServerDataType
+from datarobot.models.credential import CredentialDataSchema
 from datarobot.models.sharing import SharingAccess
-from datarobot.utils import from_api, parse_time
+from datarobot.utils import from_api, parse_time, to_api
 from datarobot.utils.pagination import unpaginate
 
 _data_store_params_converter = t.Dict(
     {t.Key("driver_id"): String(), t.Key("jdbc_url", optional=True): t.Or(String(), t.Null())}
 ).ignore_extra("*")
 
 if TYPE_CHECKING:
@@ -245,25 +246,43 @@
         self.canonical_name = r_data["canonicalName"]
         self.params = DataStoreParameters(r_data["params"]["driverId"], r_data["params"]["jdbcUrl"])
 
     def delete(self) -> None:
         """Removes the DataStore"""
         self._client.delete(f"{self._path}{self.id}/")
 
-    def test(self, username: str, password: str) -> TestResponse:
+    def test(
+        self,
+        username: Optional[str] = None,
+        password: Optional[str] = None,
+        credential_id: Optional[str] = None,
+        use_kerberos: Optional[bool] = None,
+        credential_data: Optional[Dict[str, str]] = None,
+    ) -> TestResponse:
         """
         Tests database connection.
 
+        .. versionchanged:: v3.2
+           Added `credential_id`, `use_kerberos` and `credential_data` optional params and made
+           `username` and `password` optional.
+
         Parameters
         ----------
         username : str
-            the username for database authentication.
+            optional, the username for database authentication.
         password : str
-            the password for database authentication. The password is encrypted
+            optional, the password for database authentication. The password is encrypted
             at server side and never saved / stored
+        credential_id : str
+            optional, id of the set of credentials to use instead of username and password
+        use_kerberos : bool
+            optional, whether to use Kerberos for data store authentication
+        credential_data : dict
+            optional, the credentials to authenticate with the database, to use instead of
+            user/password or credential ID
 
         Returns
         -------
         message : dict
             message with status.
 
         Examples
@@ -271,16 +290,23 @@
         .. code-block:: python
 
             >>> import datarobot as dr
             >>> data_store = dr.DataStore.get('5ad5d2afef5cd700014d3cae')
             >>> data_store.test(username='db_username', password='db_password')
             {'message': 'Connection successful'}
         """
-        payload = {"user": username, "password": password}
-        return self._client.post(f"{self._path}{self.id}/test/", data=payload).json()  # type: ignore[no-any-return]
+        payload = {
+            "user": username,
+            "password": password,
+            "credential_id": credential_id,
+            "use_kerberos": use_kerberos,
+        }
+        if credential_data:
+            payload["credential_data"] = CredentialDataSchema(credential_data)
+        return self._client.post(f"{self._path}{self.id}/test/", data=to_api(payload)).json()  # type: ignore[no-any-return] # noqa: E501 # pylint: disable=C0301
 
     def schemas(self, username: str, password: str) -> SchemasResponse:
         """
         Returns list of available schemas.
 
         Parameters
         ----------
```

### Comparing `datarobot-3.2.0b0/datarobot/models/dataset.py` & `datarobot-3.2.0b1/datarobot/models/dataset.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/datetime_trend_plots.py` & `datarobot-3.2.0b1/datarobot/models/datetime_trend_plots.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/deployment/accuracy.py` & `datarobot-3.2.0b1/datarobot/models/deployment/accuracy.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/deployment/bias_and_fairness.py` & `datarobot-3.2.0b1/datarobot/models/deployment/bias_and_fairness.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/deployment/data_drift.py` & `datarobot-3.2.0b1/datarobot/models/deployment/data_drift.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/deployment/deployment.py` & `datarobot-3.2.0b1/datarobot/models/deployment/deployment.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 from datarobot.models.deployment.mixins import MonitoringDataQueryBuilderMixin
 from datarobot.models.deployment.service_stats import ServiceStats, ServiceStatsOverTime
 from datarobot.models.deployment.sharing import (
     DeploymentGrantSharedRoleWithId,
     DeploymentGrantSharedRoleWithUsername,
     DeploymentSharedRole,
 )
+from datarobot.models.status_check_job import StatusCheckJob
 from datarobot.utils import deprecated, from_api, get_id_from_location
 from datarobot.utils.pagination import unpaginate
 from datarobot.utils.source import parse_source_type
 from datarobot.utils.waiters import wait_for_async_resolution
 
 if TYPE_CHECKING:
     from mypy_extensions import TypedDict
@@ -994,14 +995,91 @@
                         timestamp = timestamp.isoformat()
                     actual["timestamp"] = timestamp
 
                 payload.append(actual)
             response = self._client.post(url, data={"data": payload})
             wait_for_async_resolution(self._client, response.headers["Location"])
 
+    def submit_actuals_from_catalog_async(
+        self,
+        dataset_id: str,
+        actual_value_column: str,
+        association_id_column: str,
+        dataset_version_id: Optional[str] = None,
+        timestamp_column: Optional[str] = None,
+        was_acted_on_column: Optional[str] = None,
+    ) -> StatusCheckJob:
+        """Submit actuals from AI Catalog for processing.
+        The actuals submitted will be used to calculate accuracy metrics.
+
+        Parameters
+        ----------
+        dataset_id: str,
+            The ID of the source dataset.
+        dataset_version_id: str, optional
+            The ID of the dataset version to apply the query to. If not specified, the
+            latest version associated with dataset_id is used.
+        association_id_column: str,
+            The name of the column that contains a unique identifier used with a prediction.
+        actual_value_column: str,
+            The name of the column that contains the actual value of a prediction.
+        was_acted_on_column: str, optional,
+            The name of the column that indicates if the prediction was acted on in a way that
+            could have affected the actual outcome.
+        timestamp_column: str, optional,
+            The name of the column that contains datetime or string in RFC3339 format.
+
+        Returns
+        -------
+        status_check_job : StatusCheckJob
+            Object contains all needed logic for a periodical status check of an async job.
+
+        Raises
+        ------
+        ValueError
+            if dataset_id not provided
+            if actual_value_column not provided
+            if association_id_column not provided
+
+        Examples
+        --------
+        .. code-block:: python
+
+            from datarobot import Deployment
+            deployment = Deployment.get(deployment_id='5c939e08962d741e34f609f0')
+            status_check_job = deployment.submit_actuals_from_catalog_async(data)
+        """
+        if not dataset_id:
+            raise ValueError("Catalog Dataset ID is required to submit actuals.")
+
+        if not actual_value_column:
+            raise ValueError("Actual value column is required to submit actuals.")
+
+        if not association_id_column:
+            raise ValueError("Association id column is required to submit actuals.")
+
+        actuals_config = {
+            "actualValueColumn": actual_value_column,
+            "associationIdColumn": association_id_column,
+            "datasetId": dataset_id,
+            "datasetVersionId": dataset_version_id,
+        }
+
+        if timestamp_column:
+            actuals_config["timestampColumn"] = timestamp_column
+
+        if was_acted_on_column:
+            actuals_config["wasActedOnColumn"] = was_acted_on_column
+
+        url = f"{self._path}{self.id}/actuals/fromDataset/"
+
+        response = self._client.post(url, data=actuals_config)
+
+        return StatusCheckJob.from_response(response)
+
     def get_predictions_by_forecast_date_settings(self) -> ForecastDateSettings:
         """Retrieve predictions by forecast date settings of this deployment.
 
         .. versionadded:: v2.27
 
         Returns
         -------
```

### Comparing `datarobot-3.2.0b0/datarobot/models/deployment/mixins.py` & `datarobot-3.2.0b1/datarobot/models/deployment/mixins.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/deployment/service_stats.py` & `datarobot-3.2.0b1/datarobot/models/deployment/service_stats.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/deployment/sharing.py` & `datarobot-3.2.0b1/datarobot/models/deployment/sharing.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/driver.py` & `datarobot-3.2.0b1/datarobot/models/driver.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/execution_environment.py` & `datarobot-3.2.0b1/datarobot/models/execution_environment.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/execution_environment_version.py` & `datarobot-3.2.0b1/datarobot/models/execution_environment_version.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/external_baseline_validation.py` & `datarobot-3.2.0b1/datarobot/models/external_baseline_validation.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py` & `datarobot-3.2.0b1/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py` & `datarobot-3.2.0b1/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/external_dataset_scores_insights/external_lift_chart.py` & `datarobot-3.2.0b1/datarobot/models/external_dataset_scores_insights/external_lift_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py` & `datarobot-3.2.0b1/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/external_dataset_scores_insights/external_roc_curve.py` & `datarobot-3.2.0b1/datarobot/models/external_dataset_scores_insights/external_roc_curve.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/external_dataset_scores_insights/external_scores.py` & `datarobot-3.2.0b1/datarobot/models/external_dataset_scores_insights/external_scores.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/feature.py` & `datarobot-3.2.0b1/datarobot/models/feature.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/feature_association_matrix/feature_association_featurelists.py` & `datarobot-3.2.0b1/datarobot/models/feature_association_matrix/feature_association_featurelists.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/feature_association_matrix/feature_association_matrix.py` & `datarobot-3.2.0b1/datarobot/models/feature_association_matrix/feature_association_matrix.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/feature_association_matrix/feature_association_matrix_details.py` & `datarobot-3.2.0b1/datarobot/models/feature_association_matrix/feature_association_matrix_details.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/feature_effect.py` & `datarobot-3.2.0b1/datarobot/models/feature_effect.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/featurelist.py` & `datarobot-3.2.0b1/datarobot/models/featurelist.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/imported_model.py` & `datarobot-3.2.0b1/datarobot/models/imported_model.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/job.py` & `datarobot-3.2.0b1/datarobot/models/job.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/lift_chart.py` & `datarobot-3.2.0b1/datarobot/models/lift_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/missing_report.py` & `datarobot-3.2.0b1/datarobot/models/missing_report.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/model.py` & `datarobot-3.2.0b1/datarobot/models/model.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/modeljob.py` & `datarobot-3.2.0b1/datarobot/models/modeljob.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/pairwise_statistics.py` & `datarobot-3.2.0b1/datarobot/models/pairwise_statistics.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/pareto_front.py` & `datarobot-3.2.0b1/datarobot/models/pareto_front.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/payoff_matrix.py` & `datarobot-3.2.0b1/datarobot/models/payoff_matrix.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/predict_job.py` & `datarobot-3.2.0b1/datarobot/models/predict_job.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/prediction_dataset.py` & `datarobot-3.2.0b1/datarobot/models/prediction_dataset.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/prediction_explanations.py` & `datarobot-3.2.0b1/datarobot/models/prediction_explanations.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/prediction_server.py` & `datarobot-3.2.0b1/datarobot/models/prediction_server.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/predictions.py` & `datarobot-3.2.0b1/datarobot/models/predictions.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/prime_file.py` & `datarobot-3.2.0b1/datarobot/models/prime_file.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/project.py` & `datarobot-3.2.0b1/datarobot/models/project.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/project_options.py` & `datarobot-3.2.0b1/datarobot/models/project_options.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/rating_table.py` & `datarobot-3.2.0b1/datarobot/models/rating_table.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/recommended_model.py` & `datarobot-3.2.0b1/datarobot/models/recommended_model.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/relationships_configuration.py` & `datarobot-3.2.0b1/datarobot/models/relationships_configuration.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/residuals.py` & `datarobot-3.2.0b1/datarobot/models/residuals.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/restore_discarded_features.py` & `datarobot-3.2.0b1/datarobot/models/restore_discarded_features.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/roc_curve.py` & `datarobot-3.2.0b1/datarobot/models/roc_curve.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/ruleset.py` & `datarobot-3.2.0b1/datarobot/models/ruleset.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/secondary_dataset.py` & `datarobot-3.2.0b1/datarobot/models/secondary_dataset.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/segmentation.py` & `datarobot-3.2.0b1/datarobot/models/segmentation.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/shap_impact.py` & `datarobot-3.2.0b1/datarobot/models/shap_impact.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/shap_matrix.py` & `datarobot-3.2.0b1/datarobot/models/shap_matrix.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/shap_matrix_job.py` & `datarobot-3.2.0b1/datarobot/models/shap_matrix_job.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/sharing.py` & `datarobot-3.2.0b1/datarobot/models/sharing.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/trafarets.py` & `datarobot-3.2.0b1/datarobot/models/trafarets.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/training_predictions.py` & `datarobot-3.2.0b1/datarobot/models/training_predictions.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/types.py` & `datarobot-3.2.0b1/datarobot/models/types.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/use_cases/use_case.py` & `datarobot-3.2.0b1/datarobot/models/use_cases/use_case.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,14 +118,60 @@
         self.entity_id = entity_id
         self.use_case_id = use_case_id
         self.created_at = created_at
         self.created = UseCaseUser(**created)
         self.is_deleted = is_deleted
 
 
+def get_reference_entity_info(
+    entity: Union[UseCaseReferenceEntity, T]
+) -> Tuple[UseCaseAPIPathEntityType, Optional[str]]:
+    """
+    Get the entity type and entity id for a reference entity instance
+    Parameters
+    ----------
+    entity : Union[UseCaseReferenceEntity, Project, Dataset, Application]
+        The entity instance to add to a Use Case.
+    Returns
+    -------
+    entity_info : Tuple[UseCaseEntityType, str]
+        The entity type and entity id
+    """
+    from ..application import Application
+    from ..dataset import Dataset
+    from ..prediction_dataset import PredictionDataset
+    from ..project import Project
+
+    if isinstance(entity, Project):
+        return UseCaseAPIPathEntityType.PROJECT, entity.id
+    elif isinstance(entity, Dataset):
+        return UseCaseAPIPathEntityType.DATASET, entity.id
+    elif isinstance(entity, Application):
+        return UseCaseAPIPathEntityType.APPLICATION, entity.id
+    elif isinstance(entity, UseCaseReferenceEntity):
+        entity_type = UseCaseReferenceEntityMap.get(entity.entity_type)
+        if entity_type:
+            return entity_type, entity.entity_id
+    error_message = (
+        f"Entity must be Project, Dataset, Application, "
+        f"or UseCaseReferenceEntity. Invalid type: {type(entity).__name__}."
+    )
+    if isinstance(entity, UseCaseReferenceEntity):
+        # If we're failing here, it's because the UseCaseReferenceEntity is a notebook or other unsupported type
+        error_message = error_message + f" Unsupported Entity Type: {entity.entity_type}."
+    if isinstance(entity, PredictionDataset):
+        # Adding a specific error for PredictionDataset since the name would indicate it could
+        # be treated as a Dataset, when in fact it's a separate entity and not a subclass.
+        error_message = (
+            error_message + " PredictionDataset is not a subclass of Dataset and "
+            "cannot be added to a UseCase at this time."
+        )
+    raise TypeError(error_message)
+
+
 class UseCase(APIObject):
     """Representation of a Use Case.
 
     Attributes
     ----------
     id : str
         The ID of the Use Case.
@@ -391,59 +437,14 @@
             The updated Use Case.
         """
         payload = {"name": name, "description": description}
         path = f"{self._path}{self.id}/"
         r_data = self._client.patch(path, data=payload).json()
         return self.from_server_data(r_data)
 
-    def _get_reference_entity_info(
-        self, entity: Union[UseCaseReferenceEntity, T]
-    ) -> Tuple[UseCaseAPIPathEntityType, Optional[str]]:
-        """
-        Get the entity type and entity id for a reference entity instance
-        Parameters
-        ----------
-        entity : Union[UseCaseReferenceEntity, Project, Dataset, Application]
-            The entity instance to add to a Use Case.
-        Returns
-        -------
-        entity_info : Tuple[UseCaseEntityType, str]
-            The entity type and entity id
-        """
-        from ..application import Application
-        from ..dataset import Dataset
-        from ..prediction_dataset import PredictionDataset
-        from ..project import Project
-
-        if isinstance(entity, Project):
-            return UseCaseAPIPathEntityType.PROJECT, entity.id
-        elif isinstance(entity, Dataset):
-            return UseCaseAPIPathEntityType.DATASET, entity.id
-        elif isinstance(entity, Application):
-            return UseCaseAPIPathEntityType.APPLICATION, entity.id
-        elif isinstance(entity, UseCaseReferenceEntity):
-            entity_type = UseCaseReferenceEntityMap.get(entity.entity_type)
-            if entity_type:
-                return entity_type, entity.entity_id
-        error_message = (
-            f"Entity must be Project, Dataset, Application, "
-            f"or UseCaseReferenceEntity. Invalid type: {type(entity).__name__}."
-        )
-        if isinstance(entity, UseCaseReferenceEntity):
-            # If we're failing here, it's because the UseCaseReferenceEntity is a notebook or other unsupported type
-            error_message = error_message + f" Unsupported Entity Type: {entity.entity_type}."
-        if isinstance(entity, PredictionDataset):
-            # Adding a specific error for PredictionDataset since the name would indicate it could
-            # be treated as a Dataset, when in fact it's a separate entity and not a subclass.
-            error_message = (
-                error_message + " PredictionDataset is not a subclass of Dataset and "
-                "cannot be added to a UseCase at this time."
-            )
-        raise TypeError(error_message)
-
     def add(
         self,
         entity: Optional[Union[UseCaseReferenceEntity, T]] = None,
         entity_type: Optional[UseCaseEntityType] = None,
         entity_id: Optional[str] = None,
     ) -> UseCaseReferenceEntity:
         """
@@ -475,15 +476,15 @@
         if entity and (e_type or entity_id):
             raise InvalidUsageError(
                 "Can only accept either an entity, or an entity type and entity id."
             )
         if not entity and (not e_type or not entity_id):
             raise InvalidUsageError("Missing entity, or an entity type and entity id.")
         if entity:
-            e_type, e_id = self._get_reference_entity_info(entity)
+            e_type, e_id = get_reference_entity_info(entity)
         path = f"{self._path}{self.id}/{e_type}/{e_id}/"
         r_data = self._client.post(path)
         return UseCaseReferenceEntity.from_server_data(r_data.json())
 
     def remove(
         self,
         entity: Optional[Union[UseCaseReferenceEntity, T]] = None,
@@ -509,15 +510,15 @@
         if entity and (entity_type or entity_id):
             raise InvalidUsageError(
                 "Can only accept either an entity, or an entity type and entity id."
             )
         if not entity and (not entity_type or not entity_id):
             raise InvalidUsageError("Missing entity, or an entity type and entity id.")
         if entity:
-            e_type, e_id = self._get_reference_entity_info(entity)
+            e_type, e_id = get_reference_entity_info(entity)
         path = f"{self._path}{self.id}/{e_type}/{e_id}/"
         self._client.delete(path)
         return None
 
     def share(
         self,
         roles: List[SharingRole],
```

### Comparing `datarobot-3.2.0b0/datarobot/models/use_cases/utils.py` & `datarobot-3.2.0b1/datarobot/models/use_cases/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,31 +6,48 @@
 # DataRobot, Inc.
 #
 # This is proprietary source code of DataRobot, Inc. and its
 # affiliates.
 #
 # Released under the terms of DataRobot Tool and Utility Agreement.
 # pylint: disable=cyclic-import
+import contextvars
 import functools
 from inspect import Parameter, signature
-from typing import Any, Callable, Dict, List, Optional, TypeVar, Union
+from typing import Any, Callable, Dict, List, Optional, Set, Tuple, TypeVar, Union
+import warnings
 
 from typing_extensions import ParamSpec
 
 from datarobot.enums import UseCaseReferenceEntityMap
-from datarobot.errors import InvalidUsageError
-from datarobot.models.use_cases.use_case import UseCase
+from datarobot.errors import InvalidUsageError, MultipleUseCasesNotAllowed
+from datarobot.models.use_cases.use_case import (
+    get_reference_entity_info,
+    UseCase,
+    UseCaseReferenceEntity,
+)
 
 from ...context import Context
+from ...utils.logger import get_logger
 
 P = ParamSpec("P")
 T = TypeVar("T")
 
 UseCaseLike = Union[List[UseCase], UseCase, List[str], str]
 
+_use_case_linked: contextvars.ContextVar[Optional[Set[Tuple[str, str]]]] = contextvars.ContextVar(
+    "use_case_linked", default=None
+)
+_decorator_use_cases: contextvars.ContextVar[Optional[UseCaseLike]] = contextvars.ContextVar(
+    "decorator_use_cases", default=None
+)
+
+
+logger = get_logger(__name__)
+
 
 def resolve_use_cases(
     params: Dict[str, Any],
     use_cases: Optional[UseCaseLike] = None,
     use_case_key: str = "experiment_container_ids",
 ) -> Dict[str, Any]:
     """
@@ -81,14 +98,23 @@
         ]
     if isinstance(use_cases, UseCase):
         return [use_cases.id]
     else:
         return [use_cases]
 
 
+def _add_to_use_case(use_case_id: str, entity: Union[UseCaseReferenceEntity, T]) -> None:
+    _, entity_id = get_reference_entity_info(entity)
+    linked = _use_case_linked.get()
+    if entity_id is not None and linked is not None and (use_case_id, entity_id) not in linked:
+        use_case = UseCase.get(use_case_id=use_case_id)
+        use_case.add(entity=entity)
+        linked.add((use_case_id, entity_id))
+
+
 def add_to_use_case(
     allow_multiple: bool,
 ) -> Callable[[Callable[P, T]], Callable[..., T]]:
     """
     A decorator to mark functions as adding the return value to a given Use Case. When implemented,
     the decorator will add a `use_cases` keyword-only argument to the decorated function or method that
     will automatically add the returned object to a Use Case.
@@ -188,23 +214,47 @@
                 """
                 Parameters
                 ----------
                 use_cases: list[UseCase] | UseCase | list[string] | string, optional
                     A list of UseCase objects, UseCase object,
                     list of Use Case IDs or a single Use Case ID to add this new entity to. Must be a kwarg.
                 """
-                ret = func(*args, **kwargs)
+                use_case_ids = None
+                context_use_case_token = None
+                linked_use_cases_token = None
 
+                # take care of use_case param
                 if use_cases is None:
-                    use_cases = Context.use_case
-                if use_cases is not None:
-                    use_case_ids = resolve_use_case_ids(use_cases=use_cases)
-                    for use_case_id in use_case_ids:
-                        use_case = UseCase.get(use_case_id=use_case_id)
-                        use_case.add(entity=ret)
+                    # check contextvar that could be set by outer iterations first then Context
+                    use_cases = _decorator_use_cases.get(Context.use_case)
+                else:
+                    # if use_case passed, set it to be used by inner calls instead of Context
+                    context_use_case_token = _decorator_use_cases.set(use_cases)
+
+                try:
+                    if use_cases is not None:
+                        # Should only ever resolve to a single use case
+                        use_case_ids = resolve_use_case_ids(use_cases=use_cases)
+
+                    # _use_case_linked never created? must be top level call, initialize set
+                    # to track entities added to UseCase before we call the wrapped function
+                    # as it can also call decorated method inside
+                    if _use_case_linked.get() is None:
+                        linked_use_cases_token = _use_case_linked.set(set())
+                    ret = func(*args, **kwargs)
+
+                    if use_case_ids:
+                        for use_case_id in use_case_ids:
+                            _add_to_use_case(use_case_id, ret)
+                finally:
+                    if context_use_case_token:
+                        _decorator_use_cases.reset(context_use_case_token)
+                    if linked_use_cases_token:
+                        _use_case_linked.reset(linked_use_cases_token)
+
                 return ret
 
             return add_to_multiple
         else:
 
             @functools.wraps(func)
             def add_to_one(
@@ -214,21 +264,49 @@
             ) -> T:
                 """
                 Parameters
                 ----------
                 use_case: UseCase | string, optional
                     A single UseCase object or ID to add this new <return_object_type> to. Must be a kwarg.
                 """
-                ret = func(*args, **kwargs)
+                use_case_id: Optional[str] = None
+                context_use_case_token: Optional[contextvars.Token[Union[UseCaseLike, None]]] = None
+                linked_use_cases_token = None
 
+                # take care of use_case param
                 if use_case is None:
-                    use_case = Context.use_case
-                if use_case is not None:
-                    # Should only ever resolve to a single use case
-                    use_case_id = resolve_use_case_ids(use_cases=use_case)[0]
-                    use_case = UseCase.get(use_case_id=use_case_id)
-                    use_case.add(entity=ret)
+                    # check contextvar that could be set by outer iterations first then Context
+                    use_cases = _decorator_use_cases.get(Context.use_case)
+                    # but it may have been set to a list
+                    if isinstance(use_cases, list):
+                        warnings.warn(MultipleUseCasesNotAllowed())
+                    else:
+                        use_case = use_cases
+                else:
+                    # if use_case passed, set it to be used by inner calls instead of Context
+                    context_use_case_token = _decorator_use_cases.set(use_case)
+
+                try:
+                    if use_case is not None:
+                        # Should only ever resolve to a single use case
+                        use_case_id = resolve_use_case_ids(use_cases=use_case)[0]
+
+                    # _use_case_linked never created? must be top level call, initialize set
+                    # to track entities added to UseCase before we call the wrapped function
+                    # as it can also call decorated method inside
+                    if _use_case_linked.get() is None:
+                        linked_use_cases_token = _use_case_linked.set(set())
+                    ret = func(*args, **kwargs)
+
+                    if use_case_id:
+                        _add_to_use_case(use_case_id, ret)
+                finally:
+                    if context_use_case_token:
+                        _decorator_use_cases.reset(context_use_case_token)
+                    if linked_use_cases_token:
+                        _use_case_linked.reset(linked_use_cases_token)
+
                 return ret
 
             return add_to_one
 
     return wrapper
```

### Comparing `datarobot-3.2.0b0/datarobot/models/user_blueprints/models.py` & `datarobot-3.2.0b1/datarobot/models/user_blueprints/models.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/user_blueprints/trafarets.py` & `datarobot-3.2.0b1/datarobot/models/user_blueprints/trafarets.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/validators.py` & `datarobot-3.2.0b1/datarobot/models/validators.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/visualai/augmentation.py` & `datarobot-3.2.0b1/datarobot/models/visualai/augmentation.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/visualai/images.py` & `datarobot-3.2.0b1/datarobot/models/visualai/images.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/visualai/insights.py` & `datarobot-3.2.0b1/datarobot/models/visualai/insights.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/models/word_cloud.py` & `datarobot-3.2.0b1/datarobot/models/word_cloud.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/rest.py` & `datarobot-3.2.0b1/datarobot/rest.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/utils/__init__.py` & `datarobot-3.2.0b1/datarobot/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/utils/deprecation.py` & `datarobot-3.2.0b1/datarobot/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/utils/pagination.py` & `datarobot-3.2.0b1/datarobot/utils/pagination.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/utils/retry.py` & `datarobot-3.2.0b1/datarobot/utils/retry.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/utils/source.py` & `datarobot-3.2.0b1/datarobot/utils/source.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/utils/sourcedata.py` & `datarobot-3.2.0b1/datarobot/utils/sourcedata.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot/utils/waiters.py` & `datarobot-3.2.0b1/datarobot/utils/waiters.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/datarobot.egg-info/PKG-INFO` & `datarobot-3.2.0b1/datarobot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datarobot
-Version: 3.2.0b0
+Version: 3.2.0b1
 Summary: This client library is designed to support the DataRobot API.
 Home-page: https://datarobot.com
 Author: datarobot
 Author-email: support@datarobot.com
 Maintainer: datarobot
 Maintainer-email: info@datarobot.com
 License: DataRobot Tool and Utility Agreement
```

### Comparing `datarobot-3.2.0b0/datarobot.egg-info/SOURCES.txt` & `datarobot-3.2.0b1/datarobot.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 datarobot/mixins/update_attributes_mixin.py
 datarobot/models/__init__.py
 datarobot/models/advanced_tuning.py
 datarobot/models/anomaly_assessment.py
 datarobot/models/api_object.py
 datarobot/models/application.py
 datarobot/models/automated_documentation.py
+datarobot/models/batch_job.py
 datarobot/models/batch_monitoring_job.py
 datarobot/models/batch_prediction_job.py
 datarobot/models/blueprint.py
 datarobot/models/calendar_file.py
 datarobot/models/change_request.py
 datarobot/models/cluster.py
 datarobot/models/cluster_insight.py
@@ -91,14 +92,15 @@
 datarobot/models/ruleset.py
 datarobot/models/secondary_dataset.py
 datarobot/models/segmentation.py
 datarobot/models/shap_impact.py
 datarobot/models/shap_matrix.py
 datarobot/models/shap_matrix_job.py
 datarobot/models/sharing.py
+datarobot/models/status_check_job.py
 datarobot/models/trafarets.py
 datarobot/models/training_predictions.py
 datarobot/models/types.py
 datarobot/models/validators.py
 datarobot/models/word_cloud.py
 datarobot/models/deployment/__init__.py
 datarobot/models/deployment/accuracy.py
```

### Comparing `datarobot-3.2.0b0/datarobot.egg-info/requires.txt` & `datarobot-3.2.0b1/datarobot.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/pyproject.toml` & `datarobot-3.2.0b1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/setup.py` & `datarobot-3.2.0b1/setup.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.2.0b0/setup_major.py` & `datarobot-3.2.0b1/setup_major.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 # affiliates.
 #
 # Released under the terms of DataRobot Tool and Utility Agreement.
 from setuptools import find_packages, setup
 
 from common_setup import common_setup_kwargs, DEFAULT_CLASSIFIERS, DESCRIPTION_TEMPLATE, version
 
-# if "b" in version:
-#     msg = (
-#         "Major releases must not have a 'b' for beta in the version. "
-#         "Go back and make a release branch with tag, then update the version number."
-#     )
-#     raise RuntimeError(msg)
+if "b" in version:
+    msg = (
+        "Major releases must not have a 'b' for beta in the version. "
+        "Go back and make a release branch with tag, then update the version number."
+    )
+    # raise RuntimeError(msg)
 
 python_versions = ">= 3.7"
 
 description = DESCRIPTION_TEMPLATE.format(
     package_name="datarobot",
     pypi_url_target="https://pypi.python.org/pypi/datarobot/",
     extra_desc="",
```

