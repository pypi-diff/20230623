# Comparing `tmp/dataquality-0.8.9.tar.gz` & `tmp/dataquality-0.9.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataquality-0.8.9.tar", last modified: Thu Dec 15 23:41:39 2022, max compression
+gzip compressed data, was "dataquality-0.9.0a0.tar", last modified: Fri Jun 23 16:27:27 2023, max compression
```

## Comparing `dataquality-0.8.9.tar` & `dataquality-0.9.0a0.tar`

### file list

```diff
@@ -1,176 +1,161 @@
--rw-r--r--   0        0        0       99 2022-10-11 23:00:09.655956 dataquality-0.8.9/.coveragerc
--rw-r--r--   0        0        0      131 2022-10-11 23:00:09.656126 dataquality-0.8.9/.editorconfig
--rw-r--r--   0        0        0      181 2022-10-11 23:00:09.656277 dataquality-0.8.9/.flake8
--rw-r--r--   0        0        0       75 2022-10-11 23:00:09.656495 dataquality-0.8.9/.github/CODEOWNERS
--rw-r--r--   0        0        0      924 2022-10-11 23:00:09.656756 dataquality-0.8.9/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0        0        0      590 2022-10-11 23:00:09.656922 dataquality-0.8.9/.github/ISSUE_TEMPLATE/doc.md
--rw-r--r--   0        0        0      700 2022-10-11 23:00:09.657078 dataquality-0.8.9/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0        0        0      542 2022-10-11 23:00:09.657221 dataquality-0.8.9/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0        0        0     1169 2022-10-11 23:00:09.657374 dataquality-0.8.9/.github/pull_request_template.md
--rw-r--r--   0        0        0      525 2022-10-11 23:00:09.657583 dataquality-0.8.9/.github/workflows/publish.yaml
--rw-r--r--   0        0        0      740 2022-10-11 23:00:09.657729 dataquality-0.8.9/.github/workflows/test.yaml
--rw-r--r--   0        0        0     2292 2022-12-09 01:34:41.687656 dataquality-0.8.9/.gitignore
--rw-r--r--   0        0        0        6 2022-10-11 23:00:09.658013 dataquality-0.8.9/.python-version
--rw-r--r--   0        0        0     8078 2022-10-11 23:00:09.658217 dataquality-0.8.9/CONTRIBUTING.md
--rw-r--r--   0        0        0     1066 2022-10-11 23:00:09.658384 dataquality-0.8.9/LICENSE
--rw-r--r--   0        0        0      548 2022-10-11 23:00:09.658550 dataquality-0.8.9/README.md
--rw-r--r--   0        0        0     4485 2022-12-15 23:41:37.187563 dataquality-0.8.9/dataquality/__init__.py
--rw-r--r--   0        0        0     8443 2022-12-15 23:31:05.910410 dataquality-0.8.9/dataquality/analytics.py
--rw-r--r--   0        0        0        0 2022-10-11 23:00:09.000000 dataquality-0.8.9/dataquality/clients/__init__.py
--rw-r--r--   0        0        0    31697 2022-12-15 23:31:05.927629 dataquality-0.8.9/dataquality/clients/api.py
--rw-r--r--   0        0        0     4125 2022-10-11 23:00:09.000000 dataquality-0.8.9/dataquality/clients/objectstore.py
--rw-r--r--   0        0        0        0 2022-10-11 23:00:09.000000 dataquality-0.8.9/dataquality/core/__init__.py
--rw-r--r--   0        0        0     8371 2022-12-15 23:31:06.069608 dataquality-0.8.9/dataquality/core/_config.py
--rw-r--r--   0        0        0     3104 2022-12-15 23:31:06.045893 dataquality-0.8.9/dataquality/core/auth.py
--rw-r--r--   0        0        0     6108 2022-12-15 23:31:06.082327 dataquality-0.8.9/dataquality/core/finish.py
--rw-r--r--   0        0        0     9768 2022-12-15 23:31:06.062587 dataquality-0.8.9/dataquality/core/init.py
--rw-r--r--   0        0        0    15137 2022-12-15 23:31:06.053808 dataquality-0.8.9/dataquality/core/log.py
--rw-r--r--   0        0        0     7039 2022-12-15 23:31:06.076104 dataquality-0.8.9/dataquality/core/report.py
--rw-r--r--   0        0        0        0 2022-11-28 17:23:58.644880 dataquality-0.8.9/dataquality/dq_auto/__init__.py
--rw-r--r--   0        0        0     9405 2022-12-15 23:31:06.393084 dataquality-0.8.9/dataquality/dq_auto/auto.py
--rw-r--r--   0        0        0     4098 2022-12-15 23:31:06.333955 dataquality-0.8.9/dataquality/dq_auto/base_data_manager.py
--rw-r--r--   0        0        0     7262 2022-12-15 23:31:06.379759 dataquality-0.8.9/dataquality/dq_auto/ner.py
--rw-r--r--   0        0        0     3768 2022-12-15 23:31:06.310402 dataquality-0.8.9/dataquality/dq_auto/ner_trainer.py
--rw-r--r--   0        0        0     3070 2022-12-15 23:31:06.384090 dataquality-0.8.9/dataquality/dq_auto/tc_trainer.py
--rw-r--r--   0        0        0    11287 2022-12-15 23:31:06.373912 dataquality-0.8.9/dataquality/dq_auto/text_classification.py
--rw-r--r--   0        0        0      293 2022-10-31 17:31:56.991517 dataquality-0.8.9/dataquality/exceptions.py
--rw-r--r--   0        0        0        0 2022-10-11 23:00:09.000000 dataquality-0.8.9/dataquality/integrations/__init__.py
--rw-r--r--   0        0        0    15422 2022-12-15 23:31:06.300508 dataquality-0.8.9/dataquality/integrations/experimental/keras.py
--rw-r--r--   0        0        0     9603 2022-12-15 23:31:06.289374 dataquality-0.8.9/dataquality/integrations/hf.py
--rw-r--r--   0        0        0     4418 2022-12-15 23:31:06.250210 dataquality-0.8.9/dataquality/integrations/keras.py
--rw-r--r--   0        0        0    25573 2022-12-15 23:31:06.275830 dataquality-0.8.9/dataquality/integrations/spacy.py
--rw-r--r--   0        0        0     5701 2022-12-15 23:31:06.281061 dataquality-0.8.9/dataquality/integrations/torch.py
--rw-r--r--   0        0        0     8344 2022-12-15 23:31:06.259439 dataquality-0.8.9/dataquality/integrations/transformers_trainer.py
--rw-r--r--   0        0        0       95 2022-10-11 23:00:09.000000 dataquality-0.8.9/dataquality/loggers/__init__.py
--rw-r--r--   0        0        0    10577 2022-12-15 23:31:05.945221 dataquality-0.8.9/dataquality/loggers/base_logger.py
--rw-r--r--   0        0        0      357 2022-12-15 23:31:05.989196 dataquality-0.8.9/dataquality/loggers/data_logger/__init__.py
--rw-r--r--   0        0        0    21618 2022-12-15 23:31:06.020215 dataquality-0.8.9/dataquality/loggers/data_logger/base_data_logger.py
--rw-r--r--   0        0        0     1935 2022-12-15 23:31:05.986971 dataquality-0.8.9/dataquality/loggers/data_logger/image_classification.py
--rw-r--r--   0        0        0    19532 2022-12-15 23:31:05.994896 dataquality-0.8.9/dataquality/loggers/data_logger/text_classification.py
--rw-r--r--   0        0        0    14796 2022-12-15 23:31:06.000577 dataquality-0.8.9/dataquality/loggers/data_logger/text_multi_label.py
--rw-r--r--   0        0        0    31289 2022-12-15 23:31:06.009806 dataquality-0.8.9/dataquality/loggers/data_logger/text_ner.py
--rw-r--r--   0        0        0        0 2022-10-11 23:00:09.000000 dataquality-0.8.9/dataquality/loggers/logger_config/__init__.py
--rw-r--r--   0        0        0     1702 2022-12-15 23:31:06.039210 dataquality-0.8.9/dataquality/loggers/logger_config/base_logger_config.py
--rw-r--r--   0        0        0      260 2022-12-09 01:34:41.691356 dataquality-0.8.9/dataquality/loggers/logger_config/image_classification.py
--rw-r--r--   0        0        0      958 2022-12-15 23:31:06.029388 dataquality-0.8.9/dataquality/loggers/logger_config/text_classification.py
--rw-r--r--   0        0        0     1510 2022-12-15 23:31:06.032713 dataquality-0.8.9/dataquality/loggers/logger_config/text_multi_label.py
--rw-r--r--   0        0        0     1608 2022-12-15 23:31:06.036035 dataquality-0.8.9/dataquality/loggers/logger_config/text_ner.py
--rw-r--r--   0        0        0      362 2022-12-15 23:31:05.953592 dataquality-0.8.9/dataquality/loggers/model_logger/__init__.py
--rw-r--r--   0        0        0     8218 2022-12-15 23:31:05.979653 dataquality-0.8.9/dataquality/loggers/model_logger/base_model_logger.py
--rw-r--r--   0        0        0     1015 2022-12-15 23:31:05.950221 dataquality-0.8.9/dataquality/loggers/model_logger/image_classification.py
--rw-r--r--   0        0        0     7838 2022-12-15 23:31:05.958149 dataquality-0.8.9/dataquality/loggers/model_logger/text_classification.py
--rw-r--r--   0        0        0     9058 2022-12-15 23:31:05.963261 dataquality-0.8.9/dataquality/loggers/model_logger/text_multi_label.py
--rw-r--r--   0        0        0    33524 2022-12-15 23:31:05.972893 dataquality-0.8.9/dataquality/loggers/model_logger/text_ner.py
--rw-r--r--   0        0        0    27895 2022-12-15 23:31:05.890944 dataquality-0.8.9/dataquality/metrics.py
--rw-r--r--   0        0        0      165 2022-10-11 23:00:09.000000 dataquality-0.8.9/dataquality/schemas/__init__.py
--rw-r--r--   0        0        0     8363 2022-12-15 23:31:06.224815 dataquality-0.8.9/dataquality/schemas/condition.py
--rw-r--r--   0        0        0      570 2022-12-15 23:31:06.204166 dataquality-0.8.9/dataquality/schemas/dataframe.py
--rw-r--r--   0        0        0     4382 2022-12-15 23:31:06.220218 dataquality-0.8.9/dataquality/schemas/edit.py
--rw-r--r--   0        0        0      662 2022-11-28 17:23:58.658371 dataquality-0.8.9/dataquality/schemas/hf.py
--rw-r--r--   0        0        0      118 2022-12-15 23:31:06.206491 dataquality-0.8.9/dataquality/schemas/job.py
--rw-r--r--   0        0        0     5254 2022-12-15 23:31:06.201016 dataquality-0.8.9/dataquality/schemas/metrics.py
--rw-r--r--   0        0        0      992 2022-12-15 23:31:06.228257 dataquality-0.8.9/dataquality/schemas/ner.py
--rw-r--r--   0        0        0      617 2022-12-15 23:31:06.239527 dataquality-0.8.9/dataquality/schemas/report.py
--rw-r--r--   0        0        0      287 2022-10-11 23:00:09.000000 dataquality-0.8.9/dataquality/schemas/request_type.py
--rw-r--r--   0        0        0     1397 2022-12-15 23:31:06.209696 dataquality-0.8.9/dataquality/schemas/route.py
--rw-r--r--   0        0        0      928 2022-12-15 23:31:06.231109 dataquality-0.8.9/dataquality/schemas/split.py
--rw-r--r--   0        0        0      770 2022-12-15 23:31:06.234039 dataquality-0.8.9/dataquality/schemas/task_type.py
--rw-r--r--   0        0        0      244 2022-12-15 23:31:06.236970 dataquality-0.8.9/dataquality/schemas/torch.py
--rw-r--r--   0        0        0      222 2022-10-11 23:00:09.000000 dataquality-0.8.9/dataquality/utils/__init__.py
--rw-r--r--   0        0        0      674 2022-11-02 20:22:30.684530 dataquality-0.8.9/dataquality/utils/ampli.py
--rw-r--r--   0        0        0      401 2022-12-15 23:31:06.089109 dataquality-0.8.9/dataquality/utils/auth.py
--rw-r--r--   0        0        0     5784 2022-12-15 23:31:06.193967 dataquality-0.8.9/dataquality/utils/auto.py
--rw-r--r--   0        0        0      865 2022-12-15 21:23:01.762336 dataquality-0.8.9/dataquality/utils/auto_trainer.py
--rw-r--r--   0        0        0      154 2022-12-15 23:31:06.103700 dataquality-0.8.9/dataquality/utils/cloud.py
--rw-r--r--   0        0        0      651 2022-12-09 01:34:41.693535 dataquality-0.8.9/dataquality/utils/cv.py
--rw-r--r--   0        0        0     3381 2022-12-15 23:31:06.154205 dataquality-0.8.9/dataquality/utils/dq_logger.py
--rw-r--r--   0        0        0      129 2022-10-11 23:00:09.000000 dataquality-0.8.9/dataquality/utils/file.py
--rw-r--r--   0        0        0     1672 2022-12-15 23:31:06.129311 dataquality-0.8.9/dataquality/utils/hdf5_store.py
--rw-r--r--   0        0        0     3039 2022-12-15 23:31:06.189283 dataquality-0.8.9/dataquality/utils/helpers.py
--rw-r--r--   0        0        0     9962 2022-12-15 23:31:06.095391 dataquality-0.8.9/dataquality/utils/hf_tokenizer.py
--rw-r--r--   0        0        0      429 2022-11-28 17:23:58.665769 dataquality-0.8.9/dataquality/utils/imports.py
--rw-r--r--   0        0        0     7977 2022-12-15 23:31:06.111254 dataquality-0.8.9/dataquality/utils/keras.py
--rw-r--r--   0        0        0     2408 2022-12-15 23:31:06.142227 dataquality-0.8.9/dataquality/utils/ml.py
--rw-r--r--   0        0        0    23873 2022-11-02 20:22:30.685786 dataquality-0.8.9/dataquality/utils/name.py
--rw-r--r--   0        0        0     5923 2022-12-15 23:31:06.177280 dataquality-0.8.9/dataquality/utils/profiler.py
--rw-r--r--   0        0        0     4070 2022-12-15 23:31:06.125979 dataquality-0.8.9/dataquality/utils/spacy_integration.py
--rw-r--r--   0        0        0      260 2022-11-28 17:23:58.668908 dataquality-0.8.9/dataquality/utils/tf.py
--rw-r--r--   0        0        0     1912 2022-12-15 23:31:06.114129 dataquality-0.8.9/dataquality/utils/thread_pool.py
--rw-r--r--   0        0        0     9488 2022-12-15 23:31:06.185769 dataquality-0.8.9/dataquality/utils/torch.py
--rw-r--r--   0        0        0     2739 2022-12-15 23:31:06.106465 dataquality-0.8.9/dataquality/utils/transformers.py
--rw-r--r--   0        0        0     9149 2022-12-15 23:31:06.136612 dataquality-0.8.9/dataquality/utils/vaex.py
--rw-r--r--   0        0        0     1440 2022-11-02 20:22:30.688040 dataquality-0.8.9/dataquality/utils/version.py
--rw-r--r--   0        0        0    18832 2022-10-11 23:00:09.671318 dataquality-0.8.9/docs/Dataquality-Client-Demo.ipynb
--rw-r--r--   0        0        0    10352 2022-12-06 23:24:23.704737 dataquality-0.8.9/docs/End to End runs per task type.ipynb
--rw-r--r--   0        0        0    12031 2022-10-11 23:00:09.671739 dataquality-0.8.9/docs/Inference-Demo.ipynb
--rw-r--r--   0        0        0     6893 2022-10-11 23:00:09.671910 dataquality-0.8.9/docs/NER Inference.ipynb
--rw-r--r--   0        0        0      172 2022-12-09 01:34:41.694895 dataquality-0.8.9/docs/cv/README.md
--rw-r--r--   0        0        0     4245 2022-12-09 01:34:41.695431 dataquality-0.8.9/docs/cv/cv-demo-hf.py
--rw-r--r--   0        0        0     1893 2022-12-09 01:34:41.695867 dataquality-0.8.9/docs/cv/cv-testing-benchmark.py
--rw-r--r--   0        0        0      154 2022-10-11 23:00:09.672060 dataquality-0.8.9/docs/index.md
--rw-r--r--   0        0        0       61 2022-10-11 23:00:09.672196 dataquality-0.8.9/mkdocs.yml
--rw-r--r--   0        0        0       66 2022-10-11 23:00:09.672321 dataquality-0.8.9/mypy.ini
--rw-r--r--   0        0        0     1571 2022-12-15 21:23:01.763974 dataquality-0.8.9/pyproject.toml
--rw-r--r--   0        0        0       61 2022-10-11 23:00:09.672594 dataquality-0.8.9/pytest.ini
--rwxr-xr-x   0        0        0      247 2022-10-11 23:00:09.672835 dataquality-0.8.9/scripts/bump-version.sh
--rwxr-xr-x   0        0        0      100 2022-10-11 23:00:09.672960 dataquality-0.8.9/scripts/clean.sh
--rwxr-xr-x   0        0        0       60 2022-10-11 23:00:09.673077 dataquality-0.8.9/scripts/docs-build.sh
--rwxr-xr-x   0        0        0       55 2022-10-11 23:00:09.673199 dataquality-0.8.9/scripts/docs-serve.sh
--rwxr-xr-x   0        0        0      320 2022-10-11 23:00:09.673322 dataquality-0.8.9/scripts/format.sh
--rwxr-xr-x   0        0        0      106 2022-10-11 23:00:09.673446 dataquality-0.8.9/scripts/install.sh
--rwxr-xr-x   0        0        0      126 2022-10-11 23:00:09.673573 dataquality-0.8.9/scripts/lint.sh
--rwxr-xr-x   0        0        0       29 2022-10-11 23:00:09.673690 dataquality-0.8.9/scripts/publish.sh
--rwxr-xr-x   0        0        0       66 2022-10-11 23:00:09.673820 dataquality-0.8.9/scripts/set-local-env.sh
--rwxr-xr-x   0        0        0       56 2022-10-11 23:00:09.673948 dataquality-0.8.9/scripts/test-cov-html.sh
--rwxr-xr-x   0        0        0      216 2022-10-11 23:00:09.674078 dataquality-0.8.9/scripts/test.sh
--rw-r--r--   0        0        0        0 2022-10-11 23:00:09.674219 dataquality-0.8.9/tests/__init__.py
--rw-r--r--   0        0        0     3479 2022-12-15 23:31:06.527876 dataquality-0.8.9/tests/auto/test_ner_auto.py
--rw-r--r--   0        0        0    16171 2022-12-15 23:31:06.523820 dataquality-0.8.9/tests/auto/test_tc_auto.py
--rw-r--r--   0        0        0    10549 2022-12-15 23:31:06.444129 dataquality-0.8.9/tests/clients/test_api.py
--rw-r--r--   0        0        0     5852 2022-12-15 23:31:06.418269 dataquality-0.8.9/tests/conftest.py
--rw-r--r--   0        0        0     1409 2022-12-15 23:31:06.481108 dataquality-0.8.9/tests/core/test_auth.py
--rw-r--r--   0        0        0      418 2022-11-02 20:22:30.689801 dataquality-0.8.9/tests/core/test_cloud.py
--rw-r--r--   0        0        0     6719 2022-12-15 23:31:06.497841 dataquality-0.8.9/tests/core/test_config.py
--rw-r--r--   0        0        0     6122 2022-12-15 23:31:06.492412 dataquality-0.8.9/tests/core/test_finish.py
--rw-r--r--   0        0        0    15940 2022-12-15 23:31:06.511453 dataquality-0.8.9/tests/core/test_init.py
--rw-r--r--   0        0        0     6907 2022-12-15 23:31:06.487171 dataquality-0.8.9/tests/core/test_report.py
--rw-r--r--   0        0        0       40 2022-10-11 23:00:09.674520 dataquality-0.8.9/tests/exceptions.py
--rw-r--r--   0        0        0     4990 2022-12-15 23:31:06.709420 dataquality-0.8.9/tests/inference/test_inference.py
--rw-r--r--   0        0        0     3234 2022-11-02 20:22:30.691277 dataquality-0.8.9/tests/inference/test_text_classification_inf.py
--rw-r--r--   0        0        0     3792 2022-11-02 20:22:30.691419 dataquality-0.8.9/tests/inference/test_text_ner_inf.py
--rw-r--r--   0        0        0     3862 2022-10-11 23:00:09.675468 dataquality-0.8.9/tests/integration/mock_training_run.py
--rw-r--r--   0        0        0     3954 2022-12-15 23:31:06.679834 dataquality-0.8.9/tests/integrations/hf/test_cv_hf.py
--rw-r--r--   0        0        0    10897 2022-12-15 23:31:06.673447 dataquality-0.8.9/tests/integrations/hf/test_hf_integration.py
--rw-r--r--   0        0        0    10123 2022-12-15 23:31:06.662649 dataquality-0.8.9/tests/integrations/hf/test_text_classification_hf.py
--rw-r--r--   0        0        0     9263 2022-12-15 23:31:06.640380 dataquality-0.8.9/tests/integrations/keras/test_experimental.py
--rw-r--r--   0        0        0      514 2022-12-15 21:23:01.768632 dataquality-0.8.9/tests/integrations/keras/test_utils.py
--rw-r--r--   0        0        0     1346 2022-12-15 23:31:06.689001 dataquality-0.8.9/tests/integrations/spacy/conftest.py
--rw-r--r--   0        0        0      760 2022-11-02 20:22:30.692338 dataquality-0.8.9/tests/integrations/spacy/test_spacy_integration.py
--rw-r--r--   0        0        0    16355 2022-12-15 23:31:06.699854 dataquality-0.8.9/tests/integrations/spacy/test_spacy_ner.py
--rw-r--r--   0        0        0      904 2022-12-15 23:31:06.645632 dataquality-0.8.9/tests/integrations/torch/test_pt_utils.py
--rw-r--r--   0        0        0     7367 2022-12-15 23:31:06.653430 dataquality-0.8.9/tests/integrations/torch/test_text_classification_pt.py
--rw-r--r--   0        0        0    11728 2022-12-15 23:31:06.453921 dataquality-0.8.9/tests/loggers/test_multi_label.py
--rw-r--r--   0        0        0    23385 2022-12-15 23:31:06.475658 dataquality-0.8.9/tests/loggers/test_ner.py
--rw-r--r--   0        0        0    13108 2022-12-15 23:31:06.460897 dataquality-0.8.9/tests/loggers/test_text_classification.py
--rw-r--r--   0        0        0     7226 2022-12-15 23:31:06.622782 dataquality-0.8.9/tests/schemas/test_conditions.py
--rw-r--r--   0        0        0      402 2022-11-02 20:22:30.695867 dataquality-0.8.9/tests/schemas/test_metrics.py
--rw-r--r--   0        0        0    29166 2022-12-15 23:31:06.434729 dataquality-0.8.9/tests/test_dataquality.py
--rw-r--r--   0        0        0     1783 2022-11-28 17:23:58.686840 dataquality-0.8.9/tests/test_telemetrics.py
--rw-r--r--   0        0        0        0 2022-11-02 20:22:30.697603 dataquality-0.8.9/tests/test_utils/__init__.py
--rw-r--r--   0        0        0     5900 2022-12-15 23:31:06.565806 dataquality-0.8.9/tests/test_utils/data_utils.py
--rw-r--r--   0        0        0     3808 2022-12-15 23:31:06.536970 dataquality-0.8.9/tests/test_utils/hf_datasets_mock.py
--rw-r--r--   0        0        0    11378 2022-11-02 20:22:30.698317 dataquality-0.8.9/tests/test_utils/hf_integration_constants.py
--rw-r--r--   0        0        0     8122 2022-11-28 17:23:58.687297 dataquality-0.8.9/tests/test_utils/hf_integration_constants_inference.py
--rw-r--r--   0        0        0     3695 2022-11-02 20:22:30.698590 dataquality-0.8.9/tests/test_utils/lightning_model.py
--rw-r--r--   0        0        0     4908 2022-12-15 23:31:06.548195 dataquality-0.8.9/tests/test_utils/mock_request.py
--rw-r--r--   0        0        0     2840 2022-11-02 20:22:30.699379 dataquality-0.8.9/tests/test_utils/ner_constants.py
--rw-r--r--   0        0        0     4239 2022-12-15 23:31:06.553629 dataquality-0.8.9/tests/test_utils/spacy_integration.py
--rw-r--r--   0        0        0    22487 2022-12-06 23:24:23.709042 dataquality-0.8.9/tests/test_utils/spacy_integration_constants.py
--rw-r--r--   0        0        0    23021 2022-12-06 23:24:23.709498 dataquality-0.8.9/tests/test_utils/spacy_integration_constants_inference.py
--rw-r--r--   0        0        0     4614 2022-12-15 23:31:06.607721 dataquality-0.8.9/tests/utils/test_auto.py
--rw-r--r--   0        0        0     1623 2022-11-02 20:22:30.700412 dataquality-0.8.9/tests/utils/test_dq_logger.py
--rw-r--r--   0        0        0      224 2022-12-15 23:31:06.612161 dataquality-0.8.9/tests/utils/test_name.py
--rw-r--r--   0        0        0      288 2022-11-28 17:23:58.689269 dataquality-0.8.9/tests/utils/test_tf_version.py
--rw-r--r--   0        0        0      601 2022-11-02 20:22:30.701010 dataquality-0.8.9/tests/utils/test_vaex_utils.py
--rw-r--r--   0        0        0     1316 2022-12-15 23:31:06.599087 dataquality-0.8.9/tests/utils/test_version.py
--rw-r--r--   0        0        0     2735 1970-01-01 00:00:00.000000 dataquality-0.8.9/PKG-INFO
+drwxr-xr-x   0 franz      (501) staff       (20)        0 2023-06-23 16:27:27.793130 dataquality-0.9.0a0/
+-rw-r--r--   0 franz      (501) staff       (20)     1066 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/LICENSE
+-rw-r--r--   0 franz      (501) staff       (20)     4939 2023-06-23 16:27:27.793340 dataquality-0.9.0a0/PKG-INFO
+-rw-r--r--   0 franz      (501) staff       (20)     4429 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/README.md
+drwxr-xr-x   0 franz      (501) staff       (20)        0 2023-06-23 16:27:27.703515 dataquality-0.9.0a0/dataquality/
+-rw-r--r--   0 franz      (501) staff       (20)     6071 2023-06-23 16:27:08.000000 dataquality-0.9.0a0/dataquality/__init__.py
+-rw-r--r--   0 franz      (501) staff       (20)     8300 2023-06-23 16:26:44.000000 dataquality-0.9.0a0/dataquality/analytics.py
+drwxr-xr-x   0 franz      (501) staff       (20)        0 2023-06-23 16:27:27.707654 dataquality-0.9.0a0/dataquality/clients/
+-rw-r--r--   0 franz      (501) staff       (20)        0 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/clients/__init__.py
+-rw-r--r--   0 franz      (501) staff       (20)    33222 2023-06-21 17:17:50.000000 dataquality-0.9.0a0/dataquality/clients/api.py
+-rw-r--r--   0 franz      (501) staff       (20)     8187 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/clients/objectstore.py
+drwxr-xr-x   0 franz      (501) staff       (20)        0 2023-06-23 16:27:27.710400 dataquality-0.9.0a0/dataquality/core/
+-rw-r--r--   0 franz      (501) staff       (20)     1848 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/core/__init__.py
+-rw-r--r--   0 franz      (501) staff       (20)     9495 2023-06-21 17:17:50.000000 dataquality-0.9.0a0/dataquality/core/_config.py
+-rw-r--r--   0 franz      (501) staff       (20)     3104 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/core/auth.py
+-rw-r--r--   0 franz      (501) staff       (20)     6499 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/core/finish.py
+-rw-r--r--   0 franz      (501) staff       (20)     9615 2023-06-21 17:17:50.000000 dataquality-0.9.0a0/dataquality/core/init.py
+-rw-r--r--   0 franz      (501) staff       (20)    23390 2023-06-21 17:17:50.000000 dataquality-0.9.0a0/dataquality/core/log.py
+-rw-r--r--   0 franz      (501) staff       (20)     7039 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/core/report.py
+drwxr-xr-x   0 franz      (501) staff       (20)        0 2023-06-23 16:27:27.714469 dataquality-0.9.0a0/dataquality/dq_auto/
+-rw-r--r--   0 franz      (501) staff       (20)        0 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/dq_auto/__init__.py
+-rw-r--r--   0 franz      (501) staff       (20)    10048 2023-06-21 17:17:50.000000 dataquality-0.9.0a0/dataquality/dq_auto/auto.py
+-rw-r--r--   0 franz      (501) staff       (20)     4699 2023-06-21 17:17:50.000000 dataquality-0.9.0a0/dataquality/dq_auto/base_data_manager.py
+-rw-r--r--   0 franz      (501) staff       (20)     7430 2023-06-21 17:17:50.000000 dataquality-0.9.0a0/dataquality/dq_auto/ner.py
+-rw-r--r--   0 franz      (501) staff       (20)     4265 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/dq_auto/ner_trainer.py
+-rw-r--r--   0 franz      (501) staff       (20)     1594 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/dq_auto/notebook.py
+-rw-r--r--   0 franz      (501) staff       (20)     3559 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/dq_auto/tc_trainer.py
+-rw-r--r--   0 franz      (501) staff       (20)    10676 2023-06-21 17:17:50.000000 dataquality-0.9.0a0/dataquality/dq_auto/text_classification.py
+drwxr-xr-x   0 franz      (501) staff       (20)        0 2023-06-23 16:27:27.715032 dataquality-0.9.0a0/dataquality/dq_start/
+-rw-r--r--   0 franz      (501) staff       (20)    11313 2023-06-23 16:26:44.000000 dataquality-0.9.0a0/dataquality/dq_start/__init__.py
+-rw-r--r--   0 franz      (501) staff       (20)     4512 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/dqyolo.py
+-rw-r--r--   0 franz      (501) staff       (20)      293 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/exceptions.py
+drwxr-xr-x   0 franz      (501) staff       (20)        0 2023-06-23 16:27:27.719267 dataquality-0.9.0a0/dataquality/integrations/
+-rw-r--r--   0 franz      (501) staff       (20)        0 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/integrations/__init__.py
+-rw-r--r--   0 franz      (501) staff       (20)    14966 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/integrations/fastai.py
+-rw-r--r--   0 franz      (501) staff       (20)    10024 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/integrations/hf.py
+-rw-r--r--   0 franz      (501) staff       (20)    15575 2023-06-23 16:26:44.000000 dataquality-0.9.0a0/dataquality/integrations/keras.py
+-rw-r--r--   0 franz      (501) staff       (20)    14309 2023-06-21 17:17:50.000000 dataquality-0.9.0a0/dataquality/integrations/setfit.py
+-rw-r--r--   0 franz      (501) staff       (20)    13302 2023-06-23 16:26:44.000000 dataquality-0.9.0a0/dataquality/integrations/torch.py
+-rw-r--r--   0 franz      (501) staff       (20)    27174 2023-06-23 16:26:44.000000 dataquality-0.9.0a0/dataquality/integrations/torch_semantic_segmentation.py
+-rw-r--r--   0 franz      (501) staff       (20)    13430 2023-06-23 16:26:44.000000 dataquality-0.9.0a0/dataquality/integrations/transformers_trainer.py
+-rw-r--r--   0 franz      (501) staff       (20)    17147 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/integrations/ultralytics.py
+-rw-r--r--   0 franz      (501) staff       (20)     4165 2023-06-21 17:17:50.000000 dataquality-0.9.0a0/dataquality/internal.py
+drwxr-xr-x   0 franz      (501) staff       (20)        0 2023-06-23 16:27:27.720398 dataquality-0.9.0a0/dataquality/loggers/
+-rw-r--r--   0 franz      (501) staff       (20)       95 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/loggers/__init__.py
+-rw-r--r--   0 franz      (501) staff       (20)    13410 2023-06-21 17:17:50.000000 dataquality-0.9.0a0/dataquality/loggers/base_logger.py
+drwxr-xr-x   0 franz      (501) staff       (20)        0 2023-06-23 16:27:27.724043 dataquality-0.9.0a0/dataquality/loggers/data_logger/
+-rw-r--r--   0 franz      (501) staff       (20)      517 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/loggers/data_logger/__init__.py
+-rw-r--r--   0 franz      (501) staff       (20)    27255 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/loggers/data_logger/base_data_logger.py
+-rw-r--r--   0 franz      (501) staff       (20)    12826 2023-06-23 16:26:44.000000 dataquality-0.9.0a0/dataquality/loggers/data_logger/image_classification.py
+-rw-r--r--   0 franz      (501) staff       (20)    10355 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/loggers/data_logger/object_detection.py
+-rw-r--r--   0 franz      (501) staff       (20)     5888 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/loggers/data_logger/semantic_segmentation.py
+-rw-r--r--   0 franz      (501) staff       (20)     9864 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/loggers/data_logger/tabular_classification.py
+-rw-r--r--   0 franz      (501) staff       (20)    21106 2023-06-21 17:17:50.000000 dataquality-0.9.0a0/dataquality/loggers/data_logger/text_classification.py
+-rw-r--r--   0 franz      (501) staff       (20)    14941 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/loggers/data_logger/text_multi_label.py
+-rw-r--r--   0 franz      (501) staff       (20)    31953 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/loggers/data_logger/text_ner.py
+drwxr-xr-x   0 franz      (501) staff       (20)        0 2023-06-23 16:27:27.729046 dataquality-0.9.0a0/dataquality/loggers/logger_config/
+-rw-r--r--   0 franz      (501) staff       (20)        0 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/loggers/logger_config/__init__.py
+-rw-r--r--   0 franz      (501) staff       (20)     2042 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/loggers/logger_config/base_logger_config.py
+-rw-r--r--   0 franz      (501) staff       (20)      510 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/loggers/logger_config/image_classification.py
+-rw-r--r--   0 franz      (501) staff       (20)      537 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/loggers/logger_config/object_detection.py
+-rw-r--r--   0 franz      (501) staff       (20)      226 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/loggers/logger_config/semantic_segmentation.py
+-rw-r--r--   0 franz      (501) staff       (20)      398 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/loggers/logger_config/tabular_classification.py
+-rw-r--r--   0 franz      (501) staff       (20)      958 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/loggers/logger_config/text_classification.py
+-rw-r--r--   0 franz      (501) staff       (20)     1510 2023-06-21 17:18:47.000000 dataquality-0.9.0a0/dataquality/loggers/logger_config/text_multi_label.py
+-rw-r--r--   0 franz      (501) staff       (20)     1608 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/loggers/logger_config/text_ner.py
+drwxr-xr-x   0 franz      (501) staff       (20)        0 2023-06-23 16:27:27.732480 dataquality-0.9.0a0/dataquality/loggers/model_logger/
+-rw-r--r--   0 franz      (501) staff       (20)      420 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/loggers/model_logger/__init__.py
+-rw-r--r--   0 franz      (501) staff       (20)     7510 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/loggers/model_logger/base_model_logger.py
+-rw-r--r--   0 franz      (501) staff       (20)     3309 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/loggers/model_logger/image_classification.py
+-rw-r--r--   0 franz      (501) staff       (20)     9435 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/loggers/model_logger/object_detection.py
+-rw-r--r--   0 franz      (501) staff       (20)    11742 2023-06-23 16:26:44.000000 dataquality-0.9.0a0/dataquality/loggers/model_logger/semantic_segmentation.py
+-rw-r--r--   0 franz      (501) staff       (20)      519 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/loggers/model_logger/tabular_classification.py
+-rw-r--r--   0 franz      (501) staff       (20)     7555 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/loggers/model_logger/text_classification.py
+-rw-r--r--   0 franz      (501) staff       (20)     9120 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/loggers/model_logger/text_multi_label.py
+-rw-r--r--   0 franz      (501) staff       (20)    32052 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/loggers/model_logger/text_ner.py
+-rw-r--r--   0 franz      (501) staff       (20)    28653 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/metrics.py
+-rw-r--r--   0 franz      (501) staff       (20)        0 2023-06-21 17:17:50.000000 dataquality-0.9.0a0/dataquality/py.typed
+drwxr-xr-x   0 franz      (501) staff       (20)        0 2023-06-23 16:27:27.746117 dataquality-0.9.0a0/dataquality/schemas/
+-rw-r--r--   0 franz      (501) staff       (20)      165 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/schemas/__init__.py
+-rw-r--r--   0 franz      (501) staff       (20)     8361 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/schemas/condition.py
+-rw-r--r--   0 franz      (501) staff       (20)      569 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/schemas/dataframe.py
+-rw-r--r--   0 franz      (501) staff       (20)     4382 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/schemas/edit.py
+-rw-r--r--   0 franz      (501) staff       (20)      662 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/schemas/hf.py
+-rw-r--r--   0 franz      (501) staff       (20)      118 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/schemas/job.py
+-rw-r--r--   0 franz      (501) staff       (20)     5241 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/schemas/metrics.py
+-rw-r--r--   0 franz      (501) staff       (20)      145 2023-06-23 16:26:44.000000 dataquality-0.9.0a0/dataquality/schemas/model.py
+-rw-r--r--   0 franz      (501) staff       (20)      992 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/schemas/ner.py
+-rw-r--r--   0 franz      (501) staff       (20)      617 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/schemas/report.py
+-rw-r--r--   0 franz      (501) staff       (20)      287 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/schemas/request_type.py
+-rw-r--r--   0 franz      (501) staff       (20)     1495 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/schemas/route.py
+-rw-r--r--   0 franz      (501) staff       (20)     4190 2023-06-23 16:26:44.000000 dataquality-0.9.0a0/dataquality/schemas/semantic_segmentation.py
+-rw-r--r--   0 franz      (501) staff       (20)      992 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/schemas/split.py
+-rw-r--r--   0 franz      (501) staff       (20)     1295 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/schemas/task_type.py
+-rw-r--r--   0 franz      (501) staff       (20)      740 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/schemas/torch.py
+drwxr-xr-x   0 franz      (501) staff       (20)        0 2023-06-23 16:27:27.772433 dataquality-0.9.0a0/dataquality/utils/
+-rw-r--r--   0 franz      (501) staff       (20)      222 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/utils/__init__.py
+-rw-r--r--   0 franz      (501) staff       (20)      634 2023-06-23 16:26:44.000000 dataquality-0.9.0a0/dataquality/utils/ampli.py
+-rw-r--r--   0 franz      (501) staff       (20)      401 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/utils/auth.py
+-rw-r--r--   0 franz      (501) staff       (20)     8903 2023-06-21 17:17:50.000000 dataquality-0.9.0a0/dataquality/utils/auto.py
+-rw-r--r--   0 franz      (501) staff       (20)      925 2023-06-21 17:17:50.000000 dataquality-0.9.0a0/dataquality/utils/auto_trainer.py
+-rw-r--r--   0 franz      (501) staff       (20)      154 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/utils/cloud.py
+-rw-r--r--   0 franz      (501) staff       (20)     1229 2023-06-21 17:17:50.000000 dataquality-0.9.0a0/dataquality/utils/cuda.py
+-rw-r--r--   0 franz      (501) staff       (20)     2082 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/utils/cv.py
+-rw-r--r--   0 franz      (501) staff       (20)     3387 2023-06-21 17:17:50.000000 dataquality-0.9.0a0/dataquality/utils/dq_logger.py
+-rw-r--r--   0 franz      (501) staff       (20)     3514 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/utils/dqyolo.py
+-rw-r--r--   0 franz      (501) staff       (20)     4898 2023-06-21 17:17:50.000000 dataquality-0.9.0a0/dataquality/utils/emb.py
+-rw-r--r--   0 franz      (501) staff       (20)     3591 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/utils/file.py
+-rw-r--r--   0 franz      (501) staff       (20)     5685 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/utils/hdf5_store.py
+-rw-r--r--   0 franz      (501) staff       (20)     3784 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/utils/helpers.py
+-rw-r--r--   0 franz      (501) staff       (20)     2163 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/utils/hf_images.py
+-rw-r--r--   0 franz      (501) staff       (20)    10182 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/utils/hf_tokenizer.py
+-rw-r--r--   0 franz      (501) staff       (20)      429 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/utils/imports.py
+-rw-r--r--   0 franz      (501) staff       (20)     8023 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/utils/keras.py
+-rw-r--r--   0 franz      (501) staff       (20)     2408 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/utils/ml.py
+-rw-r--r--   0 franz      (501) staff       (20)    24732 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/utils/name.py
+-rw-r--r--   0 franz      (501) staff       (20)     1661 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/utils/od.py
+-rw-r--r--   0 franz      (501) staff       (20)     3187 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/utils/patcher.py
+-rw-r--r--   0 franz      (501) staff       (20)     5923 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/utils/profiler.py
+drwxr-xr-x   0 franz      (501) staff       (20)        0 2023-06-23 16:27:27.778864 dataquality-0.9.0a0/dataquality/utils/semantic_segmentation/
+-rw-r--r--   0 franz      (501) staff       (20)        0 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/utils/semantic_segmentation/__init__.py
+-rw-r--r--   0 franz      (501) staff       (20)       43 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/utils/semantic_segmentation/constants.py
+-rw-r--r--   0 franz      (501) staff       (20)    10033 2023-06-23 16:26:44.000000 dataquality-0.9.0a0/dataquality/utils/semantic_segmentation/errors.py
+-rw-r--r--   0 franz      (501) staff       (20)    11898 2023-06-21 17:17:50.000000 dataquality-0.9.0a0/dataquality/utils/semantic_segmentation/lm.py
+-rw-r--r--   0 franz      (501) staff       (20)    10144 2023-06-23 16:26:44.000000 dataquality-0.9.0a0/dataquality/utils/semantic_segmentation/metrics.py
+-rw-r--r--   0 franz      (501) staff       (20)     5309 2023-06-23 16:26:44.000000 dataquality-0.9.0a0/dataquality/utils/semantic_segmentation/polygons.py
+-rw-r--r--   0 franz      (501) staff       (20)     1914 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/utils/semantic_segmentation/utils.py
+-rw-r--r--   0 franz      (501) staff       (20)    15187 2023-06-21 17:17:50.000000 dataquality-0.9.0a0/dataquality/utils/setfit.py
+-rw-r--r--   0 franz      (501) staff       (20)      260 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/utils/tf.py
+-rw-r--r--   0 franz      (501) staff       (20)     1987 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/utils/thread_pool.py
+-rw-r--r--   0 franz      (501) staff       (20)    24980 2023-06-23 16:26:44.000000 dataquality-0.9.0a0/dataquality/utils/torch.py
+-rw-r--r--   0 franz      (501) staff       (20)     5087 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/utils/transformers.py
+-rw-r--r--   0 franz      (501) staff       (20)    12825 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/utils/ultralytics.py
+-rw-r--r--   0 franz      (501) staff       (20)     5597 2023-06-21 17:17:50.000000 dataquality-0.9.0a0/dataquality/utils/upload.py
+-rw-r--r--   0 franz      (501) staff       (20)    10670 2023-06-21 17:17:50.000000 dataquality-0.9.0a0/dataquality/utils/vaex.py
+-rw-r--r--   0 franz      (501) staff       (20)     1087 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/dataquality/utils/version.py
+drwxr-xr-x   0 franz      (501) staff       (20)        0 2023-06-23 16:27:27.706319 dataquality-0.9.0a0/dataquality.egg-info/
+-rw-r--r--   0 franz      (501) staff       (20)     4939 2023-06-23 16:27:27.000000 dataquality-0.9.0a0/dataquality.egg-info/PKG-INFO
+-rw-r--r--   0 franz      (501) staff       (20)     5079 2023-06-23 16:27:27.000000 dataquality-0.9.0a0/dataquality.egg-info/SOURCES.txt
+-rw-r--r--   0 franz      (501) staff       (20)        1 2023-06-23 16:27:27.000000 dataquality-0.9.0a0/dataquality.egg-info/dependency_links.txt
+-rw-r--r--   0 franz      (501) staff       (20)       51 2023-06-23 16:27:27.000000 dataquality-0.9.0a0/dataquality.egg-info/entry_points.txt
+-rw-r--r--   0 franz      (501) staff       (20)     1293 2023-06-23 16:27:27.000000 dataquality-0.9.0a0/dataquality.egg-info/requires.txt
+-rw-r--r--   0 franz      (501) staff       (20)       18 2023-06-23 16:27:27.000000 dataquality-0.9.0a0/dataquality.egg-info/top_level.txt
+-rw-r--r--   0 franz      (501) staff       (20)     3847 2023-06-23 16:26:44.000000 dataquality-0.9.0a0/pyproject.toml
+-rw-r--r--   0 franz      (501) staff       (20)      293 2023-06-23 16:27:27.794154 dataquality-0.9.0a0/setup.cfg
+-rw-r--r--   0 franz      (501) staff       (20)       38 2023-06-21 17:17:50.000000 dataquality-0.9.0a0/setup.py
+drwxr-xr-x   0 franz      (501) staff       (20)        0 2023-06-23 16:27:27.781134 dataquality-0.9.0a0/tests/
+-rw-r--r--   0 franz      (501) staff       (20)    31396 2023-06-21 17:17:50.000000 dataquality-0.9.0a0/tests/test_dataquality.py
+-rw-r--r--   0 franz      (501) staff       (20)     1783 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/tests/test_telemetrics.py
+drwxr-xr-x   0 franz      (501) staff       (20)        0 2023-06-23 16:27:27.792454 dataquality-0.9.0a0/tests/test_utils/
+-rw-r--r--   0 franz      (501) staff       (20)        0 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/tests/test_utils/__init__.py
+-rw-r--r--   0 franz      (501) staff       (20)     6129 2023-06-21 17:17:50.000000 dataquality-0.9.0a0/tests/test_utils/data_utils.py
+-rw-r--r--   0 franz      (501) staff       (20)     1692 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/tests/test_utils/hf_datasets_mock.py
+-rw-r--r--   0 franz      (501) staff       (20)    11616 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/tests/test_utils/hf_integration_constants.py
+-rw-r--r--   0 franz      (501) staff       (20)     8122 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/tests/test_utils/hf_integration_constants_inference.py
+-rw-r--r--   0 franz      (501) staff       (20)     3695 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/tests/test_utils/lightning_model.py
+-rw-r--r--   0 franz      (501) staff       (20)     3017 2023-06-23 16:26:44.000000 dataquality-0.9.0a0/tests/test_utils/mock_data.py
+-rw-r--r--   0 franz      (501) staff       (20)     5594 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/tests/test_utils/mock_request.py
+-rw-r--r--   0 franz      (501) staff       (20)     2840 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/tests/test_utils/ner_constants.py
+-rw-r--r--   0 franz      (501) staff       (20)      863 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/tests/test_utils/pt_datasets_mock.py
+-rw-r--r--   0 franz      (501) staff       (20)     7910 2023-06-14 11:37:38.000000 dataquality-0.9.0a0/tests/test_utils/tc_constants.py
```

### Comparing `dataquality-0.8.9/LICENSE` & `dataquality-0.9.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.9/dataquality/__init__.py` & `dataquality-0.9.0a0/dataquality/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,142 +1,141 @@
-"dataquality"
+"""dataquality is a library for tracking and analyzing your machine learning models.
+:param model: The model to inspect, if a string, it will be assumed to be auto
+:param task: Task type for example "text_classification"
+:param project: Project name
+:param run: Run name
+:param train_data: Training data
+:param test_data: Optional test data
+:param val_data: Optional: validation data
+:param labels: The labels for the run
+:param framework: The framework to use, if provided it will be used instead of
+    inferring it from the model. For example, if you have a torch model, you
+    can pass framework="torch". If you have a torch model, you can pass
+    framework="torch"
+:param args: Additional arguments
+:param kwargs: Additional keyword arguments
+.. code-block:: python
+    import dataquality
+    with dataquality(
+        model,
+        "text_classification",
+        labels = ["neg", "pos"],
+        train_data = train_data
+    ):
+        model.fit(train_data)
+If you want to train without a model, you can use the auto framework:
+.. code-block:: python
+    import dataquality
+    with dataquality(labels = ["neg", "pos"],
+                     train_data = train_data):
+        dataquality.get_insights()
+"""
 
-__version__ = "v0.8.9"
 
-import os
+__version__ = "v0.9.0a0"
+
+import sys
+from typing import Any, List, Optional
 
 import dataquality.core._config
 import dataquality.integrations
 
 # We try/catch this in case the user installed dq inside of jupyter. You need to
 # restart the kernel after the install and we want to make that clear. This is because
-# of vaex: https://github.com/vaexio/vaex/pull/2226
 try:
     import dataquality.metrics
     from dataquality.analytics import Analytics
     from dataquality.clients.api import ApiClient
 except (FileNotFoundError, AttributeError):
     raise Exception(
         "It looks like you've installed dataquality from a notebook. "
         "Please restart the kernel before continuing"
     ) from None
+from dataquality.core import configure, set_console_url
 from dataquality.core._config import config
 from dataquality.core.auth import login, logout
 from dataquality.core.finish import finish, get_run_status, wait_for_run
 from dataquality.core.init import init
 from dataquality.core.log import (
     docs,
+    get_current_run_labels,
     get_data_logger,
     get_model_logger,
     log_data_sample,
     log_data_samples,
     log_dataset,
     log_image_dataset,
     log_model_outputs,
+    log_xgboost,
     set_epoch,
     set_epoch_and_split,
     set_labels_for_run,
     set_split,
     set_tagging_schema,
     set_tasks_for_run,
 )
 from dataquality.core.report import build_run_report, register_run_report
 from dataquality.dq_auto.auto import auto
+from dataquality.dq_auto.notebook import auto_notebook
+from dataquality.dq_start import DataQuality
 from dataquality.schemas.condition import (
     AggregateFunction,
     Condition,
     ConditionFilter,
     Operator,
 )
 from dataquality.utils.dq_logger import get_dq_log_file
 from dataquality.utils.helpers import (
-    check_noop,
     disable_galileo,
     disable_galileo_verbose,
     enable_galileo,
     enable_galileo_verbose,
 )
 
-
-@check_noop
-def configure(do_login: bool = True) -> None:
-    """[Not for cloud users] Update your active config with new information
-
-    You can use environment variables to set the config, or wait for prompts
-    Available environment variables to update:
-    * GALILEO_CONSOLE_URL
-    * GALILEO_USERNAME
-    * GALILEO_PASSWORD
-    """
-    a.log_function("dq/configure")
-
-    if "GALILEO_API_URL" in os.environ:
-        del os.environ["GALILEO_API_URL"]
-    updated_config = dataquality.core._config.reset_config(cloud=False)
-    for k, v in updated_config.dict().items():
-        config.__setattr__(k, v)
-    config.token = None
-    config.update_file_config()
-    if do_login:
-        login()
-
-
-@check_noop
-def set_console_url(console_url: str = None) -> None:
-    """For Enterprise users. Set the console URL to your Galileo Environment.
-
-    You can also set GALILEO_CONSOLE_URL before importing dataquality to bypass this
-
-    :param console_url: If set, that will be used. Otherwise, if an environment variable
-    GALILEO_CONSOLE_URL is set, that will be used. Otherwise, you will be prompted for
-    a url.
-    """
-    a.log_function("dq/set_console_url")
-    if console_url:
-        os.environ["GALILEO_CONSOLE_URL"] = console_url
-    configure(do_login=False)
-
-
 __all__ = [
     "__version__",
     "login",
     "logout",
     "init",
     "log_data_samples",
     "log_model_outputs",
     "config",
     "configure",
     "finish",
     "set_labels_for_run",
+    "get_current_run_labels",
     "get_data_logger",
     "get_model_logger",
     "set_tasks_for_run",
     "set_tagging_schema",
     "docs",
     "wait_for_run",
     "get_run_status",
     "set_epoch",
     "set_split",
     "set_epoch_and_split",
     "set_console_url",
     "log_data_sample",
     "log_dataset",
     "log_image_dataset",
+    "log_xgboost",
     "get_dq_log_file",
     "build_run_report",
     "register_run_report",
     "AggregateFunction",
     "Operator",
     "Condition",
     "ConditionFilter",
     "disable_galileo",
     "disable_galileo_verbose",
     "enable_galileo_verbose",
     "enable_galileo",
     "auto",
+    "DataQuality",
+    "auto_notebook",
 ]
 
 try:
     import resource
 
     resource.setrlimit(resource.RLIMIT_NOFILE, (65535, 65535))
 except (ImportError, ValueError):  # The users limit is higher than our max, which is OK
@@ -151,7 +150,49 @@
 #  To log initiate the Analytics class and pass in the gallileo ApiClient + dq.config
 #  a = Analytics(ApiClient, config)
 #  Once initialized you can start logging
 #  a.log_import("dataquality")
 #  a.log_method_call("dataquality.log_data_samples")
 a = Analytics(ApiClient, config)
 a.log_import("dataquality")
+
+
+class _DataQuality:
+    """This class is used to create a singleton instance of the DataQuality class.
+
+    This is done to allow the user to use the same syntax as the original dataquality
+    package. The original package had a singleton instance of the DataQuality class
+    that was created when the package was imported. This class is used to mimic that
+    behavior.
+    """
+
+    _instance: Optional[DataQuality] = None
+
+    def __init__(self) -> None:
+        self._instance = None
+
+    def __call__(self, *args: Any, **kwargs: Any) -> DataQuality:
+        """Return the singleton instance of the DataQuality class."""
+        if self._instance is None:
+            self._instance = DataQuality(*args, **kwargs)
+        return self._instance
+
+        # we want to add the __all__ to the module
+
+    def get_insights(self) -> None:
+        return
+
+    def __dir__(self) -> List[str]:
+        return __all__
+
+    def __getattr__(self, name: str) -> Any:
+        if name in __all__:
+            return globals()[name]
+        # We return the wanted import from the original dataquality package
+        else:
+            return getattr(dataquality, name)
+
+
+# Workaround by Guido van Rossum:
+# https://mail.python.org/pipermail/python-ideas/2012-May/014969.html
+# This allows us to use the same syntax as the original dataquality package
+sys.modules[__name__] = _DataQuality()  # type: ignore
```

### Comparing `dataquality-0.8.9/dataquality/analytics.py` & `dataquality-0.9.0a0/dataquality/analytics.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from typing import Any, Dict, Optional, Tuple, Type
 
 from pydantic import BaseModel
 
 from dataquality.clients.api import ApiClient
 from dataquality.core._config import Config
 from dataquality.utils.ampli import AmpliMetric
+from dataquality.utils.patcher import Borg
 from dataquality.utils.profiler import (
     _installed_modules,
     change_function,
     exception_from_error,
     get_device_info,
     parse_exception,
     parse_exception_ipython,
@@ -23,31 +24,22 @@
 class ProfileModel(BaseModel):
     """User profile"""
 
     packages: Optional[Dict[str, str]]
     uuid: Optional[str]
 
 
-class Borg:
-    # We use a borg pattern to share state across all instances of this class.
-    # Due to submitting some errors in a thread,
-    # we want to share the thread pool executor
-    _shared_state: Dict[str, Any] = {}
-
-    def __init__(self) -> None:
-        self.__dict__ = self._shared_state
-
-
 class Analytics(Borg):
     """Analytics is used to track errors and logs in the background"""
 
     _telemetrics_disabled: bool = True
 
     def __init__(self, ApiClient: Type[ApiClient], config: Config) -> None:
-        """To initialize the Analytics class you need to pass in an ApiClient and the dq config.
+        """To initialize the Analytics class you need
+        to pass in an ApiClient and the dq config.
         :param ApiClient: The ApiClient class
         :param config: The dq config
         """
         super().__init__()
 
         try:
             self._telemetrics_disabled = self._is_telemetrics_disabled(config)
@@ -123,15 +115,15 @@
 
     def ipython_exception_handler(
         self,
         shell: Any,
         etype: Type[BaseException],
         evalue: BaseException,
         tb: TracebackType,
-        tb_offset: Any = None,
+        tb_offset: Optional[Any] = None,
     ) -> None:
         """This function is used to handle exceptions in ipython."""
 
         # we hook into the traceback,
         # inbetween we log the exception
         # and then show the original traceback.
         # because recently the track_exception_ipython was failing
@@ -141,15 +133,18 @@
                 self.track_exception_ipython(
                     etype, evalue, tb, AmpliMetric.dq_general_exception
                 )
         except Exception:
             # TODO: create internal logging endpoint
             pass
         # We need to call the default ipython exception handler to raise the error
-        shell.showtraceback((etype, evalue, tb), tb_offset=tb_offset)
+        if tb_offset is None:
+            shell.showtraceback((etype, evalue, tb))
+        else:
+            shell.showtraceback((etype, evalue, tb), tb_offset=tb_offset)
 
     def track_exception_ipython(
         self,
         etype: Type[BaseException],
         evalue: BaseException,
         tb: TracebackType,
         scope: AmpliMetric = AmpliMetric.dq_general_exception,
```

### Comparing `dataquality-0.8.9/dataquality/clients/api.py` & `dataquality-0.9.0a0/dataquality/clients/api.py`

 * *Files 12% similar despite different names*

```diff
@@ -63,30 +63,40 @@
         except GalileoException:
             return False
 
     def make_request(
         self,
         request: RequestType,
         url: str,
-        body: Dict = None,
-        data: Dict = None,
-        params: Dict = None,
-        header: Dict = None,
+        body: Optional[Dict] = None,
+        data: Optional[Dict] = None,
+        params: Optional[Dict] = None,
+        header: Optional[Dict] = None,
         timeout: Union[int, None] = None,
+        files: Optional[Dict] = None,
+        return_response_without_validation: bool = False,
     ) -> Any:
         """Makes an HTTP request.
 
         This is the center point of all functions and the main entry/exit for the
         dataquality client to interact with the server.
         """
         self.__check_login()
         header = header or headers(config.token)
         res = RequestType.get_method(request.value)(
-            url, json=body, params=params, headers=header, data=data, timeout=timeout
+            url,
+            json=body,
+            params=params,
+            headers=header,
+            data=data,
+            timeout=timeout,
+            files=files,
         )
+        if return_response_without_validation:
+            return res
         self._validate_response(res)
         return res.json()
 
     def get_project(self, project_id: UUID4) -> Dict:
         return self.make_request(
             RequestType.GET,
             url=f"{config.api_url}/{Route.projects}/{project_id}",
@@ -134,14 +144,26 @@
         if not proj:
             raise GalileoException(f"No project with name {project_name}")
         url = f"{config.api_url}/{Route.projects}/{proj['id']}/{Route.runs}"
         params = {"run_name": run_name}
         runs = self.make_request(RequestType.GET, url=url, params=params)
         return runs[0] if runs else {}
 
+    def update_run_name(self, project_name: str, run_name: str, new_name: str) -> Dict:
+        project_id, run_id = self._get_project_run_id(project_name, run_name)
+        if not project_id:
+            raise GalileoException(f"No project with name {project_name}")
+        if not run_id:
+            raise GalileoException(f"No run with name {run_name}")
+
+        url = f"{config.api_url}/{Route.projects}/{project_id}/{Route.runs}/{run_id}"
+        data = {"name": new_name}
+        run = self.make_request(RequestType.PUT, url=url, body=data)
+        return run if run else {}
+
     def create_project(self, project_name: str, is_public: bool = True) -> Dict:
         """Creates a project given a name and returns the project information"""
         body = {"name": project_name, "is_public": is_public}
         return self.make_request(
             RequestType.POST, url=f"{config.api_url}/{Route.projects}", body=body
         )
 
@@ -255,36 +277,35 @@
             run = res["id"]
         else:
             project = config.current_project_id
             run = config.current_run_id
         return project, run
 
     def get_labels_for_run(
-        self, project_name: str = None, run_name: str = None, task: str = None
+        self,
+        project_name: Optional[str] = None,
+        run_name: Optional[str] = None,
+        task: Optional[str] = None,
     ) -> List[str]:
         """Gets the labels for a given run, else the currently initialized project/run
 
         If you do not provide a project and run name, the currently initialized
         project/run will be used. Otherwise you must provide both a project and run name
         If the run is a multi-label run, a task must be provided
         """
         project, run = self._get_project_run_id(
             project_name=project_name, run_name=run_name
         )
-        task_type = self.get_task_type(project, run)
-        if not task and task_type == TaskType.text_multi_label:
-            raise GalileoException("For multi-label runs, a task name must be provided")
-
         url = f"{config.api_url}/{Route.content_path(project, run)}/{Route.labels}"
         params = {"task": task} if task else None
         res = self.make_request(RequestType.GET, url=url, params=params)
         return res["labels"]
 
     def get_tasks_for_run(
-        self, project_name: str = None, run_name: str = None
+        self, project_name: Optional[str] = None, run_name: Optional[str] = None
     ) -> List[str]:
         """Gets the task names for a given multi-label run,
 
         If you do not provide a project and run name, the currently initialized
         project/run will be used. Otherwise you must provide both a project and run name
 
         This function is only valid for multi-label runs.
@@ -316,82 +337,25 @@
         url = f"{config.api_url}/{path}/{Route.edits}"
         body = edit.dict()
         params = {"inference_name": edit.inference_name}
         return self.make_request(RequestType.POST, url=url, body=body, params=params)
 
     def reprocess_run(
         self,
-        project_name: str = None,
-        run_name: str = None,
-        labels: Union[List, List[List]] = None,
+        project_name: Optional[str] = None,
+        run_name: Optional[str] = None,
+        labels: Optional[Union[List, List[List]]] = None,
+        xray: bool = False,
     ) -> Dict:
-        """Reinitiate a project/run that has already been finished
-
-        If a project and run name have been provided, that project/run will be
-        reinitiated, otherwise we trigger the currently initialized project/run.
-
-        This will clear out the current state in the server, and will recalculate
-        * DEP score
-        * UMAP Embeddings for visualization
-        * Smart features
-
-        :param project_name: If not set, will use the currently active project
-        :param run_name: If not set, will use the currently active run
-        :param labels: If set, will reprocess the run with these labels. If not set,
-        labels will be used from the previously processed run. These must match the
-        labels that were originally logged
-        """
-        project, run = self._get_project_run_id(project_name, run_name)
-        project_name = project_name or self.get_project(project)["name"]
-        run_name = run_name or self.get_project_run(project, run)["name"]
-        task_type = self.get_task_type(project, run)
-
-        # Multi-label has tasks and List[List] for labels
-        if task_type == TaskType.text_multi_label:
-            tasks = self.get_tasks_for_run(project_name, run_name)
-            if not labels:
-                labels = [
-                    self.get_labels_for_run(project_name, run_name, t) for t in tasks
-                ]
-        else:
-            tasks = []
-            if not labels:
-                try:
-                    labels = self.get_labels_for_run(project_name, run_name)
-                except GalileoException as e:
-                    if "No data found" in str(e):
-                        e = GalileoException(
-                            f"It seems no data is available for run "
-                            f"{project_name}/{run_name}"
-                        )
-                    raise e from None
-                # There were no labels available for this run
-                except KeyError:
-                    raise GalileoException(
-                        "It seems we cannot find the labels for this run. Please call "
-                        "api_client.reprocess_run again, passing in your labels to the "
-                        "'labels' keyword"
-                    ) from None
-
-        body = dict(
-            project_id=str(project),
-            run_id=str(run),
-            labels=labels,
-            tasks=tasks or None,
-            task_type=task_type,
-            xray=False,  # Don't recalculate XRay in process
+        """Removed. Please see dq.internal.reprocess_run"""
+        raise GalileoException(
+            "It seems you are trying to reprocess a run. Please call the following:\n\n"
+            "from dataquality.internal import reprocess_run\n\n"
+            f"reprocess_run('{project_name}', '{run_name}')"
         )
-        res = self.make_request(
-            RequestType.POST, url=f"{config.api_url}/{Route.jobs}", body=body
-        )
-        print(
-            f"Job {res['job_name']} successfully resubmitted. New results will be "
-            f"available soon at {res['link']}"
-        )
-        return res
 
     def get_slice_by_name(self, project_name: str, slice_name: str) -> Dict:
         """Get a slice by name"""
         proj = self.get_project_by_name(project_name)
         url = f"{config.api_url}/{Route.content_path(proj['id'])}/{Route.slices}"
         params = {"slice_name": slice_name}
         slices = self.make_request(RequestType.GET, url=url, params=params)
@@ -417,15 +381,15 @@
         :param project_name:
         :param run_name:
         :param split:
         """
         project, run = self._get_project_run_id(project_name, run_name)
         split = conform_split(split)
         url = f"{config.api_url}/{Route.content_path(project, run, split)}/meta/columns"
-        return self.make_request(RequestType.GET, url)
+        return self.make_request(RequestType.POST, url, body={})
 
     def get_task_type(self, project_id: UUID4, run_id: UUID4) -> TaskType:
         return TaskType.get_mapping(
             self.get_project_run(project_id, run_id)["task_type"]
         )
 
     def export_run(
@@ -436,15 +400,15 @@
         file_name: str,
         inference_name: str = "",
         slice_name: Optional[str] = None,
         include_cols: Optional[List[str]] = None,
         col_mapping: Optional[Dict[str, str]] = None,
         hf_format: bool = False,
         tagging_schema: Optional[TaggingSchema] = None,
-        filter_params: Dict = None,
+        filter_params: Optional[Dict] = None,
     ) -> None:
         """Export a project/run to disk as a file
 
         :param project_name: The project name
         :param run_name: The run name
         :param split: The split to export on
         :param file_name: The file name. Must end in a supported FileType
@@ -526,15 +490,15 @@
         job_url = f"{config.api_url}/{Route.content_path(pid, rid)}/{Route.latest_job}"
         job = self.make_request(RequestType.GET, job_url)
         return job or {}
 
     def wait_for_run(
         self, project_name: Optional[str] = None, run_name: Optional[str] = None
     ) -> None:
-        print("Waiting for job...")
+        print("Waiting for job (you can safely close this window)...")
         last_progress_message = ""
         while True:
             job = self.get_run_status(project_name=project_name, run_name=run_name)
             if job.get("status") == "completed":
                 print(f"Done! Job finished with status {job.get('status')}")
                 return
             elif job.get("status") == "failed":
@@ -556,15 +520,19 @@
             else:
                 raise GalileoException(
                     f"It seems there was an issue with your job. Received "
                     f"an unexpected status {job.get('status')}"
                 )
 
     def get_presigned_url(
-        self, project_id: str, method: str, bucket_name: str, object_name: str
+        self,
+        method: str,
+        bucket_name: str,
+        object_name: str,
+        project_id: str,
     ) -> str:
         response = self.make_request(
             request=RequestType.GET,
             url=f"{config.api_url}/{Route.presigned_url}",
             params={
                 "api_url": config.api_url,
                 "bucket_name": bucket_name,
@@ -576,17 +544,17 @@
         return response["url"]
 
     def get_run_summary(
         self,
         project_name: str,
         run_name: str,
         split: str,
-        task: str = None,
-        inference_name: str = None,
-        filter_params: Dict = None,
+        task: Optional[str] = None,
+        inference_name: Optional[str] = None,
+        filter_params: Optional[Dict] = None,
     ) -> Dict:
         """Gets overall run summary, or summary of a filtered subset.
 
         Use filter_params to apply arbitrary filters on the dataframe, based on the
         filter schema:
         https://api.dev.rungalileo.io/redoc#tag/insights
         """
@@ -605,18 +573,18 @@
         return self.make_request(RequestType.POST, url, body=body, params=params)
 
     def get_run_metrics(
         self,
         project_name: str,
         run_name: str,
         split: str,
-        task: str = None,
-        inference_name: str = None,
+        task: Optional[str] = None,
+        inference_name: Optional[str] = None,
         category: str = "gold",
-        filter_params: Dict = None,
+        filter_params: Optional[Dict] = None,
     ) -> Dict[str, List]:
         project, run = self._get_project_run_id(project_name, run_name)
         split = conform_split(split)
 
         all_meta = self.get_metadata_columns(project_name, run_name, split)
         categorical_meta = [i["name"] for i in all_meta["meta"] if i["is_categorical"]]
         avl_cols = categorical_meta + ["gold", "pred"]
@@ -634,18 +602,18 @@
         return self.make_request(RequestType.POST, url, body=body, params=params)
 
     def get_column_distribution(
         self,
         project_name: str,
         run_name: str,
         split: str,
-        task: str = None,
-        inference_name: str = None,
+        task: Optional[str] = None,
+        inference_name: Optional[str] = None,
         column: str = "data_error_potential",
-        filter_params: Dict = None,
+        filter_params: Optional[Dict] = None,
     ) -> Dict[str, List]:
         project, run = self._get_project_run_id(project_name, run_name)
         split = conform_split(split)
 
         all_meta = self.get_metadata_columns(project_name, run_name, split)
         continuous_meta = [i["name"] for i in all_meta["meta"] if i["is_continuous"]]
         avl_cols = continuous_meta + ["data_error_potential"]
@@ -659,26 +627,65 @@
         url = f"{config.api_url}/{path}/{Route.distribution}"
         params = {"col": column}
         if inference_name:
             params["inference_name"] = inference_name
         body = {"task": task, "filter_params": filter_params or {}}
         return self.make_request(RequestType.POST, url, body=body, params=params)
 
-    def get_xray_cards(
-        self, project_name: str, run_name: str, split: str, inference_name: str = None
+    def get_alerts(
+        self,
+        project_name: str,
+        run_name: str,
+        split: str,
+        inference_name: Optional[str] = None,
     ) -> List[Dict[str, str]]:
-        """Queries API for xray cards for a run/split"""
+        """Queries API for alerts for a run/split"""
         project, run = self._get_project_run_id(project_name, run_name)
         path = Route.content_path(project, run, split)
-        url = f"{config.api_url}/{path}/{Route.xray}"
+        url = f"{config.api_url}/{path}/{Route.alerts}"
         params = {"inference_name": inference_name} if inference_name else None
         return self.make_request(RequestType.GET, url, params=params)
 
+    def delete_alerts_for_split(
+        self, project_id: UUID4, run_id: UUID4, split: str
+    ) -> None:
+        path = Route.content_path(project_id, run_id, split)
+        url = f"{config.api_url}/{path}/{Route.alerts}"
+        alerts = []
+        if split == "inference":
+            inference_names = self.get_inference_names(project_id, run_id)
+            for inf_name in inference_names["inference_names"]:
+                params = {"inference_name": inf_name}
+                res = self.make_request(RequestType.GET, url, params=params)
+                alerts.extend([alert["id"] for alert in res])
+        else:
+            res = self.make_request(RequestType.GET, url)
+            alerts.extend([alert["id"] for alert in res])
+        path = Route.content_path(project_id, run_id, split)
+        for alert_id in alerts:
+            url = f"{config.api_url}/{path}/{Route.alerts}/{alert_id}"
+            self.make_request(RequestType.DELETE, url)
+
+    def delete_alerts(
+        self,
+        project_name: str,
+        run_name: str,
+    ) -> None:
+        """Delete all alerts for a run"""
+        project_id, run_id = self._get_project_run_id(project_name, run_name)
+        for split in self.get_splits(project_id, run_id)["splits"]:
+            self.delete_alerts_for_split(project_id, run_id, split)
+        print(f"All alerts removed for run {project_name}/{run_name}")
+
     def get_edits(
-        self, project_name: str, run_name: str, split: str, inference_name: str = None
+        self,
+        project_name: str,
+        run_name: str,
+        split: str,
+        inference_name: Optional[str] = None,
     ) -> List:
         """Gets all edits for a run/split"""
         project, run = self._get_project_run_id(project_name, run_name)
         split = conform_split(split)
 
         url = (
             f"{config.api_url}/{Route.content_path(project, run, split)}/{Route.edits}"
@@ -688,15 +695,15 @@
 
     def export_edits(
         self,
         project_name: str,
         run_name: str,
         split: str,
         file_name: str,
-        inference_name: str = None,
+        inference_name: Optional[str] = None,
         include_cols: Optional[List[str]] = None,
         col_mapping: Optional[Dict[str, str]] = None,
         hf_format: bool = False,
         tagging_schema: Optional[TaggingSchema] = None,
     ) -> None:
         """Export the edits of a project/run/split to disk as a file
 
@@ -781,7 +788,56 @@
         return self.make_request(
             RequestType.GET,
             url=(
                 f"{config.api_url}/{Route.projects}/{project_id}/{Route.runs}/{run_id}/"
                 f"{Route.inference_names}"
             ),
         )
+
+    def set_metric_for_run(self, project_id: UUID4, run_id: UUID4, data: Dict) -> Dict:
+        return self.make_request(
+            RequestType.PUT,
+            url=(
+                f"{config.api_url}/{Route.projects}/{project_id}/{Route.runs}/{run_id}/"
+                f"{Route.metrics}"
+            ),
+            body=data,
+        )
+
+    def get_healthcheck_dq(self) -> Dict:
+        return self.make_request(
+            RequestType.GET, url=f"{config.api_url}/{Route.healthcheck_dq}"
+        )
+
+    def upload_file_for_project(
+        self,
+        project_id: str,
+        file_path: str,
+        export_format: str,
+        export_cols: List[str],
+        bucket: str,
+    ) -> Any:
+        url = f"{config.api_url}/{Route.projects}/{project_id}/{Route.upload_file}"
+        res = self.make_request(
+            return_response_without_validation=True,
+            request=RequestType.POST,
+            url=url,
+            files={
+                "file": (
+                    os.path.basename(file_path),
+                    open(file_path, "rb"),
+                    "application/octet-stream",
+                ),
+                "upload_metadata": (
+                    None,
+                    json.dumps(
+                        {
+                            "export_format": export_format,
+                            "export_cols": export_cols,
+                            "bucket": bucket,
+                        }
+                    ),
+                    "application/json",
+                ),
+            },
+        )
+        return res
```

### Comparing `dataquality-0.8.9/dataquality/core/_config.py` & `dataquality-0.9.0a0/dataquality/core/_config.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,14 +16,18 @@
 from dataquality.exceptions import GalileoException
 from dataquality.schemas.route import Route
 from dataquality.schemas.task_type import TaskType
 from dataquality.utils.helpers import galileo_disabled
 
 CLOUD_URL = "https://console.cloud.rungalileo.io"
 MINIMUM_API_VERSION = "0.4.0"
+GALILEO_DEFAULT_IMG_BUCKET_NAME = "galileo-images"
+GALILEO_DEFAULT_RUN_BUCKET_NAME = "galileo-project-runs"
+GALILEO_DEFAULT_RESULT_BUCKET_NAME = "galileo-project-runs-results"
+EXOSCALE_FQDN_SUFFIX = ".exo.io"
 
 
 class GalileoConfigVars(str, Enum):
     API_URL = "GALILEO_API_URL"
     CONSOLE_URL = "GALILEO_CONSOLE_URL"
 
     @staticmethod
@@ -39,36 +43,62 @@
         }
 
     @staticmethod
     def auto_init_vars_available() -> bool:
         return bool(os.getenv("GALILEO_API_URL"))
 
 
-class ConfigData(str, Enum):
-    DEFAULT_GALILEO_CONFIG_DIR = f"{os.environ.get('HOME', str(Path.home()))}/.galileo"
-    DEFAULT_GALILEO_CONFIG_FILE = f"{DEFAULT_GALILEO_CONFIG_DIR}/config.json"
+class ConfigData:
+    def __init__(
+        self,
+        default_galileo_config_dir: Optional[str] = None,
+        default_galileo_config_file: Optional[str] = None,
+    ) -> None:
+        self.DEFAULT_GALILEO_CONFIG_DIR = default_galileo_config_dir or (
+            f"{os.environ.get('HOME', str(Path.home()))}/.galileo"
+        )
+        self.DEFAULT_GALILEO_CONFIG_FILE = (
+            default_galileo_config_file
+            or f"{self.DEFAULT_GALILEO_CONFIG_DIR}/config.json"
+        )
+        if os.environ.get("PYTEST_XDIST_WORKER_COUNT"):
+            pid = os.getpid()
+            self.DEFAULT_GALILEO_CONFIG_DIR += f"-{pid}"
+            self.DEFAULT_GALILEO_CONFIG_FILE = (
+                f"{self.DEFAULT_GALILEO_CONFIG_DIR}/config.json"
+            )
+
+
+config_data = ConfigData()
 
 
 class Config(BaseModel):
     api_url: str
     token: Optional[str] = None
     current_user: Optional[str] = None
     current_project_id: Optional[UUID4] = None
     current_run_id: Optional[UUID4] = None
+    current_project_name: Optional[str] = None
+    current_run_name: Optional[str] = None
     task_type: Optional[TaskType] = None
+    root_bucket_name: str = GALILEO_DEFAULT_RUN_BUCKET_NAME
+    results_bucket_name: str = GALILEO_DEFAULT_RESULT_BUCKET_NAME
+    images_bucket_name: str = GALILEO_DEFAULT_IMG_BUCKET_NAME
+    minio_fqdn: Optional[str] = None
+    is_exoscale_cluster: bool = False
 
     class Config:
         validate_assignment = True
         arbitrary_types_allowed = True
         underscore_attrs_are_private = True
 
     def update_file_config(self) -> None:
         config_json = self.dict()
 
-        with open(ConfigData.DEFAULT_GALILEO_CONFIG_FILE.value, "w+") as f:
+        with open(config_data.DEFAULT_GALILEO_CONFIG_FILE, "w+") as f:
             f.write(json.dumps(config_json, default=str))
 
     @validator("api_url", pre=True, always=True, allow_reuse=True)
     def add_scheme(cls, v: str) -> str:
         if not v.startswith("http"):
             # api url needs the scheme
             v = f"http://{v}"
@@ -110,15 +140,15 @@
         raise GalileoException(err_detail.format(err=str(e))) from None
 
 
 def _check_dq_version() -> None:
     """Check that user is running valid version of DQ client
     Pings backend to check minimum DQ version requirements.
     """
-    r = requests.get(f"{config.api_url}/{Route.healthcheck}/dq")
+    r = requests.get(f"{config.api_url}/{Route.healthcheck_dq}")
     if not r.ok:
         if r.status_code == 404:
             # We don't want to raise error if api doesn't have dq healthcheck yet
             return
         raise GalileoException(r.text) from None
 
     dq_version_parsed = version.parse(dq_version)
@@ -169,18 +199,18 @@
             set_platform_urls(console_url_str=console_url)
 
 
 def set_config(cloud: bool = True) -> Config:
     if galileo_disabled():
         return Config(api_url="")
     _check_console_url()
-    if not os.path.isdir(ConfigData.DEFAULT_GALILEO_CONFIG_DIR.value):
-        os.makedirs(ConfigData.DEFAULT_GALILEO_CONFIG_DIR.value, exist_ok=True)
-    if os.path.exists(ConfigData.DEFAULT_GALILEO_CONFIG_FILE.value):
-        with open(ConfigData.DEFAULT_GALILEO_CONFIG_FILE.value) as f:
+    if not os.path.isdir(config_data.DEFAULT_GALILEO_CONFIG_DIR):
+        os.makedirs(config_data.DEFAULT_GALILEO_CONFIG_DIR, exist_ok=True)
+    if os.path.exists(config_data.DEFAULT_GALILEO_CONFIG_FILE):
+        with open(config_data.DEFAULT_GALILEO_CONFIG_FILE) as f:
             try:
                 config_vars: Dict[str, str] = json.load(f)
             # If there's an issue reading the config file for any reason, quit and
             # start fresh
             except Exception as e:
                 warnings.warn(
                     f"We had an issue reading your config file ({type(e)}). "
@@ -212,13 +242,13 @@
         config = Config(**galileo_vars)
     config.update_file_config()
     return config
 
 
 def reset_config(cloud: bool = True) -> Config:
     """Wipe the config file and reconfigure"""
-    if os.path.isfile(ConfigData.DEFAULT_GALILEO_CONFIG_FILE.value):
-        os.remove(ConfigData.DEFAULT_GALILEO_CONFIG_FILE.value)
+    if os.path.isfile(config_data.DEFAULT_GALILEO_CONFIG_FILE):
+        os.remove(config_data.DEFAULT_GALILEO_CONFIG_FILE)
     return set_config(cloud)
 
 
 config = set_config()
```

### Comparing `dataquality-0.8.9/dataquality/core/auth.py` & `dataquality-0.9.0a0/dataquality/core/auth.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.9/dataquality/core/finish.py` & `dataquality-0.9.0a0/dataquality/core/finish.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,64 +8,70 @@
 from dataquality.clients.api import ApiClient
 from dataquality.core._config import config
 from dataquality.core.report import build_run_report
 from dataquality.schemas import RequestType, Route
 from dataquality.schemas.job import JobName
 from dataquality.schemas.task_type import TaskType
 from dataquality.utils.dq_logger import DQ_LOG_FILE_HOME, upload_dq_log_file
-from dataquality.utils.helpers import check_noop, open_console_url
+from dataquality.utils.helpers import check_noop, gpu_available, open_console_url
 from dataquality.utils.thread_pool import ThreadPoolManager
 from dataquality.utils.version import _version_check
 
 api_client = ApiClient()
 a = Analytics(ApiClient, config)  # type: ignore
 
 
 @check_noop
 def finish(
     last_epoch: Optional[int] = None,
     wait: bool = True,
-    create_data_embs: bool = False,
+    create_data_embs: Optional[bool] = None,
 ) -> str:
     """
     Finishes the current run and invokes a job
 
     :param last_epoch: If set, only epochs up to this value will be uploaded/processed
         This is inclusive, so setting last_epoch to 5 would upload epochs 0,1,2,3,4,5
     :param wait: If true, after uploading the data, this will wait for the
         run to be processed by the Galileo server. If false, you can manually wait
         for the run by calling `dq.wait_for_run()` Default True
     :param create_data_embs: If True, an off-the-shelf transformer will run on the raw
         text input to generate data-level embeddings. These will be available in the
         `data view` tab of the Galileo console. You can also access these embeddings
-        via dq.metrics.get_data_embeddings()
+        via dq.metrics.get_data_embeddings(). Default True if a GPU is
+        available, else default False.
     """
     a.log_function("dq/finish")
+    if create_data_embs is None:
+        create_data_embs = gpu_available()
     ThreadPoolManager.wait_for_threads()
     assert config.current_project_id, "You must have an active project to call finish"
     assert config.current_run_id, "You must have an active run to call finish"
     assert config.task_type, "You must have a task type to call finish"
     data_logger = dataquality.get_data_logger()
     data_logger.validate_labels()
 
     _version_check()
 
     if data_logger.non_inference_logged():
         _reset_run(config.current_project_id, config.current_run_id, config.task_type)
 
+    # Certain tasks require extra finish logic
+    data_logger.logger_config.finish()
+
     data_logger.upload(last_epoch, create_data_embs=create_data_embs)
     upload_dq_log_file()
-
     body = dict(
         project_id=str(config.current_project_id),
         run_id=str(config.current_run_id),
         labels=data_logger.logger_config.labels,
         task_type=config.task_type.value,
         tasks=data_logger.logger_config.tasks,
         ner_labels=data_logger.logger_config.ner_labels,
+        feature_names=data_logger.logger_config.feature_names,
     )
     if data_logger.logger_config.inference_logged:
         body.update(
             job_name=JobName.inference,
             non_inference_logged=data_logger.non_inference_logged(),
         )
     res = api_client.make_request(
@@ -89,16 +95,20 @@
             run_id=config.current_run_id,
             link=res["link"],
         )
     elif wait:
         wait_for_run()
         open_console_url(res["link"])
 
-    # Reset the environment
+    # Reset the data logger
     data_logger._cleanup()
+
+    # Reset the model logger
+    dataquality.get_model_logger()._cleanup()
+
     return res.get("link") or ""
 
 
 @check_noop
 def wait_for_run(
     project_name: Optional[str] = None, run_name: Optional[str] = None
 ) -> None:
```

### Comparing `dataquality-0.8.9/dataquality/core/log.py` & `dataquality-0.9.0a0/dataquality/integrations/torch.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,403 +1,332 @@
-from typing import Any, Dict, List, Optional, Type, Union
-
-import numpy as np
-import pandas as pd
+import warnings
+from typing import Any, Callable, Dict, List, Optional, Union
+from warnings import warn
+
+from torch import Tensor
+from torch.nn import Module
+from torch.utils.data import DataLoader
+from torch.utils.data.sampler import SequentialSampler
+from transformers.modeling_outputs import TokenClassifierOutput
 
+import dataquality as dq
 from dataquality.analytics import Analytics
 from dataquality.clients.api import ApiClient
-from dataquality.core._config import config
+from dataquality.core.log import get_data_logger
 from dataquality.exceptions import GalileoException
-from dataquality.loggers.data_logger import BaseGalileoDataLogger
-from dataquality.loggers.data_logger.base_data_logger import ITER_CHUNK_SIZE, DataSet
-from dataquality.loggers.data_logger.image_classification import (
-    ImageClassificationDataLogger,
-)
-from dataquality.loggers.logger_config.text_multi_label import (
-    text_multi_label_logger_config,
-)
-from dataquality.loggers.model_logger import BaseGalileoModelLogger
-from dataquality.schemas.ner import TaggingSchema
-from dataquality.schemas.split import Split
 from dataquality.schemas.task_type import TaskType
-from dataquality.utils.helpers import check_noop
-
-DEFAULT_RANDOM_EMB_DIM = 2
-a = Analytics(ApiClient, config)  # type: ignore
-
-
-@check_noop
-def log_data_samples(
-    *,
-    texts: List[str],
-    ids: List[int],
-    meta: Dict[str, List[Union[str, float, int]]] = None,
-    **kwargs: Any,
-) -> None:
-    """Logs a batch of input samples for model training/test/validation/inference.
+from dataquality.schemas.torch import DimensionSlice, InputDim, Layer
+from dataquality.utils.helpers import map_indices_to_ids
+from dataquality.utils.patcher import Cleanup, RefManager
+from dataquality.utils.torch import (
+    ModelHookManager,
+    PatchDataloadersGlobally,
+    PatchSingleDataloaderIterator,
+    TorchBaseInstance,
+    TorchHelper,
+    remove_all_forward_hooks,
+    unpatch,
+)
 
-    Fields are expected as lists of their content. Field names are in the plural of
-    `log_input_sample` (text -> texts)
-    The expected arguments come from the task_type being used: See dq.docs() for details
+a = Analytics(ApiClient, dq.config)  # type: ignore
+a.log_import("torch")
 
-    ex (text classification):
-    .. code-block:: python
 
-        all_labels = ["A", "B", "C"]
-        dq.set_labels_for_run(labels = all_labels)
-
-        texts: List[str] = [
-            "Text sample 1",
-            "Text sample 2",
-            "Text sample 3",
-            "Text sample 4"
-        ]
-
-        labels: List[str] = ["B", "C", "A", "A"]
-
-        meta = {
-            "sample_importance": ["high", "low", "low", "medium"]
-            "quality_ranking": [9.7, 2.4, 5.5, 1.2]
-        }
-
-        ids: List[int] = [0, 1, 2, 3]
-        split = "training"
-
-        dq.log_data_samples(texts=texts, labels=labels, ids=ids, meta=meta split=split)
-
-    :param texts: List[str] the input samples to your model
-    :param ids: List[int | str] the ids per sample
-    :param split: Optional[str] the split for this data. Can also be set via
-        dq.set_split
-    :param meta: Dict[str, List[str | int | float]]. Log additional metadata fields to
-    each sample. The name of the field is the key of the dictionary, and the values are
-    a list that correspond in length and order to the text samples.
-    :param kwargs: See dq.docs() for details on other task specific parameters
+class TorchLogger(TorchBaseInstance):
     """
-    assert all(
-        [config.task_type, config.current_project_id, config.current_run_id]
-    ), "You must call dataquality.init before logging data"
-    data_logger = get_data_logger()
-    data_logger.log_data_samples(texts=texts, ids=ids, meta=meta, **kwargs)
-
-
-@check_noop
-def log_data_sample(*, text: str, id: int, **kwargs: Any) -> None:
-    """Log a single input example to disk
-
-    Fields are expected singular elements. Field names are in the singular of
-    `log_input_samples` (texts -> text)
-    The expected arguments come from the task_type being used: See dq.docs() for details
-
-    :param text: List[str] the input samples to your model
-    :param id: List[int | str] the ids per sample
-    :param split: Optional[str] the split for this data. Can also be set via
-        dq.set_split
-    :param kwargs: See dq.docs() for details on other task specific parameters
+    [`TorchLogger`] that sends the logs to [Galileo](https://www.rungalileo.io/)
+    for each training training step.
     """
-    assert all(
-        [config.task_type, config.current_project_id, config.current_run_id]
-    ), "You must call dataquality.init before logging data"
-    data_logger = get_data_logger()
-    # For logging a single sample, we don't want a progress bar because it will be
-    # nearly instant, and it's likely that the user will call this many times which
-    # would flood the output.
-    # We don't need to reset log_export_progress because this class instance is
-    # ephemeral
-    data_logger.log_export_progress = False
-    data_logger.log_data_sample(text=text, id=id, **kwargs)
-
-
-@check_noop
-def log_image_dataset(
-    dataset: DataSet,
-    imgs_dir: str,
-    *,
-    imgs_location_colname: Optional[str] = "relpath",
-    batch_size: int = ITER_CHUNK_SIZE,
-    id: Union[str, int] = "id",
-    label: Union[str, int] = "label",
-    split: Optional[Split] = None,
-    meta: Optional[List[Union[str, int]]] = None,
-    **kwargs: Any,
-) -> None:
-    assert isinstance(
-        dataset, pd.DataFrame
-    ), "dataset must be a pandas DataFrame"  # TODO: add support for other data types
-    a.log_function("dq/log_image_dataset")
-    assert all(
-        [config.task_type, config.current_project_id, config.current_run_id]
-    ), "You must call dataquality.init before logging data"
-    data_logger = get_data_logger()
-    assert isinstance(data_logger, ImageClassificationDataLogger), (
-        "This method is only supported for image tasks. "
-        "Please use dq.log_samples for text tasks."
-    )
-    data_logger.log_image_dataset(
-        dataset=dataset,
-        imgs_dir=imgs_dir,
-        imgs_location_colname=imgs_location_colname,
-        batch_size=batch_size,
-        id=id,
-        label=label,
-        split=split,
-        meta=meta,
-    )
 
-
-@check_noop
-def log_dataset(
-    dataset: DataSet,
-    *,
-    batch_size: int = ITER_CHUNK_SIZE,
-    text: Union[str, int] = "text",
-    id: Union[str, int] = "id",
-    split: Optional[Split] = None,
-    meta: Optional[List[Union[str, int]]] = None,
-    **kwargs: Any,
-) -> None:
-    """Log an iterable or other dataset to disk. Useful for logging memory mapped files
-
-    Dataset provided must be an iterable that can be traversed row by row, and for each
-    row, the fields can be indexed into either via string keys or int indexes. Pandas
-    and Vaex dataframes are also allowed, as well as HuggingFace Datasets
-
-    valid examples:
-        d = [
-            {"my_text": "sample1", "my_labels": "A", "my_id": 1, "sample_quality": 5.3},
-            {"my_text": "sample2", "my_labels": "A", "my_id": 2, "sample_quality": 9.1},
-            {"my_text": "sample3", "my_labels": "B", "my_id": 3, "sample_quality": 2.7},
-        ]
-        dq.log_dataset(
-            d, text="my_text", id="my_id", label="my_labels", meta=["sample_quality"]
+    embedding_dim: Optional[DimensionSlice]
+    logits_dim: Optional[DimensionSlice]
+    model: Module
+
+    def __init__(
+        self,
+        model: Module,
+        last_hidden_state_layer: Optional[Layer] = None,
+        embedding_dim: Optional[Union[str, DimensionSlice]] = None,
+        logits_dim: Optional[Union[str, DimensionSlice]] = None,
+        classifier_layer: Optional[Layer] = None,
+        embedding_fn: Optional[Callable] = None,
+        logits_fn: Optional[Callable] = None,
+        helper_data: Optional[Dict[str, Any]] = None,
+        task: Union[TaskType, None] = TaskType.text_classification,
+    ):
+        task_type = task or dq.config.task_type
+        assert task_type is not None, GalileoException(
+            "Dataquality task cannot be None."
+            "Setup with dq.init(task_type='text_classification')"
         )
-
-        Logging a pandas dataframe, df:
-              text label  id  sample_quality
-        0  sample1     A   1             5.3
-        1  sample2     A   2             9.1
-        2  sample3     B   3             2.7
-        # We don't need to set text id or label because it matches the default
-        dq.log_dataset(d, meta=["sample_quality"])
-
-        Logging and iterable of tuples:
-        d = [
-            ("sample1", "A", "ID1"),
-            ("sample2", "A", "ID2"),
-            ("sample3", "B", "ID3"),
-        ]
-        dq.log_dataset(d, text=0, id=2, label=1)
-
-    Invalid example:
-        d = {
-            "my_text": ["sample1", "sample2", "sample3"],
-            "my_labels": ["A", "A", "B"],
-            "my_id": [1, 2, 3],
-            "sample_quality": [5.3, 9.1, 2.7]
-        }
-
-    In the invalid case, use `dq.log_data_samples`:
-        meta = {"sample_quality": d["sample_quality"]}
-        dq.log_data_samples(
-            texts=d["my_text"], labels=d["my_labels"], ids=d["my_ids"], meta=meta
+        self.task = task_type
+        self.model = model
+        self.last_hidden_state_layer = last_hidden_state_layer
+        self.classifier_layer = classifier_layer
+        self.embedding_fn = embedding_fn
+        self.logits_fn = logits_fn
+
+        self._init_dimension(embedding_dim, logits_dim)
+        self.hook_manager = ModelHookManager()
+        self._attach_hooks_to_model(model, classifier_layer, last_hidden_state_layer)
+        if helper_data is None:
+            helper_data = {}
+        helper_data["torch_helper"] = TorchHelper(model, self.hook_manager)
+        self.torch_helper_data = helper_data["torch_helper"]
+        self._init_helper_data(self.hook_manager, self.model)
+        self.logger_config = dq.get_data_logger().logger_config
+
+    def _init_helper_data(self, hm: ModelHookManager, model: Module) -> None:
+        """
+        Initialize the helper data with ids from the dataloader indices,
+        patches for applied monkey patched functions and the hook manager.
+        :param hm: Hook manager
+        """
+        self.torch_helper_data.clear()
+        self.torch_helper_data = TorchHelper(model, hm)
+
+    def _attach_hooks_to_model(
+        self, model: Module, classifier_layer: Layer, last_hidden_state_layer: Layer
+    ) -> None:
+        """
+        Method to attach hooks to the model by using the hook manager
+        :param model: Model
+        :param model: pytorch model layer to attach hooks to
+        """
+        try:
+            self.hook_manager.attach_classifier_hook(
+                model, self._dq_classifier_hook_with_step_end, classifier_layer
+            )
+        except Exception as e:
+            warn(
+                "Could not attach function to model layer. Error:"
+                f" {e}. Please check that the classifier layer name:"
+                f" {classifier_layer} exists in the model. Common layers"
+                " to extract logits and the last hidden state are 'classifier'"
+                "and 'fc'. To fix this, pass the correct layer name to the "
+                "'classifier_layer' parameter in the 'watch' function. "
+                "For example: 'watch(model, classifier_layer='fc')'."
+                "You can view the model layers by using the 'model.named_children'"
+                "function or by printing the model."
+            )
+            self.hook_manager.attach_hooks_to_model(
+                model, self._dq_embedding_hook, last_hidden_state_layer
+            )
+            self.hook_manager.attach_hook(model, self._dq_logit_hook_with_step_end)
+
+    def _dq_classifier_hook_with_step_end(
+        self,
+        model: Module,
+        model_input: Tensor,
+        model_output: Union[TokenClassifierOutput, Tensor],
+    ) -> None:
+        """
+        Hook to extract the logits, embeddings from the model.
+        :param model: Model pytorch model
+        :param model_input: Model input
+        :param model_output: Model output
+        """
+        self._classifier_hook(model, model_input, model_output)
+        self._on_step_end()
+
+    def _dq_logit_hook_with_step_end(
+        self,
+        model: Module,
+        model_input: Tensor,
+        model_output: Union[TokenClassifierOutput, Tensor],
+    ) -> None:
+        """
+        Hook to extract the logits from the model.
+        :param model: Model pytorch model
+        :param model_input: Model input
+        :param model_output: Model output
+        """
+        self._dq_logit_hook(model, model_input, model_output)
+        self._on_step_end()
+
+    def _on_step_end(self) -> None:
+        """
+        Log the embeddings, ids and logits.
+        """
+        # We save the embeddings and logits in a dict called model_outputs
+        # in the helper data. This is because the embeddings and logits are
+        # extracted in the hooks and we need to log them in the on_step_end
+        # method.
+        model_outputs_store = self.torch_helper_data.model_outputs_store
+        # Workaround for multiprocessing
+        if model_outputs_store.get("ids") is None and len(
+            self.torch_helper_data.dl_next_idx_ids
+        ):
+            model_outputs_store["ids"] = self.torch_helper_data.dl_next_idx_ids.pop(0)
+
+        # Log only if embedding exists
+        assert model_outputs_store.get("embs") is not None, GalileoException(
+            "Embedding passed to the logger can not be logged"
         )
-
-    Keyword arguments are specific to the task type. See dq.docs() for details
-
-    :param dataset: The iterable or dataframe to log
-    :batch_size: The number of data samples to log at a time. Useful when logging a
-    memory mapped dataset. A larger batch_size will result in faster logging at the
-    expense of more memory usage. Default 100,000
-    :param text: str | int The column, key, or int index for text data. Default "text"
-    :param id: str | int The column, key, or int index for id data. Default "id"
-    :param split: Optional[str] the split for this data. Can also be set via
-        dq.set_split
-    :param meta: List[str | int] Additional keys/columns to your input data to be
-        logged as metadata. Consider a pandas dataframe, this would be the list of
-        columns corresponding to each metadata field to log
-    :param kwargs: See help(dq.get_data_logger().log_dataset) for more details here
-    or dq.docs() for more general task details
-    """
-    a.log_function("dq/log_dataset")
-    assert all(
-        [config.task_type, config.current_project_id, config.current_run_id]
-    ), "You must call dataquality.init before logging data"
-    data_logger = get_data_logger()
-    data_logger.log_dataset(
-        dataset,
-        batch_size=batch_size,
-        text=text,
-        id=id,
-        split=split,
-        meta=meta,
-        **kwargs,
-    )
+        assert model_outputs_store.get("logits") is not None, GalileoException(
+            "Logits passed to the logger can not be logged"
+        )
+        assert model_outputs_store.get("ids") is not None, GalileoException(
+            "id column missing in dataset (needed to map rows to the indices/ids)"
+        )
+        # Convert the indices to ids
+        cur_split = self.logger_config.cur_split.lower()  # type: ignore
+        model_outputs_store["ids"] = map_indices_to_ids(
+            self.logger_config.idx_to_id_map[cur_split], model_outputs_store["ids"]
+        )
+        dq.log_model_outputs(**model_outputs_store)
+        model_outputs_store.clear()
 
 
-@check_noop
-def log_model_outputs(
-    *,
-    embs: Optional[Union[List, np.ndarray]],
-    ids: Union[List, np.ndarray],
-    split: Optional[Split] = None,
-    epoch: Optional[int] = None,
-    logits: Union[List, np.ndarray] = None,
-    probs: Union[List, np.ndarray] = None,
-    inference_name: str = None,
-    exclude_embs: bool = False,
+def watch(
+    model: Module,
+    dataloaders: Optional[List[DataLoader]] = [],
+    classifier_layer: Optional[Union[str, Module]] = None,
+    embedding_dim: Optional[InputDim] = None,
+    logits_dim: Optional[InputDim] = None,
+    embedding_fn: Optional[Callable] = None,
+    logits_fn: Optional[Callable] = None,
+    last_hidden_state_layer: Union[Module, str, None] = None,
+    unpatch_on_start: bool = False,
+    dataloader_random_sampling: bool = False,
 ) -> None:
-    """Logs model outputs for model during training/test/validation.
-
-    :param embs: The embeddings per output sample
-    :param ids: The ids for each sample. Must match input ids of logged samples
-    :param split: The current split. Must be set either here or via dq.set_split
-    :param epoch: The current epoch. Must be set either here or via dq.set_epoch
-    :param logits: The logits for each sample
-    :param probs: Deprecated, use logits. If passed in, a softmax will NOT be applied
-    :param inference_name: Inference name indicator for this inference split.
-        If logging for an inference split, this is required.
-    :param exclude_embs: Optional flag to exclude embeddings from logging. If True and
-        embs is set to None, this will generate random embs for each sample.
-
-    The expected argument shapes come from the task_type being used
-    See dq.docs() for more task specific details on parameter shape
-    """
-    assert all(
-        [config.task_type, config.current_project_id, config.current_run_id]
-    ), "You must call dataquality.init before logging data"
-    assert (probs is not None) or (
-        logits is not None
-    ), "You must provide either logits or probs"
-    assert (embs is None and exclude_embs) or (
-        embs is not None and not exclude_embs
-    ), "embs can be omitted if and only if exclude_embs is True"
-    if embs is None and exclude_embs:
-        embs = np.random.rand(len(ids), DEFAULT_RANDOM_EMB_DIM)
-
-    model_logger = get_model_logger()(
-        embs=embs,
-        ids=ids,
-        split=Split[split].value if split else "",
-        epoch=epoch,
-        logits=logits,
-        probs=probs,
-        inference_name=inference_name,
-    )
-    model_logger.log()
-
-
-@check_noop
-def set_labels_for_run(labels: Union[List[List[str]], List[str]]) -> None:
-    """
-    Creates the mapping of the labels for the model to their respective indexes.
-
-    :param labels: An ordered list of labels (ie ['dog','cat','fish']
-    If this is a multi-label type, then labels are a list of lists where each inner
-    list indicates the label for the given task
-
-    This order MUST match the order of probabilities that the model outputs.
-
-    In the multi-label case, the outer order (order of the tasks) must match the
-    task-order of the task-probabilities logged as well.
     """
-    a.log_function("dq/set_labels_for_run")
-
-    if isinstance(labels[0], (int, np.integer)):
-        get_data_logger().logger_config.int_labels = True
-    get_data_logger().logger_config.labels = labels
-
-
-@check_noop
-def set_tasks_for_run(tasks: List[str], binary: bool = True) -> None:
-    """Sets the task names for the run (multi-label case only).
-
-    This order MUST match the order of the labels list provided in log_input_data
-    and the order of the probability vectors provided in log_model_outputs.
-
-    This also must match the order of the labels logged in set_labels_for_run (meaning
-    that the first list of labels must be the labels of the first task passed in here)
-
-    :param tasks: The list of tasks for your run
-    :param binary: Whether this is a binary multi label run. If true, tasks will also
-    be set as your labels, and you should NOT call `dq.set_labels_for_run` it will be
-    handled for you. Default True
-    """
-    if config.task_type != TaskType.text_multi_label:
-        raise GalileoException("You can only set task names for multi-label use cases.")
-    get_data_logger().logger_config.tasks = tasks
-    text_multi_label_logger_config.binary = binary
-    if binary:
-        # The labels validator will handle adding the "NOT_" to each label
-        text_multi_label_logger_config.labels = [[task] for task in tasks]
-
-
-@check_noop
-def set_tagging_schema(tagging_schema: TaggingSchema) -> None:
-    """Sets the tagging schema for NER models
-
-    Only valid for text_ner task_types. Others will throw an exception
-    """
-    get_data_logger().set_tagging_schema(tagging_schema)
-
-
-def get_model_logger(task_type: TaskType = None) -> Type[BaseGalileoModelLogger]:
-    task_type = _get_task_type(task_type)
-    return BaseGalileoModelLogger.get_logger(task_type)
-
-
-def get_data_logger(task_type: TaskType = None) -> BaseGalileoDataLogger:
-    task_type = _get_task_type(task_type)
-    return BaseGalileoDataLogger.get_logger(task_type)()
+    wraps a PyTorch model and optionally dataloaders to log the
+    embeddings and logits to [Galileo](https://www.rungalileo.io/).
 
+    .. code-block:: python
 
-def _get_task_type(task_type: TaskType = None) -> TaskType:
-    task = task_type or config.task_type
-    if not task:
+        dq.log_dataset(train_dataset, split="train")
+        train_dataloader = torch.utils.data.DataLoader()
+        model = TextClassificationModel(num_labels=len(train_dataset.list_of_labels))
+        watch(model, [train_dataloader, test_dataloader])
+        for epoch in range(NUM_EPOCHS):
+            dq.set_epoch_and_split(epoch,"training")
+            train()
+            dq.set_split("validation")
+            validate()
+        dq.finish()
+
+    :param model: Pytorch Model to be wrapped
+    :param dataloaders: List of dataloaders to be wrapped
+    :param classifier_layer: Layer to hook into (usually 'classifier' or 'fc').
+        Inputs are the embeddings and outputs are the logits.
+    :param embedding_dim: Dimension of the embeddings for example `"[:, 0]"`
+        to remove the cls token
+    :param logits_dim: Dimension of the logits from layer input and
+        logits from layer output. For example in NER `"[:,1:,:]"`.
+        If the layer is not found, the last_hidden_state_layer will be used
+    :param embedding_fn: Function to process embeddings from the model
+    :param logits_fn: Function to process logits from the model f.e.
+        `lambda x: x[0]`
+    :param last_hidden_state_layer: Layer to extract the embeddings from
+    :param unpatch_on_start: Force unpatching of dataloaders
+        instead of global patching
+    :param model: Pytorch Model to be wrapped
+    :param dataloaders: List of dataloaders to be wrapped
+    :param last_hidden_state_layer: Layer to extract the embeddings from
+    :param unpatch_on_start: Force unpatching of dataloaders
+        instead of global patching
+    :param dataloader_random_sampling: Whether a RandomSampler
+        or WeightedRandomSampler is being used. If random sampling
+        is being used, you must set this to True, otherwise logging
+        will fail at the end of training.
+
+    """
+    a.log_function("torch/watch")
+    assert dq.config.task_type, GalileoException(
+        "dq client must be initialized. " "For example: dq.init('text_classification')"
+    )
+    if unpatch_on_start:
+        unwatch(model, force=True)
+    if not getattr(model, "_dq", False):
+        setattr(model, "_dq", True)
+    else:
         raise GalileoException(
-            "You must provide either a task_type or first call "
-            "dataqualtiy.init and provide one"
+            "Model is already being watched, run unwatch(model) first"
         )
-    return task
 
+    helper_data = dq.get_model_logger().logger_config.helper_data
 
-def docs() -> None:
-    """Print the documentation for your specific input and output logging format
-
-    Based on your task_type, this will print the appropriate documentation
-    """
-    get_data_logger().doc()
-    get_model_logger().doc()
-
-
-@check_noop
-def set_epoch(epoch: int) -> None:
-    """Set the current epoch.
-
-    When set, logging model outputs will use this if not logged explicitly
-    """
-    get_data_logger().logger_config.cur_epoch = epoch
-
-
-@check_noop
-def set_split(split: Split, inference_name: Optional[str] = None) -> None:
-    """Set the current split.
-
-    When set, logging data inputs/model outputs will use this if not logged explicitly
-    When setting split to inference, inference_name must be included
-    """
-    get_data_logger().logger_config.cur_inference_name = inference_name
-    split = Split[split]
-    setattr(get_data_logger().logger_config, f"{split}_logged", True)
-    # Set cur_inference_name before split for pydantic validation
-    get_data_logger().logger_config.cur_split = split
+    logger_config = get_data_logger().logger_config
 
+    print("Attaching dataquality to model and dataloaders")
+    tl = TorchLogger(
+        model=model,
+        last_hidden_state_layer=last_hidden_state_layer,
+        embedding_dim=embedding_dim,
+        logits_dim=logits_dim,
+        classifier_layer=classifier_layer,
+        embedding_fn=embedding_fn,
+        logits_fn=logits_fn,
+        task=dq.config.task_type,
+        helper_data=helper_data,
+    )
+    # Patch the dataloader class if no dataloaders are passed
+    # or if the dataloaders have num_workers > 0
+    if dataloaders is None:
+        dataloaders = []
+    is_single_process_dataloader = all(
+        [getattr(d, "num_workers", 0) == 0 for d in dataloaders]
+    )
+    if len(dataloaders) > 0 and is_single_process_dataloader:
+        for dataloader in dataloaders:
+            if not isinstance(getattr(dataloader, "sampler", None), SequentialSampler):
+                logger_config = get_data_logger().logger_config
+                logger_config.dataloader_random_sampling = True
+
+            assert isinstance(dataloader, DataLoader), GalileoException(
+                "Invalid dataloader. Must be a pytorch dataloader"
+                "from torch.utils.data import DataLoader..."
+                "train_dataloader = DataLoader(dataset)"
+            )
+            assert (
+                getattr(dataloader, "num_workers", 0) == 0
+            ), "Dataloaders with num_workers > 0 are not supported"
+
+            # Patch the dataloader class
+            PatchSingleDataloaderIterator(
+                dataloader, tl.torch_helper_data.model_outputs_store
+            )
+
+    else:
+        # Patch the dataloader class globally
+        # Can be unpatched with unwatch()
+        PatchDataloadersGlobally(tl.torch_helper_data)
+    if dataloader_random_sampling:
+        logger_config.dataloader_random_sampling = True
+    cleanup_manager = RefManager(lambda: unwatch(model))
+    helper_data["cleaner"] = Cleanup(cleanup_manager)
+
+
+def unwatch(model: Optional[Module] = None, force: bool = True) -> None:
+    """Unwatches the model. Run after the run is finished.
+    :param force: Force unwatch even if the model is not watched"""
+
+    torch_helper_data: TorchHelper = (
+        dq.get_model_logger().logger_config.helper_data.get(
+            "torch_helper", TorchHelper()
+        )
+    )
 
-@check_noop
-def set_epoch_and_split(
-    epoch: int, split: Split, inference_name: Optional[str] = None
-) -> None:
-    """Set the current epoch and set the current split.
-    When set, logging data inputs/model outputs will use this if not logged explicitly
-    When setting split to inference, inference_name must be included
-    """
-    set_epoch(epoch)
-    set_split(split, inference_name)
+    model = model or torch_helper_data.model
+    if not getattr(model or {}, "_dq", False):
+        warn("Model is not watched, run watch(model) first")
+        if not force:
+            return
+
+    # Unpatch the dataloaders
+
+    unpatch(torch_helper_data.patches or [])
+    # Detach hooks the model. in the future use the model passed
+    # https://discuss.pytorch.org/t/how-to-check-where-the-hooks-are-in-the-model/120120/2
+    hook_manager = torch_helper_data.hook_manager
+    if hook_manager:
+        hook_manager.detach_hooks()
+    # Remove the model from the helper data
+    if isinstance(model, Module):
+        remove_all_forward_hooks(model)
+    else:
+        warnings.warn("model is not a Module")
+    torch_helper_data.model = None
+    if model and hasattr(model, "_dq"):
+        del model._dq
```

### Comparing `dataquality-0.8.9/dataquality/core/report.py` & `dataquality-0.9.0a0/dataquality/core/report.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.9/dataquality/dq_auto/auto.py` & `dataquality-0.9.0a0/dataquality/dq_auto/auto.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,36 @@
-from typing import Dict, List, Union
+from typing import Dict, List, Optional, Union
 
 import pandas as pd
 from datasets import Dataset, DatasetDict
 
 from dataquality.schemas.task_type import TaskType
 from dataquality.utils.auto import get_task_type_from_data
 
 AUTO_PROJECT_NAME = {
     TaskType.text_classification: "auto_tc",
     TaskType.text_ner: "auto_ner",
 }
 
 
 def auto(
-    hf_data: Union[DatasetDict, str] = None,
-    hf_inference_names: List[str] = None,
-    train_data: Union[pd.DataFrame, Dataset, str] = None,
-    val_data: Union[pd.DataFrame, Dataset, str] = None,
-    test_data: Union[pd.DataFrame, Dataset, str] = None,
-    inference_data: Dict[str, Union[pd.DataFrame, Dataset, str]] = None,
+    hf_data: Optional[Union[DatasetDict, str]] = None,
+    hf_inference_names: Optional[List[str]] = None,
+    train_data: Optional[Union[pd.DataFrame, Dataset, str]] = None,
+    val_data: Optional[Union[pd.DataFrame, Dataset, str]] = None,
+    test_data: Optional[Union[pd.DataFrame, Dataset, str]] = None,
+    inference_data: Optional[Dict[str, Union[pd.DataFrame, Dataset, str]]] = None,
     max_padding_length: int = 200,
     hf_model: str = "distilbert-base-uncased",
-    labels: List[str] = None,
-    project_name: str = None,
-    run_name: str = None,
+    num_train_epochs: int = 15,
+    labels: Optional[List[str]] = None,
+    project_name: Optional[str] = None,
+    run_name: Optional[str] = None,
     wait: bool = True,
-    create_data_embs: bool = False,
+    create_data_embs: Optional[bool] = None,
 ) -> None:
     """Automatically gets insights on a text classification or NER dataset
 
     Given either a pandas dataframe, file_path, or huggingface dataset path, this
     function will load the data, train a huggingface transformer model, and
     provide Galileo insights via a link to the Galileo Console
 
@@ -74,147 +75,170 @@
         * Huggingface dataset
         * Path to a local file
         * Huggingface dataset hub path
     :param max_padding_length: The max length for padding the input text
         during tokenization. Default 200
     :param hf_model: The pretrained AutoModel from huggingface that will be used to
         tokenize and train on the provided data. Default distilbert-base-uncased
+    :param num_train_epochs: The number of epochs to train for (early stopping will
+        always be active). Default 15
     :param labels: Optional list of labels for this dataset. If not provided, they
         will attempt to be extracted from the data
     :param project_name: Optional project name. If not set, a random name will
         be generated
     :param run_name: Optional run name for this data. If not set, a random name will
         be generated
     :param wait: Whether to wait for Galileo to complete processing your run.
         Default True
     :param create_data_embs: Whether to create data embeddings for this run. If True,
         Sentence-Transformers will be used to generate data embeddings for this dataset
         and uploaded with this run. You can access these embeddings via
         `dq.metrics.get_data_embeddings` in the `emb` column or
         `dq.metrics.get_dataframe(..., include_data_embs=True)` in the `data_emb` col
-        Only available for TC currently. NER coming soon. Default False.
+        Only available for TC currently. NER coming soon. Default True if a GPU is
+        available, else default False.
 
     For text classification datasets, the only required columns are `text` and `label`
 
     For NER, the required format is the huggingface standard format of `tokens` and
     `tags` (or `ner_tags`).
     See example: https://huggingface.co/datasets/rungalileo/mit_movies
 
         MIT Movies dataset in huggingface format
 
+    .. code-block:: python
+
         tokens	                                            ner_tags
         [what, is, a, good, action, movie, that, is, r...	[0, 0, 0, 0, 7, 0, ...
         [show, me, political, drama, movies, with, jef...	[0, 0, 7, 8, 0, 0, ...
         [what, are, some, good, 1980, s, g, rated, mys...	[0, 0, 0, 0, 5, 6, ...
         [list, a, crime, film, which, director, was, d...	[0, 0, 7, 0, 0, 0, ...
         [is, there, a, thriller, movie, starring, al, ...	[0, 0, 0, 7, 0, 0, ...
         ...                                               ...                      ...
 
 
     To see auto insights on a random, pre-selected dataset, simply run
-    ```python
+
+    .. code-block:: python
+
         import dataquality as dq
 
         dq.auto()
-    ```
+
 
     An example using `auto` with a hosted huggingface text classification dataset
-    ```python
+
+    .. code-block:: python
+
         import dataquality as dq
 
         dq.auto(hf_data="rungalileo/trec6")
-    ```
+
 
     Similarly, for NER
-    ```python
+
+    .. code-block:: python
+
         import dataquality as dq
 
         dq.auto(hf_data="conll2003")
-    ```
+
 
     An example using `auto` with sklearn data as pandas dataframes
-    ```python
+
+    .. code-block:: python
+
+        import dataquality as dq
         import pandas as pd
         from sklearn.datasets import fetch_20newsgroups
-        from dataquality.auto.text_classification import auto
 
         # Load the newsgroups dataset from sklearn
         newsgroups_train = fetch_20newsgroups(subset='train')
         newsgroups_test = fetch_20newsgroups(subset='test')
         # Convert to pandas dataframes
         df_train = pd.DataFrame(
             {"text": newsgroups_train.data, "label": newsgroups_train.target}
         )
         df_test = pd.DataFrame(
             {"text": newsgroups_test.data, "label": newsgroups_test.target}
         )
 
-        auto(
+        dq.auto(
              train_data=df_train,
              test_data=df_test,
              labels=newsgroups_train.target_names,
              project_name="newsgroups_work",
              run_name="run_1_raw_data"
         )
-    ```
+
 
     An example of using `auto` with a local CSV file with `text` and `label` columns
-    ```python
-    from dataquality.auto.text_classification import auto
 
-    auto(
-         train_data="train.csv",
-         test_data="test.csv",
-         project_name="data_from_local",
-         run_name="run_1_raw_data"
-    )
-    ```
+    .. code-block:: python
+
+        import dataquality as dq
+
+        dq.auto(
+            train_data="train.csv",
+            test_data="test.csv",
+            project_name="data_from_local",
+            run_name="run_1_raw_data"
+        )
     """
+    import datasets
+    import transformers
+
+    transformers.logging.enable_progress_bar()
+    datasets.logging.enable_progress_bar()
+
     # We need to import auto down here instead of at the top of the file like normal
     # because we simultaneously want analytic tracking on the files we import while
     # wanting dq.auto as a top level function. If we have these imports at the top,
     # and make dq.auto() available, then auto_tc and auto_ner will both always be
     # imported as soon as dataquality is imported. Also, transformers_trainer and
     # pytorch (which auto depends on) will be immediately imported. The only way to
     # avoid that is by having the imports only be made selectively when auto is called
     if hf_data is None and train_data is None:
         from dataquality.dq_auto.text_classification import auto as auto_tc
 
-        auto_tc()
+        auto_tc(num_train_epochs=num_train_epochs)
+        return
     task_type = get_task_type_from_data(hf_data, train_data)
     # We cannot use a common list of *args or **kwargs here because mypy screams :(
     if task_type == TaskType.text_classification:
         from dataquality.dq_auto.text_classification import auto as auto_tc
 
-        auto_tc(
+        return auto_tc(
             hf_data=hf_data,
             hf_inference_names=hf_inference_names,
             train_data=train_data,
             val_data=val_data,
             test_data=test_data,
             inference_data=inference_data,
             max_padding_length=max_padding_length,
             hf_model=hf_model,
             labels=labels,
             project_name=project_name or AUTO_PROJECT_NAME[task_type],
             run_name=run_name,
             wait=wait,
             create_data_embs=create_data_embs,
+            num_train_epochs=num_train_epochs,
         )
     elif task_type == TaskType.text_ner:
         from dataquality.dq_auto.ner import auto as auto_ner
 
-        auto_ner(
+        return auto_ner(
             hf_data=hf_data,
             hf_inference_names=hf_inference_names,
             train_data=train_data,
             val_data=val_data,
             test_data=test_data,
             inference_data=inference_data,
             hf_model=hf_model,
             labels=labels,
             project_name=project_name or AUTO_PROJECT_NAME[task_type],
             run_name=run_name,
             wait=wait,
+            num_train_epochs=num_train_epochs,
         )
     else:
         raise Exception("auto is only supported for text classification and NER!")
```

### Comparing `dataquality-0.8.9/dataquality/dq_auto/base_data_manager.py` & `dataquality-0.9.0a0/dataquality/dq_auto/base_data_manager.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from typing import Dict, List, Optional, Union
 
 import pandas as pd
 from datasets import Dataset, DatasetDict
 
 from dataquality.exceptions import GalileoException
 from dataquality.schemas.split import Split
-from dataquality.utils.auto import load_data_from_str, try_load_dataset_dict
+from dataquality.utils.auto import (
+    _apply_column_mapping,
+    load_data_from_str,
+    try_load_dataset_dict,
+)
 
 
 class BaseDatasetManager:
     DEMO_DATASETS: List[str] = []
 
     def _validate_dataset_dict(
         self,
@@ -36,43 +40,50 @@
     ) -> Dataset:
         return Dataset.from_pandas(df)
 
     def _convert_to_hf_dataset(
         self,
         data: Union[pd.DataFrame, Dataset, str],
         labels: Optional[List[str]] = None,
+        column_mapping: Optional[Dict[str, str]] = None,
     ) -> Dataset:
         """Loads the data into (hf) Dataset format.
 
         Data can be one of Dataset, pandas df, str. If str, it's either a path to a
         file or a path to a remote huggingface Dataset that we load with `load_dataset`
         """
+        ds = None
         if isinstance(data, Dataset):
-            return data
-        if isinstance(data, pd.DataFrame):
-            return self._convert_df_to_dataset(data, labels)
-        if isinstance(data, str):
+            ds = data
+        elif isinstance(data, pd.DataFrame):
+            ds = self._convert_df_to_dataset(data, labels)
+        elif isinstance(data, str):
             ds = load_data_from_str(data)
             if isinstance(ds, pd.DataFrame):
                 ds = self._convert_df_to_dataset(ds, labels)
-            return ds
-        raise GalileoException(
-            "Dataset must be one of pandas DataFrame, "
-            "huggingface Dataset, or string path"
-        )
+        if column_mapping is not None and ds is not None:
+            ds = _apply_column_mapping(ds, column_mapping)
+
+        if ds is None:
+            raise GalileoException(
+                "Dataset must be one of pandas DataFrame, "
+                "huggingface Dataset, or string path"
+            )
+        return ds
 
     def get_dataset_dict(
         self,
-        hf_data: Union[DatasetDict, str] = None,
-        hf_inference_names: List[str] = None,
-        train_data: Union[pd.DataFrame, Dataset, str] = None,
-        val_data: Union[pd.DataFrame, Dataset, str] = None,
-        test_data: Union[pd.DataFrame, Dataset, str] = None,
-        inference_data: Dict[str, Union[pd.DataFrame, Dataset, str]] = None,
+        hf_data: Optional[Union[DatasetDict, str]] = None,
+        hf_inference_names: Optional[List[str]] = None,
+        train_data: Optional[Union[pd.DataFrame, Dataset, str]] = None,
+        val_data: Optional[Union[pd.DataFrame, Dataset, str]] = None,
+        test_data: Optional[Union[pd.DataFrame, Dataset, str]] = None,
+        inference_data: Optional[Dict[str, Union[pd.DataFrame, Dataset, str]]] = None,
         labels: Optional[List[str]] = None,
+        column_mapping: Optional[Dict[str, str]] = None,
     ) -> DatasetDict:
         """Creates and/or validates the DatasetDict provided by the user.
 
         If the user provides a DatasetDict, we simply validate it. Otherwise, we
         parse a combination of the parameters provided, generate a DatasetDict of their
         training data, and validate that.
         """
@@ -83,17 +94,25 @@
             or DatasetDict()
         )
         if dd:
             inf_names = [i for i in hf_inference_names if i in dd]
         else:
             # We don't need to check for train because `try_load_dataset_dict` validates
             # that it exists already. One of hf_data or train_data must exist
-            dd[Split.train] = self._convert_to_hf_dataset(train_data, labels)
+            dd[Split.train] = self._convert_to_hf_dataset(
+                train_data, labels, column_mapping
+            )
             if val_data is not None:
-                dd[Split.validation] = self._convert_to_hf_dataset(val_data, labels)
+                dd[Split.validation] = self._convert_to_hf_dataset(
+                    val_data, labels, column_mapping
+                )
             if test_data is not None:
-                dd[Split.test] = self._convert_to_hf_dataset(test_data, labels)
+                dd[Split.test] = self._convert_to_hf_dataset(
+                    test_data, labels, column_mapping
+                )
             if inference_data is not None:
                 for inf_name, inf_df in inference_data.items():
-                    dd[inf_name] = self._convert_to_hf_dataset(inf_df, labels)
+                    dd[inf_name] = self._convert_to_hf_dataset(
+                        inf_df, labels, column_mapping
+                    )
                     inf_names.append(inf_name)
         return self._validate_dataset_dict(dd, inf_names, labels)
```

### Comparing `dataquality-0.8.9/dataquality/dq_auto/ner.py` & `dataquality-0.9.0a0/dataquality/dq_auto/ner.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,24 +42,25 @@
                 assert (
                     "tags" in ds.features or "ner_tags" in ds.features
                 ), "Dataset must have column `tags` or `ner_tags`"
         return add_val_data_if_missing(clean_dd)
 
 
 def auto(
-    hf_data: Union[DatasetDict, str] = None,
-    hf_inference_names: List[str] = None,
-    train_data: Union[pd.DataFrame, Dataset, str] = None,
-    val_data: Union[pd.DataFrame, Dataset, str] = None,
-    test_data: Union[pd.DataFrame, Dataset, str] = None,
-    inference_data: Dict[str, Union[pd.DataFrame, Dataset, str]] = None,
+    hf_data: Optional[Union[DatasetDict, str]] = None,
+    hf_inference_names: Optional[List[str]] = None,
+    train_data: Optional[Union[pd.DataFrame, Dataset, str]] = None,
+    val_data: Optional[Union[pd.DataFrame, Dataset, str]] = None,
+    test_data: Optional[Union[pd.DataFrame, Dataset, str]] = None,
+    inference_data: Optional[Dict[str, Union[pd.DataFrame, Dataset, str]]] = None,
+    num_train_epochs: int = 15,
     hf_model: str = "distilbert-base-uncased",
-    labels: List[str] = None,
+    labels: Optional[List[str]] = None,
     project_name: str = "auto_ner",
-    run_name: str = None,
+    run_name: Optional[str] = None,
     wait: bool = True,
 ) -> None:
     """Automatically gets insights on an NER or Token Classification dataset
 
     Given either a pandas dataframe, file_path, or huggingface dataset path, this
     function will load the data, train a huggingface token classification model, and
     provide Galileo insights via a link to the Galileo Console
@@ -156,18 +157,22 @@
          train_data="train.csv",
          test_data="test.csv",
          project_name="data_from_local",
          run_name="run_1_raw_data"
     )
     ```
     """
-    a.log_function("auto/ner")
     manager = NERDatasetManager()
     dd = manager.get_dataset_dict(
         hf_data, hf_inference_names, train_data, val_data, test_data, inference_data
     )
     dq.login()
+    a.log_function("auto/ner")
     if not run_name and isinstance(hf_data, str):
         run_name = run_name_from_hf_dataset(hf_data)
-    dq.init(TaskType.text_ner, project_name=project_name, run_name=run_name)
-    trainer, encoded_data = get_trainer(dd, hf_model, labels)
-    do_train(trainer, encoded_data, wait)
+    dq.init(
+        TaskType.text_ner,
+        project_name=project_name,
+        run_name=run_name,
+    )
+    trainer, encoded_data = get_trainer(dd, hf_model, num_train_epochs, labels)
+    return do_train(trainer, encoded_data, wait)
```

### Comparing `dataquality-0.8.9/dataquality/dq_auto/ner_trainer.py` & `dataquality-0.9.0a0/dataquality/dq_auto/ner_trainer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,41 @@
-from typing import Dict, List, Optional, Tuple
+from typing import Any, Dict, List, Optional, Tuple
 
-import evaluate
 import numpy as np
 from datasets import DatasetDict
 from transformers import (
     AutoModelForTokenClassification,
     AutoTokenizer,
     DataCollatorForTokenClassification,
     EarlyStoppingCallback,
     EvalPrediction,
     IntervalStrategy,
     Trainer,
     TrainingArguments,
 )
 
 import dataquality as dq
+from dataquality.exceptions import GalileoException
 from dataquality.integrations.hf import tokenize_and_log_dataset
 from dataquality.schemas.hf import HFCol
 from dataquality.schemas.split import Split
+from dataquality.utils.helpers import mps_available
 
-# For NER training, there is only 1 evaluation tool
-# https://huggingface.co/course/chapter7/2#metrics
-metric = evaluate.load("seqeval")
+try:
+    # For NER training, there is only 1 evaluation tool
+    # https://huggingface.co/course/chapter7/2#metrics
+    import evaluate
+
+    metric = evaluate.load("seqeval")
+except ImportError:
+    raise GalileoException(
+        "⚠️ Huggingface evaluate library not installed "
+        "please run `pip install dataquality[evaluate]` "
+        "to enable metrics computation."
+    )
 
 
 def compute_metrics(eval_pred: EvalPrediction) -> Dict:
     """Metrics computation for token classification
 
     Taken directly from the docs https://huggingface.co/course/chapter7/2#metrics
     and updated for typing
@@ -51,55 +61,58 @@
         "accuracy": results["overall_accuracy"],
     }
 
 
 def get_trainer(
     dd: DatasetDict,
     model_checkpoint: str,
+    num_train_epochs: int,
     labels: Optional[List[str]] = None,
 ) -> Tuple[Trainer, DatasetDict]:
     tokenizer = AutoTokenizer.from_pretrained(model_checkpoint, use_fast=True)
 
     default_cols = set(HFCol.get_fields())
     meta = [c for c in dd[Split.train].features if c not in default_cols]
     encoded_datasets = tokenize_and_log_dataset(
         dd, tokenizer, label_names=labels, meta=meta
     )
     # FIXME: Why do I need this? `tokenize_and_log_dataset` returns a DatasetDict
     #  not an Optional[DatasetDict]...?
     assert isinstance(encoded_datasets, DatasetDict)
 
-    model = AutoModelForTokenClassification.from_pretrained(
-        model_checkpoint, num_labels=len(dq.get_model_logger().logger_config.labels)
-    )
+    # Used to properly seed the model
+    def model_init() -> Any:
+        return AutoModelForTokenClassification.from_pretrained(
+            model_checkpoint, num_labels=len(dq.get_model_logger().logger_config.labels)
+        )
 
     batch_size = 64
     has_val = Split.validation in encoded_datasets
     eval_strat = IntervalStrategy.EPOCH if has_val else IntervalStrategy.NO
     load_best_model = has_val  # Can only load the best model if we have validation data
 
     args = TrainingArguments(
         "finetuned",
         evaluation_strategy=eval_strat,
-        learning_rate=2e-5,
         per_device_train_batch_size=batch_size,
         per_device_eval_batch_size=batch_size,
         load_best_model_at_end=load_best_model,
-        num_train_epochs=10,
+        num_train_epochs=num_train_epochs,
         weight_decay=0.01,
         save_strategy=IntervalStrategy.EPOCH,
         logging_strategy=IntervalStrategy.EPOCH,
         logging_dir="./logs",
         seed=42,
+        use_mps_device=mps_available(),
     )
 
     # We pass huggingface datasets here but typing expects torch datasets, so we ignore
     trainer = Trainer(
-        model,
-        args,
+        model_init=model_init,
+        args=args,
         train_dataset=encoded_datasets[Split.train],  # type: ignore
         eval_dataset=encoded_datasets.get(Split.validation),  # type: ignore
         tokenizer=tokenizer,
         compute_metrics=compute_metrics,
         data_collator=DataCollatorForTokenClassification(tokenizer),
         callbacks=[EarlyStoppingCallback(early_stopping_patience=1)],
     )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dataquality-0.8.9/dataquality/dq_auto/tc_trainer.py` & `dataquality-0.9.0a0/dataquality/dq_auto/tc_trainer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,40 @@
 from functools import partial
-from typing import Dict, List, Tuple
+from typing import Any, Dict, List, Tuple
 
-import evaluate
 import numpy as np
 from datasets import Dataset, DatasetDict
-from evaluate import EvaluationModule
 from transformers import (
     AutoModelForSequenceClassification,
     AutoTokenizer,
     BatchEncoding,
     EarlyStoppingCallback,
     EvalPrediction,
     IntervalStrategy,
     PreTrainedTokenizerBase,
     Trainer,
     TrainingArguments,
 )
 
+from dataquality.exceptions import GalileoException
 from dataquality.schemas.split import Split
+from dataquality.utils.helpers import mps_available
 
 EVAL_METRIC = "f1"
 
+try:
+    import evaluate
+    from evaluate import EvaluationModule
+except ImportError:
+    raise GalileoException(
+        "⚠️ Huggingface evaluate library not installed "
+        "please run `pip install dataquality[evaluate]` "
+        "to enable metrics computation."
+    )
+
 
 # Taken from the docs of the trainer module:
 # https://github.com/huggingface/transformers/blob/main/examples/pytorch/
 # text-classification/run_glue.py#L434
 def preprocess_function(
     input_data: Dataset, tokenizer: PreTrainedTokenizerBase, max_length: int
 ) -> BatchEncoding:
@@ -42,52 +52,55 @@
 
 
 def get_trainer(
     dd: DatasetDict,
     labels: List[str],
     model_checkpoint: str,
     max_padding_length: int,
+    num_train_epochs: int,
 ) -> Tuple[Trainer, DatasetDict]:
     tokenizer = AutoTokenizer.from_pretrained(model_checkpoint, use_fast=True)
 
     encoded_datasets = dd.map(
         lambda x: preprocess_function(x, tokenizer, max_padding_length), batched=True
     )
 
-    model = AutoModelForSequenceClassification.from_pretrained(
-        model_checkpoint, num_labels=len(labels)
-    )
+    # Used to properly seed the model
+    def model_init() -> Any:
+        return AutoModelForSequenceClassification.from_pretrained(
+            model_checkpoint, num_labels=len(labels)
+        )
 
     # Training arguments and training part
     metric = evaluate.load(EVAL_METRIC)
     # We use the users chosen evaluation metric by preloading it into the partial
     compute_metrics_partial = partial(compute_metrics, metric)
     batch_size = 64
     has_val = Split.validation in encoded_datasets
     eval_strat = IntervalStrategy.EPOCH if has_val else IntervalStrategy.NO
     load_best_model = has_val  # Can only load the best model if we have validation data
     args = TrainingArguments(
         "finetuned",
         evaluation_strategy=eval_strat,
         save_strategy=IntervalStrategy.EPOCH,
-        learning_rate=3e-4,
         per_device_train_batch_size=batch_size,
         per_device_eval_batch_size=batch_size,
-        num_train_epochs=10,
+        num_train_epochs=num_train_epochs,
         weight_decay=0.01,
         load_best_model_at_end=load_best_model,
         push_to_hub=False,
         report_to=["all"],
         seed=42,
+        use_mps_device=mps_available(),
     )
 
     # We pass huggingface datasets here but typing expects torch datasets, so we ignore
     trainer = Trainer(
-        model,
-        args,
+        model_init=model_init,
+        args=args,
         train_dataset=encoded_datasets[Split.train],  # type: ignore
         eval_dataset=encoded_datasets.get(Split.validation),  # type: ignore
         tokenizer=tokenizer,
         compute_metrics=compute_metrics_partial,
         callbacks=[EarlyStoppingCallback(early_stopping_patience=1)],
     )
     return trainer, encoded_datasets
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dataquality-0.8.9/dataquality/dq_auto/text_classification.py` & `dataquality-0.9.0a0/dataquality/integrations/setfit.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,220 +1,266 @@
-from typing import Dict, List, Optional, Union
+import contextlib
+import io
+from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Union
 
-import numpy as np
 import pandas as pd
-from datasets import ClassLabel, Dataset, DatasetDict
+import torch
+from datasets import Dataset, DatasetDict
 
 import dataquality as dq
-from dataquality import Analytics, ApiClient
-from dataquality.dq_auto.base_data_manager import BaseDatasetManager
-from dataquality.dq_auto.tc_trainer import get_trainer
+from dataquality.analytics import Analytics
+from dataquality.clients.api import ApiClient
+from dataquality.core.log import get_data_logger
+from dataquality.dq_auto.text_classification import (
+    TCDatasetManager,
+    _get_labels,
+)
 from dataquality.schemas.split import Split
 from dataquality.schemas.task_type import TaskType
-from dataquality.utils.auto import add_val_data_if_missing, run_name_from_hf_dataset
-from dataquality.utils.auto_trainer import do_train
+from dataquality.utils.auto import _apply_column_mapping, run_name_from_hf_dataset
+from dataquality.utils.patcher import PatchManager
+from dataquality.utils.setfit import (
+    SetFitModelHook,
+    _prepare_config,
+    _setup_patches,
+    get_trainer,
+    log_preds_setfit,
+    validate_setfit,
+)
+
+a = Analytics(ApiClient, dq.config)  # type: ignore
+a.log_import("setfit")
+
+
+if TYPE_CHECKING:
+    from setfit import SetFitModel, SetFitTrainer
+
+
+def unwatch(setfit_obj: Optional[Union["SetFitModel", "SetFitTrainer"]]) -> None:
+    """Unpatch SetFit model by replacing predict_proba function with original
+    function.
+    :param setfit_obj: SetFitModel or SetFitTrainer
+    """
+    a.log_function("setfit/unwatch")
+    setfitmanager = PatchManager()
+    setfitmanager.unpatch()
+    helper_data = dq.get_data_logger().logger_config.helper_data
+    if helper_data:
+        helper_data.clear()
+
+
+def watch(
+    setfit: Union["SetFitModel", "SetFitTrainer"],
+    labels: Optional[List[str]] = None,
+    project_name: str = "",
+    run_name: str = "",
+    finish: bool = True,
+    wait: bool = False,
+    batch_size: Optional[int] = None,
+    meta: Optional[List] = None,
+    validate_before_training: bool = False,
+) -> Callable:
+    """Watch a SetFit model or trainer and extract model outputs for dataquality.
+    Returns a function that can be used to evaluate the model on a dataset.
+    :param setfit: SetFit model or trainer
+    :param labels: list of labels
+    :param project_name: name of project
+    :param run_name: name of run
+    :param finish: whether to run dq.finish after evaluation
+    :param wait: whether to wait for dq.finish
+    :param batch_size: batch size for evaluation
+    :param meta: meta data for evaluation
+    :param validate_before_training: whether to do a testrun before training
+    :return: dq_evaluate function
+    """
+    a.log_function("setfit/watch")
 
-a = Analytics(ApiClient, dq.config)
-a.log_import("auto_tc")
+    from setfit import SetFitTrainer
+
+    pm = PatchManager()
+    pm.unpatch()
+    # If dq.init has been previously called, we don't need to call it again
+    # To detect this we check the paramater and the dq.config.task_type and
+    # no project_name
+    if project_name or dq.config.task_type != TaskType.text_classification:
+        init_kwargs: Dict[str, Any] = {}
+        if project_name:
+            init_kwargs["project_name"] = project_name
+        if run_name:
+            init_kwargs["run_name"] = run_name
+        dq.init("text_classification", **init_kwargs)
+        print("dataquality initialized on SetFitTrainer/SetFitModel")
+
+    labels = labels or dq.get_data_logger().logger_config.labels
+    _prepare_config()
+    if isinstance(setfit, SetFitTrainer):
+        if validate_before_training:
+            f_err = io.StringIO()
+            f_out = io.StringIO()
+            print("Validating SetFit model before training...")
+            with contextlib.redirect_stderr(f_err), contextlib.redirect_stdout(f_out):
+                validate_setfit(
+                    setfit,
+                    labels,
+                    batch_size=batch_size,
+                    meta=meta,
+                )
+
+        _setup_patches(
+            setfit,
+            labels,
+            finish=finish,
+            wait=wait,
+            batch_size=batch_size,
+            meta=meta,
+        )
+        return evaluate(setfit.model)
+    else:
+        model = setfit
+        assert labels and len(
+            labels
+        ), "Labels must be set (watch(trainer, labels=[...]))"
+        dq.set_labels_for_run(labels)
+        return evaluate(model)
+
+
+def evaluate(
+    model: "SetFitModel",
+) -> Callable:
+    """Watch SetFit model by replacing predict_proba function with SetFitModelHook.
+    :param model: SetFit model
+    :return: SetFitModelHook object"""
+    dq_hook = SetFitModelHook(model)
+    dq_store = dq_hook.store
+
+    def dq_evaluate(
+        dataset: Dataset,
+        split: Split,
+        meta: Optional[List] = None,
+        inference_name: Optional[str] = None,
+        column_mapping: Optional[Dict] = None,
+        batch_size: int = 64,
+        epoch: Optional[int] = None,
+    ) -> torch.Tensor:
+        """Evaluate SetFit model and log input and output to Galileo.
+        :param batch: batch of data as a dictionary
+        :param split: split of data (training, validation, test, inference)
+        :param meta: columns that should be logged as metadata
+        :param inference_name: inference name (if split is inference, must be provided)
+        :param column_mapping: mapping of column names (if different from default)
+        :return: output of SetFitModel.predict_proba function"""
+        a.log_function("setfit/evaluate")
+
+        column_mapping = column_mapping or dict(
+            text="text",
+            id="id",
+            label="label",
+        )
 
+        if column_mapping is not None:
+            dataset = _apply_column_mapping(dataset, column_mapping)
+        if "id" not in dataset.features:
+            dataset = dataset.map(lambda x, idx: {"id": idx}, with_indices=True)
+        if epoch is not None:
+            dq.set_epoch(epoch)
+        cur_epoch = get_data_logger().logger_config.cur_epoch
+        return log_preds_setfit(
+            model=model,
+            dataset=dataset,
+            dq_store=dq_store,
+            batch_size=batch_size,
+            split=split,
+            inference_name=inference_name,
+            meta=meta,
+            epoch=cur_epoch,
+        )
 
-class TCDatasetManager(BaseDatasetManager):
-    DEMO_DATASETS = [
-        "rungalileo/newsgroups",
-        "rungalileo/trec6",
-        "rungalileo/conv_intent",
-        "rungalileo/emotion",
-        "rungalileo/amazon_polarity_30k",
-        "rungalileo/sst2",
-    ]
-
-    def _convert_pandas_object_dtype(self, df: pd.DataFrame) -> pd.DataFrame:
-        """Converts columns of object type to string type for huggingface
-
-        Huggingface DataSets cannot handle mixed-type columns as columns due to Arrow.
-        This casts those columns to strings
-        """
-        for c in df.columns:
-            if df[c].dtype == object:
-                df[c] = df[c].astype("str")
-        return df
-
-    def _add_class_label_to_dataset(
-        self, ds: Dataset, labels: List[str] = None
-    ) -> Dataset:
-        """Map a not ClassLabel 'label' column to a ClassLabel, if possible"""
-        if "label" not in ds.features or isinstance(ds.features["label"], ClassLabel):
-            return ds
-        labels = labels if labels is not None else sorted(set(ds["label"]))
-        # For string columns, map the label2idx so we can cast to ClassLabel
-        if ds.features["label"].dtype == "string":
-            label_to_idx = dict(zip(labels, range(len(labels))))
-            ds = ds.map(lambda row: {"label": label_to_idx[row["label"]]})
-
-        # https://github.com/python/mypy/issues/6239
-        class_label = ClassLabel(num_classes=len(labels), names=labels)  # type: ignore
-        ds = ds.cast_column("label", class_label)
-        return ds
-
-    def _convert_df_to_dataset(
-        self, df: pd.DataFrame, labels: List[str] = None
-    ) -> Dataset:
-        """Converts a pandas dataframe to a well-formed huggingface dataset
-
-        The main thing happening here is that we are taking the pandas label column and
-        mapping it to a Dataset ClassLabel if possible. If not, it will get parsed later
-        or a validation error will be thrown if not possible in `_validate_dataset_dict`
-        """
-        df_copy = self._convert_pandas_object_dtype(df.copy())
-        # If there's no label column, we can't do any ClassLabel conversions. Validation
-        # of the hf DatasetDict will handle this missing label column if it's an
-        # issue. See `_validate_dataset_dict`
-        ds = Dataset.from_pandas(df_copy)
-        return self._add_class_label_to_dataset(ds, labels)
-
-    def _validate_dataset_dict(
-        self,
-        dd: DatasetDict,
-        inference_names: List[str],
-        labels: Optional[List[str]] = None,
-    ) -> DatasetDict:
-        """Validates the core components of the provided (or created) DatasetDict)
-
-        The DatasetDict that the user provides or that we create from the provided
-        train/test/val data must have the following:
-            * all keys must be one of our valid key names
-            * it must have a `text` column
-            * it must have a `label` column
-                * if the `label` column isn't a ClassLabel, we convert it to one
-
-        We then also convert the keys of the DatasetDict to our `Split` key enum so
-        we can access it easier in the future
-        """
-        clean_dd = super()._validate_dataset_dict(dd, inference_names, labels)
-        for key in list(clean_dd.keys()):
-            ds = clean_dd.pop(key)
-            assert "text" in ds.features, "Dataset must have column `text`"
-            if key not in inference_names:
-                assert "label" in ds.features, "Dataset must have column `label`"
-                if not isinstance(ds.features["label"], ClassLabel):
-                    ds = self._add_class_label_to_dataset(ds, labels)
-            if "id" not in ds.features:
-                ds = ds.add_column("id", list(range(ds.num_rows)))
-            clean_dd[key] = ds
-        return add_val_data_if_missing(clean_dd)
-
-
-def _get_labels(dd: DatasetDict, labels: Optional[List[str]] = None) -> List[str]:
-    """Gets the labels for this dataset from the dataset if not provided."""
-    if labels is not None and isinstance(labels, (list, np.ndarray)):
-        return list(labels)
-    train_labels = dd[Split.train].features["label"]
-    if hasattr(train_labels, "names"):
-        return train_labels.names
-    return sorted(set(dd[Split.train]["label"]))
-
-
-def _log_dataset_dict(dd: DatasetDict) -> None:
-    for key in dd:
-        ds = dd[key]
-        default_cols = ["text", "label", "id"]
-        meta = [i for i in ds.features if i not in default_cols]
-        if key in Split.get_valid_keys():
-            dq.log_dataset(ds, meta=meta, split=key)
-        else:
-            dq.log_dataset(ds, meta=meta, split=Split.inference, inference_name=key)
+    return dq_evaluate
 
 
 def auto(
-    hf_data: Union[DatasetDict, str] = None,
-    hf_inference_names: List[str] = None,
-    train_data: Union[pd.DataFrame, Dataset, str] = None,
-    val_data: Union[pd.DataFrame, Dataset, str] = None,
-    test_data: Union[pd.DataFrame, Dataset, str] = None,
-    inference_data: Dict[str, Union[pd.DataFrame, Dataset, str]] = None,
-    max_padding_length: int = 200,
-    hf_model: str = "distilbert-base-uncased",
-    labels: List[str] = None,
-    project_name: str = "auto_tc",
-    run_name: str = None,
+    setfit_model: Union[
+        "SetFitModel", str
+    ] = "sentence-transformers/paraphrase-mpnet-base-v2",
+    hf_data: Optional[Union[DatasetDict, str]] = None,
+    hf_inference_names: Optional[List[str]] = None,
+    train_data: Optional[Union[pd.DataFrame, Dataset, str]] = None,
+    val_data: Optional[Union[pd.DataFrame, Dataset, str]] = None,
+    test_data: Optional[Union[pd.DataFrame, Dataset, str]] = None,
+    inference_data: Optional[Dict[str, Union[pd.DataFrame, Dataset, str]]] = None,
+    labels: Optional[List[str]] = None,
+    project_name: str = "auto_tc_setfit",
+    run_name: Optional[str] = None,
+    training_args: Optional[Dict[str, Any]] = None,
+    column_mapping: Optional[Dict[str, str]] = None,
     wait: bool = True,
-    create_data_embs: bool = False,
-) -> None:
-    """Automatically gets insights on a text classification dataset
-
-    Given either a pandas dataframe, file_path, or huggingface dataset path, this
-    function will load the data, train a huggingface transformer model, and
-    provide Galileo insights via a link to the Galileo Console
-
-    One of `hf_data`, `train_data` should be provided. If neither of those are, a
-    demo dataset will be loaded by Galileo for training.
-
-    :param hf_data: Union[DatasetDict, str] Use this param if you have huggingface
-        data in the hub or in memory. Otherwise see `train_data`, `val_data`,
-        and `test_data`. If provided, train_data, val_data, and test_data are ignored
-    :param hf_inference_names: A list of key names in `hf_data` to be run as inference
-        runs after training. If set, those keys must exist in `hf_data`
-    :param train_data: Optional training data to use. Can be one of
-        * Pandas dataframe
-        * Huggingface dataset
-        * Path to a local file
-        * Huggingface dataset hub path
-    :param val_data: Optional validation data to use. The validation data is what is
-        used for the evaluation dataset in huggingface, and what is used for early
-        stopping. If not provided, but test_data is, that will be used as the evaluation
-        set. If neither val nor test are available, the train data will be randomly
-        split 80/20 for use as evaluation data.
-        Can be one of
-        * Pandas dataframe
-        * Huggingface dataset
-        * Path to a local file
-        * Huggingface dataset hub path
-    :param test_data: Optional test data to use. The test data, if provided with val,
-        will be used after training is complete, as the held-out set. If no validation
-        data is provided, this will instead be used as the evaluation set.
-        Can be one of
-        * Pandas dataframe
-        * Huggingface dataset
-        * Path to a local file
-        * Huggingface dataset hub path
-    :param inference_data: Optional inference datasets to run with after training
-        completes. The structure is a dictionary with the key being the infeerence name
-        and the value one of
-        * Pandas dataframe
-        * Huggingface dataset
-        * Path to a local file
-        * Huggingface dataset hub path
-    :param max_padding_length: The max length for padding the input text
-        during tokenization. Default 200
-    :param hf_model: The pretrained AutoModel from huggingface that will be used to
-        tokenize and train on the provided data. Default distilbert-base-uncased
-    :param labels: Optional list of labels for this dataset. If not provided, they
-        will attempt to be extracted from the data
-    :param project_name: Optional project name. If not set, a random name will
-        be generated
-    :param run_name: Optional run name for this data. If not set, a random name will
-        be generated
-    :param wait: Whether to wait for Galileo to complete processing your run.
-        Default True
-    :param create_data_embs: Whether to create data embeddings for this run. Default
-        False
-
-    To see auto insights on a random, pre-selected dataset, simply run
-    ```python
-        from dataquality.auto.text_classification import auto
-
-        auto()
-    ```
-
-    An example using `auto` with a hosted huggingface dataset
-    ```python
-        from dataquality.auto.text_classification import auto
-
-        auto(hf_data="rungalileo/trec6")
-    ```
+    create_data_embs: Optional[bool] = None,
+) -> Union["SetFitModel", "SetFitTrainer"]:
+    """Automatically processes and generates insights on a text classification dataset.
+
+    Given a pandas dataframe, a file path, or a Huggingface dataset path, this
+    function will load the data, train a Huggingface transformer model, and
+    provide insights via a link to the Console.
+
+    At least one of `hf_data`, `train_data` should be provided. If neither of
+    those are, a demo dataset will be used for training.
+
+    Parameters
+    ----------
+    setfit : SetFitModel or Huggingface model name
+        Computes text embeddings for a given text dataset with the model.
+        If a string is provided, it will be used to load a Huggingface model
+        and train it on the data.
+    hf_data : Union[DatasetDict, str], optional
+        Use this parameter if you have Huggingface data in the hub or in memory.
+        Otherwise see `train_data`, `val_data`, and `test_data`. If provided,
+        train_data, val_data, and test_data are ignored.
+    hf_inference_names : list of str, optional
+        A list of key names in `hf_data` to be run as inference
+        runs after training. If set, those keys must exist in `hf_data`.
+    train_data : pandas.DataFrame, Dataset, str, optional
+        Training data to use. Can be a pandas dataframe, a Huggingface dataset,
+        path to a local file, or Huggingface dataset hub path.
+    val_data : pandas.DataFrame, Dataset, str, optional
+        Validation data to use for evaluation and early stopping. If not provided,
+        but test_data is, that will be used as the evaluation set. If neither val_data
+        nor test_data are available, the train data will be split randomly in
+        80/20 ratio.
+    test_data : pandas.DataFrame, Dataset, str, optional
+        Test data to use. If provided with val_data, will be used after training
+        is complete,as the held-out set. If no validation data is provided,
+        this will instead be used as the evaluation set.
+    inference_data : dict, optional
+        Optional inference datasets to run after training. The structure is a dictionary
+        with the key being the inference name and the value being a pandas dataframe, a
+        Huggingface dataset, path to a local file, or Huggingface dataset hub path.
+    labels : list of str, optional
+        List of labels for this dataset. If not provided, they will attempt to
+        be extracted from the data.
+    project_name : str, optional
+        Project name. If not set, a random name will be generated.
+        Default is "auto_tc_setfit".
+    run_name : str, optional
+        Run name for this data. If not set, a random name will be generated.
+    training_args : dict, optional
+        A dictionary of arguments for the SetFitTrainer. It allows you
+        to customize training configuration such as learning rate,
+        batch size, number of epochs, etc.
+    column_mapping : dict, optional
+        A dictionary of column names to use for the provided data.
+        Needs to map to the following keys: "text", "id", "label".
+    wait : bool, optional
+        Whether to wait for the processing of your run to complete. Default is True.
+    create_data_embs : bool, optional
+        Whether to create data embeddings for this run. Default is None.
+
+    Returns
+    -------
+    SetFitModel or SetFitTrainer
+        A SetFitTrainer instance trained on the provided dataset.
 
     An example using `auto` with sklearn data as pandas dataframes
     ```python
         import pandas as pd
         from sklearn.datasets import fetch_20newsgroups
         from dataquality.auto.text_classification import auto
 
@@ -225,48 +271,122 @@
         df_train = pd.DataFrame(
             {"text": newsgroups_train.data, "label": newsgroups_train.target}
         )
         df_test = pd.DataFrame(
             {"text": newsgroups_test.data, "label": newsgroups_test.target}
         )
 
-        auto(
+        auto(model=model,
              train_data=df_train,
              test_data=df_test,
              labels=newsgroups_train.target_names,
              project_name="newsgroups_work",
              run_name="run_1_raw_data"
         )
     ```
 
     An example of using `auto` with a local CSV file with `text` and `label` columns
     ```python
     from dataquality.auto.text_classification import auto
 
     auto(
+         setfit_model="sentence-transformers/paraphrase-mpnet-base-v2",
          train_data="train.csv",
          test_data="test.csv",
          project_name="data_from_local",
          run_name="run_1_raw_data"
     )
     ```
     """
-    a.log_function("auto/tc")
     manager = TCDatasetManager()
     dd = manager.get_dataset_dict(
         hf_data,
         hf_inference_names,
         train_data,
         val_data,
         test_data,
         inference_data,
         labels,
+        column_mapping,
     )
     labels = _get_labels(dd, labels)
     dq.login()
-    if not run_name and isinstance(hf_data, str):
-        run_name = run_name_from_hf_dataset(hf_data)
+    a.log_function("setfit/auto")
+
+    if not run_name:
+        run_name = run_name_from_hf_dataset(hf_data or "setfit_auto")
     dq.init(TaskType.text_classification, project_name=project_name, run_name=run_name)
     dq.set_labels_for_run(labels)
-    _log_dataset_dict(dd)
-    trainer, encoded_data = get_trainer(dd, labels, hf_model, max_padding_length)
-    do_train(trainer, encoded_data, wait, create_data_embs)
+    if isinstance(setfit_model, str):
+        # Load the model and train it
+        trainer, encoded_data = get_trainer(dd, setfit_model, training_args)
+        return do_train(
+            trainer,
+            encoded_data,
+            wait,
+            create_data_embs,
+        )
+    else:
+        # Don't train, just evaluate
+        return do_model_eval(setfit_model, dd, wait, create_data_embs)
+
+
+def do_model_eval(
+    model: "SetFitModel",
+    encoded_data: DatasetDict,
+    wait: bool,
+    create_data_embs: Optional[bool] = None,
+) -> "SetFitModel":
+    dq_evaluate = watch(
+        model,
+        finish=False,
+    )
+    for split in [Split.train, Split.test, Split.val]:
+        if split in encoded_data:
+            dq_evaluate(
+                encoded_data[split],
+                split=split,
+                # for inference set the split to inference
+                # and pass an inference_name="inference_run_1"
+            )
+
+    inf_names = [k for k in encoded_data if k not in Split.get_valid_keys()]
+    for inf_name in inf_names:
+        dq_evaluate(
+            encoded_data[inf_name],
+            split=Split.inference,  # type: ignore
+            inference_name=inf_name,  # type: ignore
+        )
+
+    dq.finish(wait=wait, create_data_embs=create_data_embs)
+    return model
+
+
+def do_train(
+    trainer: "SetFitTrainer",
+    encoded_data: DatasetDict,
+    wait: bool,
+    create_data_embs: Optional[bool] = None,
+) -> "SetFitTrainer":
+    watch(trainer, finish=False)
+
+    trainer.train()
+    dq_evaluate = watch(trainer, finish=False)
+    if Split.test in encoded_data:
+        # We pass in a huggingface dataset but typing wise they expect a torch dataset
+        dq_evaluate(
+            encoded_data[Split.test],
+            split=Split.test,
+            # for inference set the split to inference
+            # and pass an inference_name="inference_run_1"
+        )
+
+    inf_names = [k for k in encoded_data if k not in Split.get_valid_keys()]
+    for inf_name in inf_names:
+        dq_evaluate(
+            encoded_data[inf_name],
+            split=Split.inference,  # type: ignore
+            inference_name=inf_name,  # type: ignore
+        )
+
+    dq.finish(wait=wait, create_data_embs=create_data_embs)
+    return trainer
```

### Comparing `dataquality-0.8.9/dataquality/integrations/experimental/keras.py` & `dataquality-0.9.0a0/dataquality/integrations/keras.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         super(DataQualityCallback, self).__init__()
         if not tf.executing_eagerly():
             raise GalileoException(
                 "Tensorflow must be running eagerly. "
                 "Set `model.compile(run_eagerly=True)` to fix this"
             )
 
-    def on_train_begin(self, logs: Any = None) -> None:
+    def on_train_begin(self, logs: Optional[Any] = None) -> None:
         """Initialize the training by extracting the model input arguments.
         and from it generate the indices of the batches."""
         assert self.model.run_eagerly, GalileoException(
             "Model must be run run eagerly."
             "Set `model.compile(run_eagerly=True)` to fix this"
         )
 
@@ -98,21 +98,21 @@
 
     def _clear_logger_config_helper_data(self) -> None:
         """Clear the helper data from the logger config for the current step."""
         self.store.pop("input", None)
         self.store.pop("output", None)
         self.store.pop("indices_ids", None)
 
-    def on_train_batch_begin(self, batch: Any, logs: Dict = None) -> None:
+    def on_train_batch_begin(self, batch: Any, logs: Optional[Dict] = None) -> None:
         """At the beginning of the batch we clear the
         helper data from the logger config."""
         self._clear_logger_config_helper_data()
         dq.set_split(Split.train)
 
-    def on_train_batch_end(self, batch: Any, logs: Dict = None) -> None:
+    def on_train_batch_end(self, batch: Any, logs: Optional[Dict] = None) -> None:
         """At the end of the batch we log the input
         of the classifier and the output.
         :param batch: The batch number.
         :param logs: The logs."""
         dq.set_split(Split.train)
         # We try to fetch the indices directly from the store
         ids = self.store.get("indices_ids")
@@ -130,15 +130,15 @@
 
         self.log_function(
             embs=self.store["input"],
             logits=self.store["output"],
             ids=ids,
         )
 
-    def on_test_begin(self, logs: Any = None) -> None:
+    def on_test_begin(self, logs: Optional[Any] = None) -> None:
         """At the beginning of the test we set the split to test.
         And generate the indices of the batches."""
         dq.set_split(Split.test)
         x_len = get_x_len(self.fit_kwargs.get("val_x"))
         if x_len is None:
             self.val_x_len_is_none = True
         else:
@@ -146,21 +146,21 @@
                 x=x_len,
                 batch_size=self.fit_kwargs.get(f"{Split.test}_batch_size")
                 or self.fit_kwargs["batch_size"],
                 steps_per_epoch=self.fit_kwargs.get(f"{Split.test}_steps"),
                 sample_weight=self.fit_kwargs.get("val_sample_weight"),
             )
 
-    def on_test_batch_begin(self, batch: Any, logs: Dict = None) -> None:
+    def on_test_batch_begin(self, batch: Any, logs: Optional[Dict] = None) -> None:
         """At the beginning of the batch we clear the helper
         data from the logger config."""
         self._clear_logger_config_helper_data()
         dq.set_split(Split.test)
 
-    def on_test_batch_end(self, batch: Any, logs: Dict = None) -> None:
+    def on_test_batch_end(self, batch: Any, logs: Optional[Dict] = None) -> None:
         """At the end of the test batch we log the input of the classifier
         and the output."""
         dq.set_split(Split.test)
         ids = self.store.get("indices_ids")
 
         if ids is None:
             step = batch
@@ -193,15 +193,15 @@
         else:
             self.store[f"{Split.validation}_indices"] = generate_indices(
                 x=x_len,
                 batch_size=predict_kwargs.get("batch_size"),
                 steps_per_epoch=predict_kwargs.get("steps"),
             )
 
-    def on_predict_batch_end(self, batch: int, logs: Any = None) -> None:
+    def on_predict_batch_end(self, batch: int, logs: Optional[Any] = None) -> None:
         """Log the validation batch"""
         dq.set_split(Split.validation)
         ids = self.store.get("indices_ids")
         if ids is None:
             step = batch
             ids = self.store.get(f"{Split.validation}_indices", {}).get(
                 f"epoch_0_{step}"
@@ -276,44 +276,47 @@
 
         return orig_func(*args, **kwargs)
 
     return train_step_wrapper
 
 
 def select_model_layer(
-    model: tf.keras.layers.Layer, layer: Optional[Union[tf.keras.layers.Layer, str]]
+    model: tf.keras.layers.Layer, layer: Union[tf.keras.layers.Layer, str, None] = None
 ) -> tf.keras.layers.Layer:
     """Selects the classifier layer from the model.
     :param model: The model.
-    :param layer: The layer to select. If the layer with the name
+    :param layer: The layer to select. If None, the layer with the name
     'classifier' is selected."""
-    chosen_layer = layer
-    if isinstance(chosen_layer, str) is None:
+    chosen_layer = None
+    if isinstance(layer, tf.keras.layers.Layer):
+        chosen_layer = layer
+    elif isinstance(layer, str):
         for model_layer in model.layers:
             if model_layer.name == layer:
                 chosen_layer = model_layer
                 break
     else:
+        layer = "classifier"
         for model_layer in model.layers:
-            if model_layer.name == "classifier":
+            if model_layer.name == layer:
                 chosen_layer = model_layer
                 break
-    assert chosen_layer is not None, GalileoException("Layer could not be found")
-    assert not isinstance(chosen_layer, str), GalileoException(
-        "Layer could not be found"
+
+    assert chosen_layer is not None, GalileoException(
+        f"Layer {layer} cannot be found, check that it exists in the model's summary."
     )
     return chosen_layer
 
 
 def _watch(
     logger_data: Dict[str, Any],
     logger_config: BaseLoggerConfig,
     log_function: Callable,
     model: tf.keras.layers.Layer,
-    layer: Any = None,
+    layer: Optional[Any] = None,
     seed: int = 42,
 ) -> None:
     """Internal watch function that is used to watch the model during training.
     :param logger_data: The store for temporary logger data
     :param logger_config: The configuration of the logger
     :param log_function: The function that is used to log the data
     :param model: The model that is watched
@@ -356,15 +359,17 @@
     patch_layer_call(
         chosen_layer,
         before_call=partial(save_input, logger_data),
         after_call=partial(save_output, logger_data),
     )
 
 
-def watch(model: tf.keras.layers.Layer, layer: Any = None, seed: int = 42) -> None:
+def watch(
+    model: tf.keras.layers.Layer, layer: Optional[Any] = None, seed: int = 42
+) -> None:
     """Watch a model and log the inputs and outputs of a layer.
     :param model: The model to watch
     :param layer: The layer to watch, if None the classifier layer is used
     :param seed: The seed to use for the model"""
     if not getattr(model, "_dq", False):
         model._dq = True
     else:
```

### Comparing `dataquality-0.8.9/dataquality/integrations/hf.py` & `dataquality-0.9.0a0/dataquality/integrations/hf.py`

 * *Files 4% similar despite different names*

```diff
@@ -130,15 +130,15 @@
     if HFCol.ner_tags in ds.features and hasattr(
         ds.features[HFCol.ner_tags].feature, "names"
     ):
         return ds.features[HFCol.ner_tags].feature.names
     # If there is an "ner_labels" column (like from the Galileo export), we can use that
     if HFCol.ner_labels in ds.features:
         return ds[HFCol.ner_labels][0]
-    # The user must provide them
+    # The user must provide label_names
     raise GalileoException(
         "Could not extract labels from Dataset. Provide `label_names` to the "
         "`tokenize_and_log_dataset` function as a list of strings"
     )
 
 
 @check_noop
@@ -187,19 +187,28 @@
         if ds_key not in Split.get_valid_keys():
             dq_split = Split.inference
             inference_name = ds_key
             kwargs = {"inference_name": inference_name}
             dataset = dataset.remove_columns([HFCol.gold_spans])
         else:
             dq_split = conform_split(ds_key)
-            # Filter out rows with no gold spans
-            dataset = dataset.filter(lambda row: len(row[HFCol.gold_spans]) != 0)
 
+        # Filter out rows with no tokens
+        dataset = dataset.filter(lambda row: len(row[HFCol.text_token_indices]) != 0)
         ids = list(range(len(dataset)))
         dataset = dataset.add_column(HFCol.id, ids)
+        ds_orig_len = len(dataset)
+        ds_len = len(dataset)
+        if ds_orig_len != ds_len:
+            warnings.warn(
+                f"We found {ds_orig_len-ds_len} empty samples in your dataset for "
+                f"split {ds_key}. These will not be logged to Galileo. If you are not "
+                "expecting these, you should inspect your original data",
+                GalileoWarning,
+            )
         tokenized_datasets[ds_key] = dataset
         split_meta = [c for c in meta if c in dataset.features]
         dq.log_dataset(
             dataset, split=dq_split, meta=split_meta, **kwargs  # type: ignore
         )
 
     return tokenized_datasets
```

### Comparing `dataquality-0.8.9/dataquality/loggers/base_logger.py` & `dataquality-0.9.0a0/dataquality/loggers/base_logger.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 import os
 import shutil
 from abc import abstractmethod
 from enum import Enum, unique
+from functools import lru_cache
 from glob import glob
-from typing import Any, Dict, List, Optional, Type, TypeVar, Union
+from typing import Any, Dict, List, Optional, Tuple, Type, TypeVar, Union
 
 import numpy as np
 
-from dataquality.core._config import ConfigData, config
+from dataquality.core._config import config, config_data
 from dataquality.exceptions import GalileoException
 from dataquality.loggers.logger_config.base_logger_config import (
     BaseLoggerConfig,
     base_logger_config,
 )
 from dataquality.schemas.split import Split, conform_split
 from dataquality.schemas.task_type import TaskType
 from dataquality.utils.cloud import is_galileo_cloud
 from dataquality.utils.dq_logger import upload_dq_log_file
+from dataquality.utils.file import _shutil_rmtree_retry
 from dataquality.utils.imports import hf_available, tf_available, torch_available
+from dataquality.utils.patcher import PatchManager
 from dataquality.utils.tf import is_tf_2
 
 T = TypeVar("T", bound="BaseGalileoLogger")
 
 
 @unique
 class BaseLoggerAttributes(str, Enum):
@@ -51,69 +54,124 @@
     pred_emb = "pred_emb"
     gold_emb = "gold_emb"
     pred_spans = "pred_spans"
     text_token_indices = "text_token_indices"
     text_token_indices_flat = "text_token_indices_flat"
     log_helper_data = "log_helper_data"
     inference_name = "inference_name"
+    image = "image"
 
     @staticmethod
     def get_valid() -> List[str]:
         return list(map(lambda x: x.value, BaseLoggerAttributes))
 
 
 class BaseGalileoLogger:
     """
     An abstract base class that all model logger and data loggers inherit from
     """
 
     __logger_name__ = ""
-    LOG_FILE_DIR = f"{ConfigData.DEFAULT_GALILEO_CONFIG_DIR}/logs"
+    LOG_FILE_DIR = f"{config_data.DEFAULT_GALILEO_CONFIG_DIR}/logs"  # type: ignore
     logger_config: BaseLoggerConfig = base_logger_config
 
     def __init__(self) -> None:
         self.split: Optional[str] = None
         self.inference_name: Optional[str] = None
 
+    @property
+    def proj_run(self) -> str:
+        """Returns the project and run id
+
+        Example:
+            proj-id/run-id
+        """
+        return f"{config.current_project_id}/{config.current_run_id}"
+
+    @property
     def write_output_dir(self) -> str:
-        return (
-            f"{BaseGalileoLogger.LOG_FILE_DIR}/{config.current_project_id}/"
-            f"{config.current_run_id}"
-        )
+        """Returns the path to the output directory for the current run
 
+        Example:
+            /Users/username/.galileo/logs/proj-id/run-id
+        """
+        return f"{BaseGalileoLogger.LOG_FILE_DIR}/{self.proj_run}"
+
+    @property
     def split_name(self) -> str:
+        """Returns the name of the current split
+
+        If the split is inference, it will return the name of the inference
+        concatenated to the end of the split name
+
+        Example:
+            training
+            inference_inf-name1
+        """
         split = self.split
         if split == Split.inference:
             split = f"{split}_{self.inference_name}"
         return str(split)
 
+    @property
+    def split_name_path(self) -> str:
+        """Returns the path part of the current split
+
+        If the split is inference, it will return the name of the inference
+        run after the split name
+
+        Example:
+            training
+            inference/inf-name1
+        """
+        split = self.split
+        if split == Split.inference:
+            split = f"{split}/{self.inference_name}"
+        return str(split)
+
     @staticmethod
     def get_valid_attributes() -> List[str]:
         return BaseLoggerAttributes.get_valid()
 
     @abstractmethod
-    def validate(self) -> None:
+    def validate_and_format(self) -> None:
         """Validates params passed in during logging. Implemented by child"""
 
     def set_split_epoch(self) -> None:
+        """Sets the split for the current logger
+
+        If the split is not set, it will use the split set in the logger config
+        """
         if not self.split:
             if self.logger_config.cur_split:
                 self.split = self.logger_config.cur_split
             else:
                 raise GalileoException(
                     "You didn't log a split and did not set a split. Use "
                     "'dataquality.set_split' to set the split"
                 )
+
+        # Inference split must have inference name
+        if self.split == Split.inference and self.inference_name is None:
+            if self.logger_config.cur_inference_name is not None:
+                self.inference_name = self.logger_config.cur_inference_name
+            else:
+                raise GalileoException(
+                    "For inference split you must either log an inference name "
+                    "or set it before logging. Use `dataquality.set_split` to set "
+                    "inference_name"
+                )
+
         self.split = self.validate_split(self.split)
         # Set this config variable in validation, right before logging split data
         setattr(self.logger_config, f"{self.split}_logged", True)
 
     def is_valid(self) -> bool:
         try:
-            self.validate()
+            self.validate_and_format()
         except AssertionError:
             return False
         return True
 
     @classmethod
     def non_inference_logged(cls) -> bool:
         """Return true if training, test, or validation data is logged
@@ -202,39 +260,56 @@
             raise GalileoException(
                 f"Logged data should be of type int, string, pytorch tensor, "
                 f"or tf tensor, but got {type(v)}"
             )
         return v
 
     @staticmethod
-    def validate_task(task_type: Union[str, TaskType]) -> None:
-        if task_type not in TaskType.get_valid_tasks():
+    def validate_task(task_type: Union[str, TaskType]) -> TaskType:
+        """Raises error if task type is not a valid TaskType"""
+        try:
+            return TaskType[task_type]
+        except KeyError:
             raise GalileoException(
                 f"Task type {task_type} not valid. Choose one of "
                 f"{TaskType.get_valid_tasks()}"
             )
 
     @classmethod
     def _cleanup(cls) -> None:
-        """
-        Cleans up the current run data and metadata locally
+        """Cleans up the current run data and metadata locally
+
+        Does so by deleting the run directory and resetting the logger config
+
+        Example:
+            # Deletes all files in the run directory
+            /Users/username/.galileo/logs/proj-id/run-id
         """
         assert config.current_project_id
         assert config.current_run_id
         location = (
             f"{cls.LOG_FILE_DIR}/{config.current_project_id}"
             f"/{config.current_run_id}"
         )
         print("🧹 Cleaning up")
         for path in glob(f"{location}/*"):
             if os.path.isfile(path):
                 os.remove(path)
             else:
-                shutil.rmtree(path)
+                # Sometimes the directory is not deleted immediately
+                # This can happen if the client is using an nfs
+                # so we try again after a short delay
+                try:
+                    shutil.rmtree(path)
+                except OSError:
+                    _shutil_rmtree_retry(path)
+
         cls.logger_config.reset()
+        pm = PatchManager()
+        pm.unpatch()
 
     def upload(self) -> None:
         ...
 
     @classmethod
     def get_all_subclasses(cls: Type[T]) -> List[Type[T]]:
         all_subclasses = []
@@ -253,14 +328,18 @@
 
     @classmethod
     def doc(cls) -> None:
         print(cls.__doc__)
 
     @classmethod
     def validate_split(cls, split: Union[str, Split]) -> str:
+        """Raises error if split is not a valid Split
+
+        Also raises if a cloud user tries to log inference data
+        """
         split = conform_split(split).value
         if is_galileo_cloud() and split == Split.inference:
             raise GalileoException(
                 "You cannot log inference data from a Galileo Cloud account, only "
                 "enterprise accounts can access this feature. Please email us at "
                 "team@rungalileo.io for more information."
             )
@@ -275,31 +354,36 @@
         # If a currently active thread crashed, check and raise a top level exception
         if cls.logger_config.exception:
             upload_dq_log_file()
             raise GalileoException(cls.logger_config.exception)
 
     @classmethod
     def is_hf_dataset(cls, df: Any) -> bool:
-        if hf_available:
+        if hf_available():
             import datasets
 
             return isinstance(df, datasets.Dataset)
         return False
 
+    @staticmethod
+    @lru_cache(1)
+    def _label_idx_map(labels: Tuple[str]) -> Dict[str, int]:
+        return {label: idx for idx, label in enumerate(labels)}
+
     @property
     def label_idx_map(self) -> Dict[str, int]:
         """Convert a list of labels to a dictionary of label to index
 
         Example:
         --------
         >>> labels = ["O", "B-PER", "I-PER", "B-LOC", "I-LOC"]
         >>> label_idx_map(labels)
         {"O": 0, "B-PER": 1, "I-PER": 2, "B-LOC": 3, "I-LOC": 4}
         """
-        return {label: idx for idx, label in enumerate(self.logger_config.labels or [])}
+        return self._label_idx_map(tuple(self.logger_config.labels or []))
 
     def labels_to_idx(self, gold_sequence: List[str]) -> np.ndarray:
         """Convert a list of labels to a np array of indices
 
         Example:
         --------
         # labels = ["O", "B-PER", "I-PER", "B-LOC", "I-LOC"]
```

### Comparing `dataquality-0.8.9/dataquality/loggers/data_logger/base_data_logger.py` & `dataquality-0.9.0a0/dataquality/loggers/data_logger/base_data_logger.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,45 @@
 import gc
 import glob
 import os
-import shutil
 import sys
 import warnings
 from abc import abstractmethod
 from collections import Counter
-from typing import Any, Dict, Iterable, List, Optional, Tuple, TypeVar, Union
+from typing import Any, Dict, Iterable, List, Optional, TypeVar, Union
 
 import numpy as np
 import pandas as pd
-import pyarrow as pa
 import vaex
+from huggingface_hub.utils import HfHubHTTPError
 from vaex.dataframe import DataFrame
 
 from dataquality.clients.objectstore import ObjectStore
 from dataquality.core._config import config
 from dataquality.exceptions import GalileoException, GalileoWarning
 from dataquality.loggers.base_logger import BaseGalileoLogger, BaseLoggerAttributes
-from dataquality.schemas.dataframe import BaseLoggerInOutFrames, DFVar
+from dataquality.schemas.dataframe import BaseLoggerDataFrames, DFVar
 from dataquality.schemas.ner import TaggingSchema
 from dataquality.schemas.split import Split
 from dataquality.utils import tqdm
 from dataquality.utils.cloud import is_galileo_cloud
-from dataquality.utils.hdf5_store import HDF5_STORE
+from dataquality.utils.cuda import cuml_available
+from dataquality.utils.emb import (
+    DATA_EMB_PATH,
+    apply_umap_to_embs,
+    upload_umap_data_embs,
+)
+from dataquality.utils.file import _shutil_rmtree_retry
 from dataquality.utils.helpers import galileo_verbose_logging
 from dataquality.utils.thread_pool import ThreadPoolManager
 from dataquality.utils.vaex import (
     _join_in_out_frames,
-    concat_hdf5_files,
-    create_data_embs,
+    create_data_embs_df,
     filter_df,
+    get_output_df,
     validate_unique_ids,
 )
 
 DATA_FOLDERS = ["emb", "prob", "data"]
 DataSet = TypeVar("DataSet", bound=Union[Iterable, pd.DataFrame, DataFrame])
 MetasType = TypeVar("MetasType", bound=Dict[str, List[Union[str, float, int]]])
 MetaType = TypeVar("MetaType", bound=Dict[str, Union[str, float, int]])
@@ -45,39 +50,67 @@
 try:
     vaex.progress.bar("vaex")
 except NameError:
     vaex.progress._progressbar_registry.registry["vaex"] = vaex.progress.simple
 
 
 class BaseGalileoDataLogger(BaseGalileoLogger):
+    """Base class for data loggers.
+
+    A document col is a large str > 1k chars < 10k chars
+    To avoid massive files, we limit the number of documents logged
+    """
+
     MAX_META_COLS = 25  # Limit the number of metadata attrs a user can log
-    MAX_STR_LEN = 1000  # Max characters in a string metadata attribute
+    MAX_STR_LEN = 1_000  # Max characters in a string metadata attribute
+    MAX_DOC_LEN = 10_000  # Max characters in document metadata attribute
+    LIMIT_NUM_DOCS = 3  # Limit the number of documents logged per split
     INPUT_DATA_BASE = "input_data"
     MAX_DATA_SIZE_CLOUD = 300_000
     # 2GB max size for arrow strings. We use 1.5GB for some buffer
     # https://issues.apache.org/jira/browse/ARROW-17828
     STRING_MAX_SIZE_B = 1.5e9
 
     DATA_FOLDER_EXTENSION = {data_folder: "hdf5" for data_folder in DATA_FOLDERS}
+    INPUT_DATA_FILE_EXT = "arrow"
 
-    def __init__(self, meta: MetasType = None) -> None:
+    def __init__(self, meta: Optional[MetasType] = None) -> None:
         super().__init__()
         self.meta: Dict = meta or {}
         self.log_export_progress = True
 
+    @property
     def input_data_path(self) -> str:
-        return f"{self.write_output_dir()}/{BaseGalileoDataLogger.INPUT_DATA_BASE}"
+        """Return the path to the input data folder.
+
+        Example:
+            /Users/username/.galileo/logs/proj-id/run-id/input_data
+        """
+        return f"{self.write_output_dir}/{BaseGalileoDataLogger.INPUT_DATA_BASE}"
+
+    def input_data_file(
+        self, input_num: Optional[int] = None, split: Optional[str] = None
+    ) -> str:
+        """Return the path to the input data file.
 
-    def input_data_file(self, input_num: int = None, split: str = None) -> str:
+        Example:
+            /Users/username/.galileo/logs/proj-id/run-id/input_data/train/data_0.arrow
+        """
         if not split:
             assert self.split
             split = str(self.split)
         if input_num is None:
+            # input_data_logged is a dict of {split: input_num}
+            # where input_num is incremented in log()
             input_num = self.logger_config.input_data_logged[split]
-        return f"{self.input_data_path()}/{split}/data_{input_num}.arrow"
+
+        return (
+            f"{self.input_data_path}/{split}/"
+            f"data_{input_num}.{self.INPUT_DATA_FILE_EXT}"
+        )
 
     @abstractmethod
     def log_data_sample(self, *, text: str, id: int, **kwargs: Any) -> None:
         """Log a single input sample. See child for details"""
 
     @abstractmethod
     def log_data_samples(
@@ -90,185 +123,260 @@
         self,
         dataset: DataSet,
         *,
         batch_size: int = ITER_CHUNK_SIZE,
         text: Union[str, int] = "text",
         id: Union[str, int] = "id",
         split: Optional[Split] = None,
-        meta: Optional[List[Union[str, int]]] = None,
+        meta: Union[List[str], List[int], None] = None,
         **kwargs: Any,
     ) -> None:
         """Log a dataset/iterable of input samples.
 
         Provide the dataset and the keys to index into it. See child for details"""
 
     def validate_ids_for_split(self, ids: List[int]) -> None:
-        split = self.split_name()
+        """Validate ids for the current split
+
+        Validates:
+        - that the ids are unique for the current split
+        - that the ids are not already logged for the current split
+
+        On success:
+        - adds the ids to the logged_input_ids for the current split
+        """
+        split = self.split_name
         exc = (
             "If you've re-run a block of code or notebook cell that logs model "
             "outputs, that could be the cause. Try reinitializing with `dq.init` "
             "to clear your local environment, and then logging your data again. Call "
             "`dq.enable_galileo_verbose()` to see the duplicate IDs"
         )
         id_set = set(ids)
         if len(id_set) != len(ids):
             exc = "It seems you do not have unique ids in this logged data. " + exc
-            dups = {k: v for k, v in Counter(ids).items() if v > 1}
             if galileo_verbose_logging():
+                dups = {k: v for k, v in Counter(ids).items() if v > 1}
                 exc += f"split:{split}, dup ids and counts: {dups}"
             raise GalileoException(exc)
         # This means some logged ids were already logged!
         if len(id_set - self.logger_config.logged_input_ids[split]) != len(ids):
-            extra = self.logger_config.logged_input_ids[split].intersection(id_set)
             exc = "Some ids in this dataset were already logged for this split. " + exc
             if galileo_verbose_logging():
-                exc += f"split:{split}, overlapping ids: {extra}"
+                overlapping = self.logger_config.logged_input_ids[split].intersection(
+                    id_set
+                )
+                exc += f"split:{split}, overlapping ids: {overlapping}"
             raise GalileoException(exc)
+
         self.logger_config.logged_input_ids[split].update(ids)
 
     def add_ids_to_split(self, ids: List) -> None:
         if self.split:
             self.logger_config.idx_to_id_map[str(self.split)].extend(ids)
 
     def log(self) -> None:
         """Writes input data to disk in .galileo/logs
 
         If input data already exist, append new data to existing input file.
         If the dataset is very large this function will be called multiple
         times for a given split.
         """
-        self.validate()
-        write_input_dir = self.write_output_dir()
+        self.validate_and_format()
+        # E.g. /Users/username/.galileo/logs/proj-id/run-id
+        write_input_dir = self.write_output_dir
         os.makedirs(write_input_dir, exist_ok=True)
-        os.makedirs(f"{self.input_data_path()}/{self.split}", exist_ok=True)
+        # E.g. /Users/username/.galileo/logs/proj-id/run-id/training
+        os.makedirs(f"{self.input_data_path}/{self.split}", exist_ok=True)
 
         df = self._get_input_df()
+        # Validates cloud size limit
         self.validate_data_size(df)
+
         ids = df["id"].tolist()
         self.validate_ids_for_split(ids)
         self.add_ids_to_split(ids)
 
+        self.export_df(df)
+
+    def export_df(self, df: vaex.DataFrame) -> None:
+        """Export the dataframe and increment the input_data_logged
+        in this helper in order to allow for overrides in child classes.
+
+        For instance semseg needs to do this in a multithreaded way and
+        add locks to avoid threading issues
+        """
         file_path = self.input_data_file()
         if self.log_export_progress:
             with vaex.progress.tree("vaex", title=f"Logging {len(df)} samples"):
                 df.export(file_path)
         else:
             df.export(file_path)
 
         df.close()
         self.logger_config.input_data_logged[str(self.split)] += 1
 
+    @property
+    def support_data_embs(self) -> bool:
+        return True
+
     def upload(
         self, last_epoch: Optional[int] = None, create_data_embs: bool = False
     ) -> None:
         """
         Iterates through all of each splits children folders [data/emb/prob] for each
         inference name / epoch, concatenates all of the files with vaex, and uploads
         them to a single file in minio
 
         If create_data_embs is True, this will also run an off the shelf transformer
         and upload those text embeddings alongside the models finetuned embeddings
         """
+        # For linting
+        assert (
+            config.current_project_id and config.current_run_id
+        ), "You must call dq.init and train a model before calling finish"
         ThreadPoolManager.wait_for_threads()
         self.check_for_logging_failures()
         print("☁️ Uploading Data")
         object_store = ObjectStore()
         proj_run = f"{config.current_project_id}/{config.current_run_id}"
         location = f"{self.LOG_FILE_DIR}/{proj_run}"
 
+        if cuml_available():
+            apply_umap_to_embs(location, last_epoch)
+        else:
+            print(
+                "CuML libraries not found, running standard process. "
+                "For faster Galileo processing, consider installing\n"
+                "`pip install 'dataquality[cuda]' --extra-index-url="
+                "https://pypi.nvidia.com/`"
+            )
+
+        if cuml_available() and create_data_embs and self.support_data_embs:
+            print("Creating and uploading data embeddings")
+            upload_umap_data_embs(
+                config.current_project_id,
+                config.current_run_id,
+                self.input_data_path,
+                location,
+                last_epoch,
+            )
+            # We have already created them here, so don't try again later
+            create_data_embs = False
+
         for split in Split.get_valid_attributes():
-            split_loc = f"{location}/{split}"
-            input_logged = os.path.exists(f"{self.input_data_path()}/{split}")
-            output_logged = os.path.exists(split_loc)
-            if not output_logged:
-                continue
-            if not input_logged:
-                warnings.warn(
-                    f"There was output data logged for split {split} but no input data "
-                    "logged. Skipping upload for this split as there are no samples "
-                    "to join to.",
-                    GalileoWarning,
-                )
-                continue
-            in_frame_path = f"{self.input_data_path()}/{split}"
-            in_frame_split = vaex.open(f"{in_frame_path}/*.arrow")
-            in_frame_split = self.convert_large_string(in_frame_split)
             self.upload_split(
-                object_store,
-                in_frame_split,
-                split,
-                split_loc,
-                last_epoch,
-                create_data_embs,
+                location, split, object_store, last_epoch, create_data_embs
             )
-            in_frame_split.close()
-            shutil.rmtree(in_frame_path)
-            gc.collect()
+
+    def upload_split(
+        self,
+        location: str,
+        split: str,
+        object_store: ObjectStore,
+        last_epoch: Optional[int],
+        create_data_embs: bool,
+    ) -> None:
+        split_loc = f"{location}/{split}"
+        in_frame_path = f"{self.input_data_path}/{split}"
+        input_logged = os.path.exists(in_frame_path)
+        output_logged = os.path.exists(split_loc)
+        if not output_logged:
+            return
+        if not input_logged:
+            warnings.warn(
+                f"There was output data logged for split {split} but no input data "
+                "logged. Skipping upload for this split as there are no samples "
+                "to join to.",
+                GalileoWarning,
+            )
+            return
+        in_frame_split = vaex.open(f"{in_frame_path}/*.{self.INPUT_DATA_FILE_EXT}")
+        in_frame_split = self.convert_large_string(in_frame_split)
+        self.upload_split_from_in_frame(
+            object_store,
+            in_frame_split,
+            split,
+            split_loc,
+            last_epoch,
+            create_data_embs,
+        )
+        in_frame_split.close()
+        _shutil_rmtree_retry(in_frame_path)
+        gc.collect()
 
     @classmethod
     def create_and_upload_data_embs(
         cls, df: DataFrame, split: str, epoch_or_inf: str
     ) -> None:
         """Uploads off the shelf data embeddings for a split"""
         object_store = ObjectStore()
         df_copy = df.copy()
-        # Create
-        data_embs = create_data_embs(df_copy)
+        try:
+            data_embs = create_data_embs_df(df_copy)
+        except HfHubHTTPError as e:
+            warnings.warn(
+                "Unable to download transformer from huggingface. Data embeddings "
+                f"will be skipped. {str(e)}"
+            )
+            return
         proj_run_split = f"{config.current_project_id}/{config.current_run_id}/{split}"
-        minio_file = f"{proj_run_split}/{epoch_or_inf}/data_emb/data_emb.hdf5"
+        minio_file = f"{proj_run_split}/{epoch_or_inf}/{DATA_EMB_PATH}"
         # And upload
         object_store.create_project_run_object_from_df(data_embs, minio_file)
 
     def convert_large_string(self, df: DataFrame) -> DataFrame:
         """Cast regular string to large_string for the text column
 
         Arrow strings have a max size of 2GB, so in order to export to hdf5 and
         join the strings in the text column, we upcast to a large string.
 
         We only do this for types that write to HDF5 files
         """
         df_copy = df.copy()
+        if "text" not in df_copy.get_column_names():
+            return df_copy
         # Characters are each 1 byte. If more bytes > max, it needs to be large_string
         text_bytes = df_copy["text"].str.len().sum()
         if text_bytes > self.STRING_MAX_SIZE_B:
-            df_copy["text"] = df_copy["text"].to_arrow().cast(pa.large_string())
+            df_copy["text"] = df_copy['astype(text, "large_string")']
         return df_copy
 
     @classmethod
-    def upload_split(
+    def upload_split_from_in_frame(
         cls,
         object_store: ObjectStore,
         in_frame: DataFrame,
         split: str,
         split_loc: str,
         last_epoch: Optional[int] = None,
         create_data_embs: bool = False,
     ) -> None:
-        # If set, last_epoch will only let you upload to and including the provided
-        # epoch value, nothing more.
-        # If None, then slicing a list [:None] will include all values
         epochs_or_infs = os.listdir(split_loc)
         epochs_or_infs = sorted(
             epochs_or_infs, key=lambda i: int(i) if split != Split.inference else i
         )
         # last_epoch is inclusive
         last_epoch = last_epoch + 1 if last_epoch else last_epoch
+        # If set, last_epoch will only let you upload to and including the provided
+        # epoch value, nothing more.
+        # If None, then slicing a list [:None] will include all values
         epochs_or_infs = epochs_or_infs[:last_epoch]
 
         largest_epoch = epochs_or_infs[-1]
 
         # For each inference name or epoch of the given split
         for epoch_or_inf in tqdm(
             epochs_or_infs,
             total=len(epochs_or_infs),
             desc=split,
             file=sys.stdout,
         ):
             input_batch = in_frame.copy()
-            prob_only = cls.prob_only(epochs_or_infs, split, epoch_or_inf)
+            prob_only = cls.prob_only(epochs_or_infs, split, epoch_or_inf, last_epoch)
             if split == Split.inference:
                 input_batch = filter_df(input_batch, "inference_name", epoch_or_inf)
                 if not len(input_batch):
                     warnings.warn(
                         "There was output data logged for inference_name "
                         f"{epoch_or_inf} but no input data logged. Skipping upload for "
                         "this inference run as there are no samples to join to.",
@@ -292,140 +400,148 @@
     def create_in_out_frames(
         cls,
         in_frame: DataFrame,
         dir_name: str,
         prob_only: bool,
         split: str,
         epoch_or_inf: Union[str, int],
-    ) -> BaseLoggerInOutFrames:
+    ) -> BaseLoggerDataFrames:
         """Formats the input data and model output data
 
         In this step, we concatenate the many hdf5 files created during model training
         and logging. We log those in threaded processes, and here we combine them
         into a single hdf5 file that vaex can read into a dataframe
 
         :param in_frame: the input dataframe
         :param dir_name: The directory of all of the output hdf5 files
         :param prob_only: If we are only uploading probability data. We only upload
             probability data for all epochs except the last one (we dont use cross-epoch
             embeddings currently, so we dont log them)
         :param split: The split we are logging for
         :param epoch_or_inf: The epoch or inference name we are logging for
         """
-        str_cols = concat_hdf5_files(dir_name, prob_only)
-        out_frame = vaex.open(f"{dir_name}/{HDF5_STORE}")
-
-        if split == Split.inference:
-            dtype: Union[str, None] = "str"
-            epoch_or_inf_name = "inference_name"
-        else:
-            dtype = None
-            epoch_or_inf_name = "epoch"
-
-        # Post concat, string columns come back as bytes and need conversion
-        for col in str_cols:
-            out_frame[col] = out_frame[col].to_arrow().cast(pa.large_string())
-        if prob_only:
-            out_frame["split"] = vaex.vconstant(
-                split, length=len(out_frame), dtype="str"
-            )
-            out_frame[epoch_or_inf_name] = vaex.vconstant(
-                epoch_or_inf, length=len(out_frame), dtype=dtype
-            )
-
+        out_frame = get_output_df(dir_name, prob_only, split, epoch_or_inf)
+        epoch_or_inf_name = "inference_name" if split == Split.inference else "epoch"
         return cls.process_in_out_frames(
             in_frame, out_frame, prob_only, epoch_or_inf_name, split
         )
 
     @classmethod
     def process_in_out_frames(
         cls,
         in_frame: DataFrame,
         out_frame: DataFrame,
         prob_only: bool,
         epoch_or_inf_name: str,
         split: str,
-    ) -> BaseLoggerInOutFrames:
+    ) -> BaseLoggerDataFrames:
         """Processes input and output dataframes from logging
 
         Validates uniqueness of IDs in the output dataframe
         Joins inputs and outputs
         Splits the dataframes into prob, emb, and data for uploading to minio
 
         :param in_frame: The input dataframe
         :param out_frame: The model output dataframe
         :param prob_only: If we are only uploading probabilities, or everything
         :param epoch_or_inf_name: The epoch or inference name we are uploading for
         """
         validate_unique_ids(out_frame, epoch_or_inf_name)
-        in_out = _join_in_out_frames(in_frame, out_frame)
+        allow_missing_in_df_ids = cls.logger_config.dataloader_random_sampling
+
+        in_out = _join_in_out_frames(
+            in_frame, out_frame, allow_missing_in_df_ids=allow_missing_in_df_ids
+        )
 
-        prob, emb, data_df = cls.split_dataframe(in_out, prob_only, split)
+        dataframes = cls.separate_dataframe(in_out, prob_only, split)
         # These df vars will be used in upload_in_out_frames
-        emb.set_variable("skip_upload", prob_only)
-        data_df.set_variable("skip_upload", prob_only)
+        dataframes.emb.set_variable("skip_upload", prob_only)
+        dataframes.data.set_variable("skip_upload", prob_only)
         epoch_inf_val = out_frame[[epoch_or_inf_name]][0][0]
-        prob.set_variable("progress_name", str(epoch_inf_val))
+        dataframes.prob.set_variable("progress_name", str(epoch_inf_val))
 
-        return BaseLoggerInOutFrames(prob=prob, emb=emb, data=data_df)
+        return dataframes
 
     @classmethod
     def upload_in_out_frames(
         cls,
         object_store: ObjectStore,
-        in_out_frames: BaseLoggerInOutFrames,
+        in_out_frames: BaseLoggerDataFrames,
         split: str,
         epoch_or_inf: Union[str, int],
     ) -> None:
         proj_run = f"{config.current_project_id}/{config.current_run_id}"
 
         prob = in_out_frames.prob
         emb = in_out_frames.emb
         data_df = in_out_frames.data
 
         epoch_inf = prob.variables.pop(DFVar.progress_name, "")
 
         name = "inf_name" if split == Split.inference else "epoch"
         desc = f"{split} ({name}={epoch_inf})"
+
         for data_folder, df_obj in tqdm(
             zip(DATA_FOLDERS, [emb, prob, data_df]),
             total=3,
             desc=desc,
             leave=False,
             file=sys.stdout,
         ):
             if df_obj.variables.get(DFVar.skip_upload):
                 continue
-
             ext = cls.DATA_FOLDER_EXTENSION[data_folder]
             minio_file = (
                 f"{proj_run}/{split}/{epoch_or_inf}/{data_folder}/{data_folder}.{ext}"
             )
+            cls._handle_numpy_types(df=df_obj)
             object_store.create_project_run_object_from_df(
                 df=df_obj, object_name=minio_file
             )
 
     @classmethod
+    def _handle_numpy_types(cls, df: DataFrame) -> None:
+        """Casts everything to float/int 32"""
+        for col, dt in zip(df.get_column_names(), df.dtypes):
+            if dt == "float" and dt != "float32":
+                df[col] = df[col].astype("float32")
+            elif dt == "int" and dt != "int32":
+                df[col] = df[col].astype("int32")
+
+    @classmethod
     def prob_only(
-        cls, epochs: List[str], split: str, epoch_or_inf_name: Union[int, str]
+        cls,
+        epochs: List[str],
+        split: str,
+        epoch_or_inf_name: Union[int, str],
+        last_epoch: Optional[int],
     ) -> bool:
         """Determines if we are only uploading probabilities
 
         For all epochs that aren't the last 2 (early stopping), we only want to
         upload the probabilities (for DEP calculation).
         """
         if split == Split.inference:  # Inference doesn't have DEP
             return False
 
         # If split is not inference, epoch_or_inf must be epoch
         epoch = int(epoch_or_inf_name)
         max_epoch_for_split = max([int(i) for i in epochs])
+        if last_epoch is not None:
+            max_epoch_for_split = min(max_epoch_for_split, last_epoch)
         return bool(epoch < max_epoch_for_split - 1)
 
-    def validate(self) -> None:
+    def validate_and_format(self) -> None:
+        """Validates the logger
+
+        Ensures that self.split is set, or sets it to the current split
+        from the logger_config.
+
+        Each child also defines an additional validate method that is called
+        """
         self.set_split_epoch()
 
     @classmethod
     @abstractmethod
     def validate_labels(cls) -> None:
         ...
 
@@ -436,16 +552,16 @@
                 f"The first {self.MAX_META_COLS} will be logged only.",
                 GalileoWarning,
             )
         # When logging metadata columns, if the user breaks a rule, don't fail
         # completely, just warn them and remove that metadata column
         # Cast to list for in-place dictionary mutation
         reserved_keys = BaseLoggerAttributes.get_valid()
-        valid_meta = {}
-        for key, values in list(self.meta.items())[: self.MAX_META_COLS]:
+        valid_meta_cols = []
+        for key, values in list(self.meta.items()):
             # Key must not override a default
             if key in reserved_keys:
                 warnings.warn(
                     f"Metadata column names must not override default values "
                     f"{reserved_keys}. Metadata field {key} "
                     f"will be removed.",
                     GalileoWarning,
@@ -466,30 +582,61 @@
                     f"Expected {batch_size} values for key {key} but got "
                     f"{len(values)}. Will not log this metadata column.",
                     GalileoWarning,
                 )
                 continue
             # Values must be a point, not an iterable
             valid_types = (str, int, float, np.floating, np.integer)
-            invalid_values = filter(
-                lambda t: not isinstance(t, valid_types)
-                or (isinstance(t, str) and len(t) > self.MAX_STR_LEN),
-                values,
-            )
+            invalid_values = filter(lambda t: not isinstance(t, valid_types), values)
             bad_val = next(invalid_values, None)
             if bad_val:
                 warnings.warn(
                     f"Metadata column {key} has one or more invalid values {bad_val} "
-                    f"of type {type(bad_val)}. Only strings of "
-                    f"len < {self.MAX_STR_LEN} and numbers can be logged.",
+                    f"of type {type(bad_val)}.",
                     GalileoWarning,
                 )
                 continue
-            valid_meta[key] = values
-        self.meta = valid_meta
+            valid_meta_cols.append(key)
+
+        def valid_str_col(df: DataFrame, key: str) -> bool:
+            """Valid str col checks length of longest str in metadata col"""
+            if df[key].dtype != "string":
+                return True
+
+            max_str_len = df[key].str.len().max()
+            if max_str_len > self.MAX_DOC_LEN:
+                warnings.warn(
+                    f"Metadata column {key} has one or more strings that are longer "
+                    f"than max document length of {self.MAX_DOC_LEN} characters. "
+                    "Will not log this metadata column.",
+                    GalileoWarning,
+                )
+                return False
+            if max_str_len > self.MAX_STR_LEN:
+                if len(self.logger_config.metadata_documents) >= self.LIMIT_NUM_DOCS:
+                    warnings.warn(
+                        "You have already logged limit of 3 document columns. A "
+                        "document column is a column that has max str length between"
+                        f"1,000 and 10,000 characters. Metadata column {key} has one "
+                        f"or more strings that are longer than {self.MAX_STR_LEN} "
+                        "characters. Will not log this metadata column.",
+                        GalileoWarning,
+                    )
+                    return False
+                else:
+                    self.logger_config.metadata_documents.add(key)
+
+            return True
+
+        df: DataFrame = vaex.from_dict(
+            {k: v for k, v in self.meta.items() if k in valid_meta_cols}
+        )
+        valid_meta_cols = [k for k in valid_meta_cols if valid_str_col(df, k)]
+        valid_meta_cols = valid_meta_cols[: self.MAX_META_COLS]  # Take first 25
+        self.meta = {k: v for k, v in self.meta.items() if k in valid_meta_cols}
 
     @staticmethod
     def get_data_logger_attr(cls: object) -> str:
         """
         Returns the attribute that corresponds to the logger in the class.
         This assumes only 1 logger object exists in the class
 
@@ -500,17 +647,17 @@
             member_class = getattr(cls, attr)
             if isinstance(member_class, BaseGalileoDataLogger):
                 return attr
         raise AttributeError("No data logger attribute found!")
 
     @classmethod
     @abstractmethod
-    def split_dataframe(
-        cls, df: DataFrame, prob_only: bool, split: str
-    ) -> Tuple[DataFrame, DataFrame, DataFrame]:
+    def separate_dataframe(
+        cls, df: DataFrame, prob_only: bool = False, split: Optional[str] = None
+    ) -> BaseLoggerDataFrames:
         ...
 
     def validate_kwargs(self, kwargs: Dict) -> None:
         """Raises if a function that shouldn't get kwargs gets any"""
         if kwargs.keys():
             raise GalileoException(f"Unexpected arguments: {tuple(kwargs.keys())}")
 
@@ -520,20 +667,24 @@
 
     @classmethod
     def set_tagging_schema(cls, tagging_schema: TaggingSchema) -> None:
         """Sets the tagging schema, if applicable. Must be implemented by child"""
         raise GalileoException(f"Cannot set tagging schema for {cls.__logger_name__}")
 
     def validate_data_size(self, df: DataFrame) -> None:
+        """Validates that the data size is within the limits of Galileo Cloud
+
+        If the data size is too large, a warning is raised.
+        """
         if not is_galileo_cloud():
             return
         samples_logged = len(df)
-        path_to_logged_data = f"{self.input_data_path()}/*/*arrow"
+        path_to_logged_data = f"{self.input_data_path}/*/*arrow"
         if glob.glob(path_to_logged_data):
-            samples_logged += len(vaex.open(f"{self.input_data_path()}/*/*arrow"))
+            samples_logged += len(vaex.open(f"{self.input_data_path}/*/*arrow"))
         nrows = BaseGalileoDataLogger.MAX_DATA_SIZE_CLOUD
         if samples_logged > nrows:
             warnings.warn(
                 f"⚠️ Hey there! You've logged over {nrows} rows in your input data. "
                 f"Galileo Cloud only supports up to {nrows} rows. "
                 "If you are using larger datasets, you may see degraded performance. "
                 "Please email us at team@rungalileo.io if you have any questions.",
```

### Comparing `dataquality-0.8.9/dataquality/loggers/data_logger/text_classification.py` & `dataquality-0.9.0a0/dataquality/loggers/data_logger/text_classification.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 from collections import defaultdict
 from enum import Enum, unique
-from typing import Any, DefaultDict, Dict, Iterable, List, Optional, Tuple, Union
+from typing import Any, DefaultDict, Dict, Iterable, List, Optional, Union, cast
 
 import numpy as np
 import pandas as pd
 import vaex
+from datasets import ClassLabel
 from vaex.dataframe import DataFrame
 
+import dataquality
 from dataquality.exceptions import GalileoException
 from dataquality.loggers.data_logger.base_data_logger import (
     ITER_CHUNK_SIZE,
     BaseGalileoDataLogger,
     DataSet,
     MetasType,
     MetaType,
 )
 from dataquality.loggers.logger_config.text_classification import (
     text_classification_logger_config,
 )
 from dataquality.schemas import __data_schema_version__
+from dataquality.schemas.dataframe import BaseLoggerDataFrames
 from dataquality.schemas.split import Split
+from dataquality.utils.auto import add_class_label_to_dataset
 from dataquality.utils.vaex import rename_df
 
 
 @unique
 class GalileoDataLoggerAttributes(str, Enum):
     texts = "texts"
     labels = "labels"
@@ -71,20 +75,20 @@
     """
 
     __logger_name__ = "text_classification"
     logger_config = text_classification_logger_config
 
     def __init__(
         self,
-        texts: List[str] = None,
-        labels: List[str] = None,
-        ids: List[int] = None,
-        split: str = None,
-        meta: MetasType = None,
-        inference_name: str = None,
+        texts: Optional[List[str]] = None,
+        labels: Optional[List[str]] = None,
+        ids: Optional[List[int]] = None,
+        split: Optional[str] = None,
+        meta: Optional[MetasType] = None,
+        inference_name: Optional[str] = None,
     ) -> None:
         """Create data logger.
 
         :param texts: The raw text inputs for model training. List[str]
         :param labels: the ground truth labels aligned to each text field.
         List[str]
         :param ids: Optional unique indexes for each record. If not provided, will
@@ -193,15 +197,15 @@
         *,
         batch_size: int = ITER_CHUNK_SIZE,
         text: Union[str, int] = "text",
         id: Union[str, int] = "id",
         label: Optional[Union[str, int]] = "label",
         split: Optional[Split] = None,
         inference_name: Optional[str] = None,
-        meta: Optional[List[Union[str, int]]] = None,
+        meta: Union[List[str], List[int], None] = None,
         **kwargs: Any,
     ) -> None:
         """
         Log a dataset of input samples for text classification
 
         :param dataset: The dataset to log. This can be an python iterable or
             Pandas/Vaex dataframe. If an iterable, it can be a list of elements that can
@@ -217,15 +221,14 @@
         :param meta: List[str, int]: The keys/indexes of each metadata field.
             Consider a pandas dataframe, this would be the list of columns corresponding
             to each metadata field to log
         """
         self.validate_kwargs(kwargs)
         self.split = split
         self.inference_name = inference_name
-        meta = meta or []
         column_map = {text: "text", id: "id"}
         label = None if split == Split.inference else label
         if label:
             column_map[label] = "label"
         if isinstance(dataset, pd.DataFrame):
             dataset = dataset.rename(columns=column_map)
             self._log_df(dataset, meta)
@@ -250,72 +253,94 @@
 
     def _log_hf_dataset(
         self,
         dataset: Any,
         batch_size: int,
         text: Union[str, int],
         id: Union[str, int],
-        meta: List[Union[str, int]],
-        label: Union[str, int] = None,
-        split: Split = None,
-        inference_name: str = None,
+        meta: Union[List[str], List[int], None] = None,
+        label: Optional[Union[str, int]] = None,
+        split: Optional[Split] = None,
+        inference_name: Optional[str] = None,
     ) -> None:
         """Helper function to log a huggingface dataset
 
         HuggingFace datasets can be sliced, returning a dict that is in the correct
         format to log directly.
         """
 
-        parse_label = lambda x: x  # noqa: E731
-        # If label is integer, convert to string #
-
-        if isinstance(dataset[0].get(label), int):
-            try:
-                parse_label = lambda x: dataset.features[label].int2str(x)  # noqa: E731
-            except Exception:
+        def parse_label(labels: Union[List[int], List[str]]) -> List[str]:
+            # If we have 1 str, they are all strings
+            if isinstance(labels[0], str):
+                return cast(List[str], labels)
+            # Otherwise they are all ints (typing)
+            else:
+                labels = cast(List[int], labels)
+            if hasattr(dataset.features[label], "int2str"):
+                return dataset.features[label].int2str(labels)
+            elif self.logger_config.labels:
+                return [self.logger_config.labels[gt] for gt in labels]
+            elif (
+                hasattr(dataset.features[label], "names")
+                and dataset.features[label].names
+            ):
+                classes = dataset.features[label].names
+                if not self.logger_config.labels:
+                    dataquality.set_labels_for_run(classes)
+                return [classes[gt] for gt in labels]
+            else:
                 # TODO: Simplify this logic with mapping the int label to string ticket
                 raise GalileoException(
-                    "Your dataset does not have label names. Please include them"
+                    "Your dataset does not have label names. Please include them or "
+                    "call dq.set_labels_for_run"
                 )
 
         assert dataset[0].get(id) is not None, GalileoException(
             f"id ({id}) field must be present in dataset"
         )
 
+        # Make sure the class labels are set
+        if (
+            label
+            and self.logger_config.labels
+            and not isinstance(dataset.features[label], ClassLabel)
+        ):
+            dataset = add_class_label_to_dataset(dataset, self.logger_config.labels)
+
         for i in range(0, len(dataset), batch_size):
             chunk = dataset[i : i + batch_size]
             data = dict(
                 text=chunk[text],
                 id=chunk[id],
                 label=parse_label(chunk[label]) if label else None,
             )
-            chunk_meta = {col: chunk[col] for col in meta}
+            chunk_meta = {col: chunk[col] for col in meta or []}
             self._log_dict(data, chunk_meta, split, inference_name)
 
     def _log_iterator(
         self,
         dataset: Iterable,
         batch_size: int,
         text: Union[str, int],
         id: Union[str, int],
-        meta: List[Union[str, int]],
-        label: Union[str, int] = None,
-        split: Split = None,
-        inference_name: str = None,
+        meta: Union[List[str], List[int], None] = None,
+        label: Optional[Union[str, int]] = None,
+        split: Optional[Split] = None,
+        inference_name: Optional[str] = None,
     ) -> None:
         batches = defaultdict(list)
         metas = defaultdict(list)
         for chunk in dataset:
             batches["text"].append(self._convert_tensor_to_py(chunk[text]))
             batches["id"].append(self._convert_tensor_to_py(chunk[id]))
             if label:
                 # Process separately because multi-label needs to override this
                 # to handle labels as a list of lists
                 batches = self._process_label(batches, chunk[label])
-            for meta_col in meta:
+            for meta_col in meta or []:
                 metas[meta_col].append(self._convert_tensor_to_py(chunk[meta_col]))
 
             if len(batches["text"]) >= batch_size:
                 self._log_dict(batches, metas, split, inference_name)
                 batches.clear()
                 metas.clear()
         # in case there are any left
@@ -324,61 +349,66 @@
 
     def _process_label(self, batches: DefaultDict, label: Any) -> DefaultDict:
         """Process label for text-classification and multi-label accordingly"""
         batches["label"].append(self._convert_tensor_to_py(label))
         return batches
 
     def _log_dict(
-        self, d: Dict, meta: Dict, split: Split = None, inference_name: str = None
+        self,
+        d: Dict,
+        meta: Dict,
+        split: Optional[Split] = None,
+        inference_name: Optional[str] = None,
     ) -> None:
         self.log_data_samples(
             texts=d["text"],
             labels=d["label"],
             ids=d["id"],
             split=split,
             inference_name=inference_name,
             meta=meta,
         )
 
     def _log_df(
-        self, df: Union[pd.DataFrame, DataFrame], meta: List[Union[str, int]]
+        self,
+        df: Union[pd.DataFrame, DataFrame],
+        meta: Union[List[str], List[int], None] = None,
     ) -> None:
-        """Helper to log a pandas or vex df"""
+        """Helper to log a pandas or vaex df"""
         self.texts = df["text"].tolist()
         self.ids = df["id"].tolist()
         # Inference case
         if "label" in df:
             self.labels = df["label"].tolist()
-        for meta_col in meta:
+        for meta_col in meta or []:
             self.meta[str(meta_col)] = df[meta_col].tolist()
         self.log()
 
     @staticmethod
     def get_valid_attributes() -> List[str]:
         """
         Returns a list of valid attributes that this logger accepts
         :return: List[str]
         """
         return GalileoDataLoggerAttributes.get_valid()
 
-    def validate(self) -> None:
+    def validate_and_format(self) -> None:
         """
         Validates that the current config is correct.
         * Text and Labels must both exist (unless split is 'inference' in which case
         labels must be None)
         * Text and Labels must be the same length
         * If ids exist, it must be the same length as text/labels
-        :return: None
 
         If the user logged labels as ints, convert them to the string labels.
         In the next optimization, we will support the API having int labels, but for
         now it expects string labels. When we make that change, we will do the opposite
         and always convert to the int index of the labels.
         """
-        super().validate()
+        super().validate_and_format()
         label_len = len(self.labels)
         text_len = len(self.texts)
         id_len = len(self.ids)
 
         set_labels_are_ints = self.logger_config.int_labels
 
         if self.split != Split.inference and str(self.labels[0]).isnumeric():
@@ -452,39 +482,40 @@
             **self.meta,
         )
         if self.inference_name:
             inp.update(inference_name=self.inference_name)
         return vaex.from_pandas(pd.DataFrame(inp))
 
     @classmethod
-    def split_dataframe(
-        cls, df: DataFrame, prob_only: bool, split: str
-    ) -> Tuple[DataFrame, DataFrame, DataFrame]:
-        """Splits the singular dataframe into its 3 components
+    def separate_dataframe(
+        cls, df: DataFrame, prob_only: bool = True, split: Optional[str] = None
+    ) -> BaseLoggerDataFrames:
+        """Separates the singular dataframe into its 3 components
 
         Gets the probability df, the embedding df, and the "data" df containing
         all other columns
         """
         df_copy = df.copy()
         # Separate out embeddings and probabilities into their own files
         prob_cols = cls._get_prob_cols()
         prob = df_copy[prob_cols]
 
         if prob_only:  # In this case, we don't care about the other columns
             emb_cols = ["id"]
             other_cols = ["id"]
         else:
-            emb_cols = ["id", "emb"]
-            ignore_cols = ["emb", "split_id"] + prob_cols
+            emb_cols = ["id", "emb", "x", "y", "emb_pca"]
+            emb_cols = [c for c in emb_cols if c in df_copy.get_column_names()]
+            ignore_cols = ["split_id"] + prob_cols + emb_cols
             other_cols = [i for i in df_copy.get_column_names() if i not in ignore_cols]
             other_cols += ["id"]
 
         emb = df_copy[emb_cols]
         data_df = df_copy[other_cols]
-        return prob, emb, data_df
+        return BaseLoggerDataFrames(prob=prob, emb=emb, data=data_df)
 
     @classmethod
     def _get_prob_cols(cls) -> List[str]:
         return ["id", "prob", "gold"]
 
     @classmethod
     def validate_labels(cls) -> None:
```

### Comparing `dataquality-0.8.9/dataquality/loggers/data_logger/text_multi_label.py` & `dataquality-0.9.0a0/dataquality/loggers/data_logger/text_multi_label.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,19 +67,19 @@
     __logger_name__ = "text_multi_label"
     logger_config: TextMultiLabelLoggerConfig = (
         text_multi_label_logger_config  # type: ignore
     )
 
     def __init__(
         self,
-        texts: List[str] = None,
-        labels: List[List[str]] = None,
-        ids: List[int] = None,
-        split: str = None,
-        meta: MetasType = None,
+        texts: Optional[List[str]] = None,
+        labels: Optional[List[List[str]]] = None,
+        ids: Optional[List[int]] = None,
+        split: Optional[str] = None,
+        meta: Optional[MetasType] = None,
     ) -> None:
         """Create data logger.
 
         :param text: The raw text inputs for model training. List[str]
         :param labels: the ground truth labels aligned to each text field.
         List[List[str]]
         :param ids: Optional unique indexes for each record. If not provided, will
@@ -134,16 +134,16 @@
     def log_data_samples(
         self,
         *,
         texts: List[str],
         ids: List[int],
         labels: Optional[List[str]] = None,
         split: Optional[Split] = None,
-        inference_name: str = None,
-        meta: MetasType = None,
+        inference_name: Optional[str] = None,
+        meta: Optional[MetasType] = None,
         task_labels: Optional[List[List[str]]] = None,
         **kwargs: Any,
     ) -> None:
         """Log input samples for text multi-label
 
         :param texts: List[str] text samples
         :param ids: List[int,str] IDs for each text sample
@@ -172,15 +172,19 @@
         # In binary multi-label, it will be a single string
         if self.logger_config.binary:
             return super()._process_label(batches, label)
         batches["label"].append(self._convert_tensor_ndarray(label).tolist())
         return batches
 
     def _log_dict(
-        self, d: Dict, meta: Dict, split: Split = None, inference_name: str = None
+        self,
+        d: Dict,
+        meta: Dict,
+        split: Optional[Split] = None,
+        inference_name: Optional[str] = None,
     ) -> None:
         self.log_data_samples(
             texts=d["text"],
             task_labels=d["label"],
             ids=d["id"],
             split=split,
             inference_name=inference_name,
@@ -215,24 +219,24 @@
                 if task in sample_label_set:
                     clean_sample_labels.append(task)
                 else:
                     clean_sample_labels.append(f"NOT_{task}")
             clean_task_labels.append(clean_sample_labels)
         self.labels = clean_task_labels
 
-    def validate(self) -> None:
+    def validate_and_format(self) -> None:
         """
         Parent validation (text_classification) with additional validation on labels
 
         in multi_label modeling, each element in self.labels should itself be a list
         """
         if self.logger_config.binary:
             self._process_binary_labels()
         self.logger_config.observed_num_tasks = len(self.labels[0])
-        super().validate()
+        super().validate_and_format()
 
     def validate_logged_labels(self) -> None:
         for ind, input_labels in enumerate(self.labels):
             assert isinstance(
                 input_labels, (list, np.ndarray, pd.Series)
             ), "labels must be a list of lists in multi-label tasks"
             assert len(input_labels) == self.logger_config.observed_num_tasks, (
```

### Comparing `dataquality-0.8.9/dataquality/loggers/data_logger/text_ner.py` & `dataquality-0.9.0a0/dataquality/loggers/data_logger/text_ner.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     BaseGalileoDataLogger,
     DataSet,
     MetasType,
     MetaType,
 )
 from dataquality.loggers.logger_config.text_ner import text_ner_logger_config
 from dataquality.schemas import __data_schema_version__
-from dataquality.schemas.dataframe import BaseLoggerInOutFrames, DFVar
+from dataquality.schemas.dataframe import BaseLoggerDataFrames, DFVar
 from dataquality.schemas.ner import NERColumns as NERCols
 from dataquality.schemas.ner import TaggingSchema
 from dataquality.schemas.split import Split
 from dataquality.utils.vaex import rename_df
 
 
 @unique
@@ -110,21 +110,21 @@
     DATA_FOLDER_EXTENSION = {"emb": "hdf5", "prob": "hdf5", "data": "arrow"}
 
     __logger_name__ = "text_ner"
     logger_config = text_ner_logger_config
 
     def __init__(
         self,
-        texts: List[str] = None,
-        text_token_indices: List[List[Tuple[int, int]]] = None,
-        gold_spans: List[List[Dict]] = None,
-        ids: List[int] = None,
-        split: str = None,
-        meta: MetasType = None,
-        inference_name: str = None,
+        texts: Optional[List[str]] = None,
+        text_token_indices: Optional[List[List[Tuple[int, int]]]] = None,
+        gold_spans: Optional[List[List[Dict]]] = None,
+        ids: Optional[List[int]] = None,
+        split: Optional[str] = None,
+        meta: Optional[MetasType] = None,
+        inference_name: Optional[str] = None,
     ) -> None:
         """Create data logger.
 
         :param texts: The raw text inputs for model training. List[str]
         :param text_token_indices: Token boundaries of text. List[Tuple(int, int)].
         Used to convert the gold_spans into token level spans internally.
         t[0] indicates the start index of the span and t[1] is the end index (exclusive)
@@ -155,16 +155,16 @@
         return GalileoDataLoggerAttributes.get_valid()
 
     def log_data_samples(
         self,
         *,
         texts: List[str],
         ids: List[int],
-        text_token_indices: List[List[Tuple[int, int]]] = None,
-        gold_spans: List[List[Dict]] = None,
+        text_token_indices: Optional[List[List[Tuple[int, int]]]] = None,
+        gold_spans: Optional[List[List[Dict]]] = None,
         split: Optional[Split] = None,
         inference_name: Optional[str] = None,
         meta: Optional[MetasType] = None,
         **kwargs: Any,  # For typing
     ) -> None:
         """Log input samples for text NER
 
@@ -200,16 +200,16 @@
         self.log()
 
     def log_data_sample(
         self,
         *,
         text: str,
         id: int,
-        text_token_indices: List[Tuple[int, int]] = None,
-        gold_spans: List[Dict] = None,
+        text_token_indices: Optional[List[Tuple[int, int]]] = None,
+        gold_spans: Optional[List[Dict]] = None,
         split: Optional[Split] = None,
         inference_name: Optional[str] = None,
         meta: Optional[MetaType] = None,
         **kwargs: Any,
     ) -> None:
         """
         Log a single input sample for text classification
@@ -247,15 +247,15 @@
         batch_size: int = ITER_CHUNK_SIZE,
         text: Union[str, int] = "text",
         id: Union[str, int] = "id",
         text_token_indices: Union[str, int] = "text_token_indices",
         gold_spans: Union[str, int] = "gold_spans",
         split: Optional[Split] = None,
         inference_name: Optional[str] = None,
-        meta: Optional[List[Union[str, int]]] = None,
+        meta: Union[List[str], List[int], None] = None,
         **kwargs: Any,
     ) -> None:
         """
         Log a dataset of input samples for NER
 
         :param dataset: The dataset to log. This can be an python iterable or
             Pandas/Vaex dataframe. If an iterable, it can be a list of elements that can
@@ -270,15 +270,14 @@
         :param meta: List[str, int]: The keys/indexes of each metadata field.
             Consider a pandas dataframe, this would be the list of columns corresponding
             to each metadata field to log
         """
         self.validate_kwargs(kwargs)
         self.split = split
         self.inference_name = inference_name
-        meta = meta or []
         column_map = {
             text: "text",
             id: "id",
             gold_spans: "gold_spans",
             text_token_indices: "text_token_indices",
         }
         if isinstance(dataset, pd.DataFrame):
@@ -323,26 +322,26 @@
         self,
         dataset: Any,
         batch_size: int,
         text: Union[str, int],
         id: Union[str, int],
         text_token_indices: Union[str, int],
         gold_spans: Union[str, int],
-        meta: List[Union[str, int]],
+        meta: Union[List[str], List[int], None] = None,
         split: Optional[Split] = None,
         inference_name: Optional[str] = None,
     ) -> None:
         """Helper function to log a huggingface dataset
 
         HuggingFace datasets can be sliced, returning a dict that is in the correct
         format to log directly.
         """
         for i in range(0, len(dataset), batch_size):
             chunk = dataset[i : i + batch_size]
-            chunk_meta: Dict = {col: chunk[col] for col in meta}
+            chunk_meta: Dict = {col: chunk[col] for col in meta or []}
             self.log_data_samples(
                 texts=chunk[text],
                 ids=chunk[id],
                 text_token_indices=chunk[text_token_indices],
                 gold_spans=chunk.get(gold_spans),
                 split=split,
                 meta=chunk_meta,
@@ -353,29 +352,29 @@
         self,
         dataset: Iterable,
         batch_size: int,
         text: Union[str, int],
         id: Union[str, int],
         text_token_indices: Union[str, int],
         gold_spans: Union[str, int],
-        meta: List[Union[str, int]],
+        meta: Union[List[str], List[int], None] = None,
         split: Optional[Split] = None,
         inference_name: Optional[str] = None,
     ) -> None:
         batches = defaultdict(list)
         metas = defaultdict(list)
         for chunk in dataset:
             batches["text"].append(chunk[text])
             batches["text_token_indices"].append(chunk[text_token_indices])
             batches["id"].append(chunk[id])
 
             if split != Split.inference:
                 batches["gold_spans"].append(chunk[gold_spans])
 
-            for meta_col in meta:
+            for meta_col in meta or []:
                 metas[meta_col].append(self._convert_tensor_to_py(chunk[meta_col]))
 
             if len(batches["text"]) >= batch_size:
                 self._log_dict(batches, metas, split)
                 batches.clear()
                 metas.clear()
 
@@ -397,35 +396,36 @@
             gold_spans=d.get("gold_spans"),
             split=split,
             meta=meta,
             inference_name=inference_name,
         )
 
     def _log_df(
-        self, df: Union[pd.DataFrame, DataFrame], meta: List[Union[str, int]]
+        self,
+        df: Union[pd.DataFrame, DataFrame],
+        meta: Union[List[str], List[int], None] = None,
     ) -> None:
         """Helper to log a pandas or vaex df"""
         self.texts = df["text"].tolist()
         self.ids = df["id"].tolist()
         self.text_token_indices = df["text_token_indices"].tolist()
         self.gold_spans = df["gold_spans"].tolist() if "gold_spans" in df else []
-        for meta_col in meta:
+        for meta_col in meta or []:
             self.meta[str(meta_col)] = df[meta_col].tolist()
         self.log()
 
-    def validate(self) -> None:
+    def validate_and_format(self) -> None:
         """
         Validates that the current config is correct.
         * Text and Labels must both exist (unless split is 'inference' in which case
         gold_spans must be None)
         * Text and Labels must be the same length
         * If ids exist, it must be the same length as text/labels
-        :return: None
         """
-        super().validate()
+        super().validate_and_format()
         assert self.logger_config.labels, (
             "You must set your labels before logging input data. "
             "See dataquality.set_labels_for_run"
         )
 
         assert self.logger_config.tagging_schema, (
             "You must set your tagging schema before logging input data. "
@@ -461,14 +461,16 @@
 
             assert text_len == text_tokenized_len == gold_span_len, (
                 f"gold spans, text, and tokenized text must be the same length for "
                 f"split {self.split}, but got (gold spans, text, text_token) "
                 f"({gold_span_len},{text_len},{text_tokenized_len})"
             )
 
+        self.text_token_indices_flat = []
+
         for sample_id, sample_spans, sample_indices, sample_text in zip(
             self.ids,
             self.gold_spans or [None] * id_len,  # type: ignore
             self.text_token_indices,
             self.texts,
         ):
             sample_key = self.logger_config.get_sample_key(Split(self.split), sample_id)
@@ -615,34 +617,36 @@
     def process_in_out_frames(
         cls,
         in_frame: DataFrame,
         out_frame: DataFrame,
         prob_only: bool,
         epoch_or_inf_name: str,
         split: str,
-    ) -> BaseLoggerInOutFrames:
+    ) -> BaseLoggerDataFrames:
         """Processes input and output dataframes from logging
 
         NER is a different case where the input data is logged at the sample level,
         but output data is logged at the span level, so we need to process it
         differently
 
         We don't have span IDs so we don't need to validate uniqueness
         We don't join the input and output frames
         We do need to split take only the rows from in_frame from this split
         Splits the dataframes into prob, emb, and input data for uploading to minio
         """
         cls._validate_duplicate_spans(out_frame, epoch_or_inf_name)
-        prob, emb, _ = cls.split_dataframe(out_frame, prob_only, split)
+        dataframes = cls.separate_dataframe(out_frame, prob_only, split)
+        # For NER data is the input data
+        dataframes.data = in_frame
         # These df vars will be used in upload_in_out_frames
-        emb.set_variable(DFVar.skip_upload, prob_only)
-        in_frame.set_variable(DFVar.skip_upload, prob_only)
+        dataframes.emb.set_variable(DFVar.skip_upload, prob_only)
+        dataframes.data.set_variable(DFVar.skip_upload, prob_only)
         epoch_inf_val = out_frame[[epoch_or_inf_name]][0][0]
-        prob.set_variable(DFVar.progress_name, str(epoch_inf_val))
-        return BaseLoggerInOutFrames(prob=prob, emb=emb, data=in_frame)
+        dataframes.prob.set_variable(DFVar.progress_name, str(epoch_inf_val))
+        return dataframes
 
     @classmethod
     def _validate_duplicate_spans(cls, df: DataFrame, epoch_or_inf_name: str) -> None:
         """Validates that duplicate spans aren't logged for an input sample
 
         Duplicate spans would be spans in a sample with identical start and end spans
         """
@@ -653,17 +657,17 @@
             raise GalileoException(
                 "It seems as though you have duplicate spans for samples in this "
                 f"split. (split:{split}, {epoch_or_inf_name}:{epoch_or_inf_value}),"
                 f"dups:\n {dup_counts[['sample_id', 'count']].to_records()}"
             )
 
     @classmethod
-    def split_dataframe(
-        cls, df: DataFrame, prob_only: bool, split: str
-    ) -> Tuple[DataFrame, DataFrame, DataFrame]:
+    def separate_dataframe(
+        cls, df: DataFrame, prob_only: bool = True, split: Optional[str] = None
+    ) -> BaseLoggerDataFrames:
         """Splits the dataframe into logical grouping for minio storage
 
         NER is a different case, where we store the text samples as "data" and
         all of the span level data is split into only "emb" and "prob". This function
         will only return 2 modified dataframes, where the third is expected to be the
         input data logged by the user
         """
@@ -692,16 +696,20 @@
                 NERCols.galileo_error_type.value,
             ]
 
         prob = df_copy[prob_cols]
         emb_cols = (
             [NERCols.id.value] if prob_only else [NERCols.id.value, NERCols.emb.value]
         )
+        # In the event that we did dimensionality reduction locally with nvidia
+        for col in ["x", "y", "emb_pca"]:
+            if col in df_copy.get_column_names():
+                emb_cols.append(col)
         emb = df_copy[emb_cols]
-        return prob, emb, df_copy
+        return BaseLoggerDataFrames(prob=prob, emb=emb, data=df_copy)
 
     @classmethod
     def validate_labels(cls) -> None:
         """Validates and cleans labels, see _clean_labels and saves ner_labels
 
         ner_labels are all of the labels that start with a tag (B-, I-, E- etc) as well
         as the O tag
@@ -775,14 +783,19 @@
             or label.startswith("U-")
         )
 
     @classmethod
     def set_tagging_schema(cls, tagging_schema: TaggingSchema) -> None:
         cls.logger_config.tagging_schema = tagging_schema
 
+    @property
+    def support_data_embs(self) -> bool:
+        """Not yet supported for NER. Coming soon!"""
+        return False
+
     @classmethod
     def create_and_upload_data_embs(
         cls, df: DataFrame, split: str, epoch_or_inf: str
     ) -> None:
         """Not yet supported for NER. Coming soon!"""
         warnings.warn(
             "Data embeddings are not yet supported for NER. Coming soon!",
```

### Comparing `dataquality-0.8.9/dataquality/loggers/logger_config/base_logger_config.py` & `dataquality-0.9.0a0/dataquality/loggers/logger_config/base_logger_config.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from collections import defaultdict
-from typing import Any, DefaultDict, Dict, List, Optional, Set
+from typing import Any, Callable, DefaultDict, Dict, List, Optional, Set
 
 from pydantic import BaseModel, validator
 
 from dataquality.schemas.condition import Condition
 from dataquality.schemas.ner import TaggingSchema
 from dataquality.schemas.split import Split
 
@@ -27,14 +27,20 @@
     input_data_logged: DefaultDict[str, int] = defaultdict(int)
     logged_input_ids: DefaultDict[str, Set] = defaultdict(set)
     idx_to_id_map: DefaultDict[str, List] = defaultdict(list)
     conditions: List[Condition] = []
     report_emails: List[str] = []
     ner_labels: List[str] = []
     int_labels: bool = False
+    feature_names: List[str] = []
+    metadata_documents: Set = set()  # A document is a large str > 1k chars < 10k chars
+    finish: Callable = lambda: None  # Overwritten in Semantic Segmentation
+    # True when calling `init` with a run that already exists
+    existing_run: bool = False
+    dataloader_random_sampling = False
 
     class Config:
         validate_assignment = True
 
     def reset(self, factory: bool = False) -> None:
         """Reset all class vars"""
         self.__init__()  # type: ignore
```

### Comparing `dataquality-0.8.9/dataquality/loggers/logger_config/text_classification.py` & `dataquality-0.9.0a0/dataquality/loggers/logger_config/text_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.9/dataquality/loggers/logger_config/text_multi_label.py` & `dataquality-0.9.0a0/dataquality/loggers/logger_config/text_multi_label.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.9/dataquality/loggers/logger_config/text_ner.py` & `dataquality-0.9.0a0/dataquality/loggers/logger_config/text_ner.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.9/dataquality/loggers/model_logger/base_model_logger.py` & `dataquality-0.9.0a0/dataquality/loggers/model_logger/base_model_logger.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,27 +12,27 @@
 from dataquality.exceptions import GalileoException, GalileoWarning, LogBatchError
 from dataquality.loggers.base_logger import BaseGalileoLogger
 from dataquality.loggers.data_logger import BaseGalileoDataLogger
 from dataquality.schemas.split import Split
 from dataquality.schemas.task_type import TaskType
 from dataquality.utils.ampli import AmpliMetric
 from dataquality.utils.dq_logger import get_dq_logger
+from dataquality.utils.hdf5_store import _save_hdf5_file
 from dataquality.utils.thread_pool import ThreadPoolManager
-from dataquality.utils.vaex import _save_hdf5_file
 
 analytics = Analytics(ApiClient, config)  # type: ignore
 
 
 class BaseGalileoModelLogger(BaseGalileoLogger):
     def __init__(
         self,
-        embs: Union[List, np.ndarray] = None,
-        probs: Union[List, np.ndarray] = None,
-        logits: Union[List, np.ndarray] = None,
-        ids: Union[List, np.ndarray] = None,
+        embs: Optional[Union[List, np.ndarray]] = None,
+        probs: Optional[Union[List, np.ndarray]] = None,
+        logits: Optional[Union[List, np.ndarray]] = None,
+        ids: Optional[Union[List, np.ndarray]] = None,
         split: str = "",
         epoch: Optional[int] = None,
         inference_name: Optional[str] = None,
     ) -> None:
         super().__init__()
         # Need to compare to None because they may be np arrays which cannot be
         # evaluated with bool directly
@@ -51,15 +51,15 @@
         (something is wrong)
 
         If validation fails with a LogBatchError, we simply warn and skip logging this
         batch, but do not halt model training
         (this batch is bad, but we can continue logging)
         """
         try:
-            self.validate()
+            self.validate_and_format()
         except AssertionError as e:
             get_dq_logger().error(
                 "Validation of data failed", split=self.split, epoch=self.epoch
             )
             raise GalileoException(
                 f"The provided logged data is invalid: {e}"
             ) from None
@@ -95,53 +95,36 @@
     def log(self) -> None:
         """The top level log function that try/excepts its child"""
         self.check_for_logging_failures()
         # We validate split and epoch before entering the thread because we reference
         # global variables (cur_split and cur_epoch) that are subject to change
         # between subsequent threads
         self.set_split_epoch()
-        get_dq_logger().debug(
-            "Starting logging process from thread", split=self.split, epoch=self.epoch
-        )
         ThreadPoolManager.add_thread(target=self._add_threaded_log)
 
     def write_model_output(self, data: Dict) -> None:
         """Creates an hdf5 file from the data dict"""
-        get_dq_logger().debug(
-            "Writing model output", split=self.split, epoch=self.epoch
-        )
         location = (
             f"{self.LOG_FILE_DIR}/{config.current_project_id}"
             f"/{config.current_run_id}"
         )
         split = data["split"][0]
 
         if split == Split.inference:
             inference_name = data["inference_name"][0]
             path = f"{location}/{split}/{inference_name}"
         else:
             epoch = data["epoch"][0]
             path = f"{location}/{split}/{epoch}"
 
         object_name = f"{str(uuid4()).replace('-', '')[:12]}.hdf5"
-        get_dq_logger().debug("Saving hdf5 file", split=self.split)
         _save_hdf5_file(path, object_name, data)
 
     def set_split_epoch(self) -> None:
         super().set_split_epoch()
-        # Inference split must have inference name
-        if self.split == Split.inference and self.inference_name is None:
-            if self.logger_config.cur_inference_name is not None:
-                self.inference_name = self.logger_config.cur_inference_name
-            else:
-                raise GalileoException(
-                    "For inference split you must either log an inference name "
-                    "or set it before logging. Use `dataquality.set_split` to set"
-                    "inference_name"
-                )
 
         # Non-inference split must have an epoch
         if self.split != Split.inference and self.epoch is None:
             if self.logger_config.cur_epoch is not None:
                 self.epoch = self.logger_config.cur_epoch
             else:
                 raise GalileoException(
@@ -188,13 +171,16 @@
         self, sample_logits: Union[List[np.ndarray], np.ndarray]
     ) -> np.ndarray:
         """Converts logits to probs via softmax"""
         # axis ensures that in a matrix of probs with dims num_samples x num_classes
         # we take the softmax for each sample
         if not isinstance(sample_logits, np.ndarray):
             sample_logits = self._convert_tensor_ndarray(sample_logits)
-        if len(sample_logits.shape) == 1 or sample_logits.shape[1] == 1:
+
+        # If shape is (num_samples, 1) or (num_samples,) then we have a binary case
+        if len(sample_logits.shape) == 1 or sample_logits.shape[-1] == 1:
             if len(sample_logits.shape) > 1:
                 # Remove final empty dimension if it's there
                 sample_logits = sample_logits.reshape(-1)
             return self.convert_logits_to_prob_binary(sample_logits)
+
         return softmax(np.array(sample_logits), axis=-1)
```

### Comparing `dataquality-0.8.9/dataquality/loggers/model_logger/text_classification.py` & `dataquality-0.9.0a0/dataquality/loggers/model_logger/text_classification.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import warnings
 from enum import Enum, unique
 from typing import Any, Dict, List, Optional, Union
 
 import numpy as np
 
 from dataquality.loggers.logger_config.text_classification import (
     text_classification_logger_config,
@@ -71,18 +70,18 @@
     """
 
     __logger_name__ = "text_classification"
     logger_config = text_classification_logger_config
 
     def __init__(
         self,
-        embs: Union[List, np.ndarray] = None,
-        probs: Union[List, np.ndarray] = None,
-        logits: Union[List, np.ndarray] = None,
-        ids: Union[List, np.ndarray] = None,
+        embs: Optional[Union[List, np.ndarray]] = None,
+        probs: Optional[Union[List, np.ndarray]] = None,
+        logits: Optional[Union[List, np.ndarray]] = None,
+        ids: Optional[Union[List, np.ndarray]] = None,
         split: str = "",
         epoch: Optional[int] = None,
         inference_name: Optional[str] = None,
     ) -> None:
         super().__init__(
             embs=embs,
             probs=probs,
@@ -111,40 +110,36 @@
         """
         try:
             has_len = len(arr) != 0
         except TypeError:
             has_len = bool(arr.shape[0])
         return has_len
 
-    def validate(self) -> None:
+    def validate_and_format(self) -> None:
         """
         Validates that the current config is correct.
         * embs, probs, and ids must exist and be the same length
         :return:
         """
-        get_dq_logger().debug("Handling logits and probs", split=self.split)
         has_logits = self._has_len(self.logits)
         has_probs = self._has_len(self.probs)
         if has_logits:
             self.logits = self._convert_tensor_ndarray(self.logits, "Prob")
             self.probs = self.convert_logits_to_probs(self.logits)
             del self.logits
         elif has_probs:
-            warnings.warn("Usage of probs is deprecated, use logits instead")
             self.probs = self._convert_tensor_ndarray(self.probs, "Prob")
 
-        get_dq_logger().debug("Converting inputs to numpy arrays", split=self.split)
         self.embs = self._convert_tensor_ndarray(self.embs, "Embedding")
         self.ids = self._convert_tensor_ndarray(self.ids)
 
         embs_len = len(self.embs)
         probs_len = len(self.probs)
         ids_len = len(self.ids)
 
-        get_dq_logger().debug("Validating embedding shape", split=self.split)
         assert self.embs.ndim == 2, "Only one embedding vector is allowed per input."
 
         assert embs_len and probs_len and ids_len, (
             f"All of emb, probs, and ids for your logger must be set, but "
             f"got emb:{bool(embs_len)}, probs:{bool(probs_len)}, ids:{bool(ids_len)}"
         )
```

### Comparing `dataquality-0.8.9/dataquality/loggers/model_logger/text_multi_label.py` & `dataquality-0.9.0a0/dataquality/loggers/model_logger/text_multi_label.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,39 +58,39 @@
     __logger_name__ = "text_multi_label"
     logger_config: TextMultiLabelLoggerConfig = (
         text_multi_label_logger_config  # type: ignore
     )
 
     def __init__(
         self,
-        embs: Union[List, np.ndarray] = None,
-        probs: Union[List[List[List]], List[np.ndarray]] = None,
-        logits: Union[List[List[List]], List[np.ndarray]] = None,
-        ids: Union[List, np.ndarray] = None,
+        embs: Optional[Union[List, np.ndarray]] = None,
+        probs: Optional[Union[List[List[List]], List[np.ndarray]]] = None,
+        logits: Optional[Union[List[List[List]], List[np.ndarray]]] = None,
+        ids: Optional[Union[List, np.ndarray]] = None,
         split: str = "",
         epoch: Optional[int] = None,
         inference_name: Optional[str] = None,
     ) -> None:
         super().__init__(
             embs=embs,
             probs=probs,
             logits=logits,
             ids=ids,
             split=split,
             epoch=epoch,
             inference_name=inference_name,
         )
 
-    def validate(self) -> None:
+    def validate_and_format(self) -> None:
         """
         Validates that the current config is correct.
         * embs, probs, and ids must exist and be the same length
         :return:
         """
-        super().validate()
+        super().validate_and_format()
         for ind, probs_per_task in enumerate(self.probs):
             assert len(probs_per_task) == self.logger_config.observed_num_tasks, (
                 f"Expected {self.logger_config.observed_num_tasks} probability vectors "
                 f"per input (based on input data logging) but found "
                 f"{len(probs_per_task)} for input {ind}."
             )
             for task_ind, task_probs in enumerate(probs_per_task):
```

### Comparing `dataquality-0.8.9/dataquality/loggers/model_logger/text_ner.py` & `dataquality-0.9.0a0/dataquality/loggers/model_logger/text_ner.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-import warnings
 from collections import defaultdict
 from enum import Enum, unique
 from typing import Any, DefaultDict, Dict, List, Optional, Tuple, Union
 
 import numpy as np
 from numpy import ndarray
 
 from dataquality.exceptions import LogBatchError
 from dataquality.loggers.logger_config.text_ner import text_ner_logger_config
 from dataquality.loggers.model_logger.base_model_logger import BaseGalileoModelLogger
 from dataquality.schemas import __data_schema_version__
 from dataquality.schemas.ner import NERErrorType, NERProbMethod, TaggingSchema
 from dataquality.schemas.split import Split
-from dataquality.utils.dq_logger import get_dq_logger
 from dataquality.utils.ml import select_span_token_for_prob
 
 
 @unique
 class GalileoModelLoggerAttributes(str, Enum):
     gold_emb = "gold_emb"
     gold_spans = "gold_spans"
@@ -93,35 +91,31 @@
     """
 
     __logger_name__ = "text_ner"
     logger_config = text_ner_logger_config
 
     def __init__(
         self,
-        embs: List[np.ndarray] = None,
-        probs: List[np.ndarray] = None,
-        logits: List[np.ndarray] = None,
-        ids: Union[List, np.ndarray] = None,
+        embs: Optional[List[np.ndarray]] = None,
+        probs: Optional[List[np.ndarray]] = None,
+        logits: Optional[List[np.ndarray]] = None,
+        ids: Optional[Union[List, np.ndarray]] = None,
         split: str = "",
         epoch: Optional[int] = None,
         inference_name: Optional[str] = None,
     ) -> None:
         super().__init__(
             embs=embs,
             probs=probs,
             logits=logits,
             ids=ids,
             split=split,
             epoch=epoch,
             inference_name=inference_name,
         )
-        # Explicit cast to List from parent
-        self.embs: List[np.ndarray] = list(self.embs)
-        self.logits: List[np.ndarray] = list(self.logits)
-        self.probs: List[np.ndarray] = list(self.probs)
 
         # Calculated internally
         self.gold_emb: List[List[np.ndarray]] = []
         self.gold_spans: List[List[Dict]] = []
         self.gold_conf_prob: List[List[np.ndarray]] = []
         self.gold_loss_prob: List[List[np.ndarray]] = []
         self.gold_loss_prob_label: List[List[int]] = []
@@ -138,33 +132,31 @@
     def get_valid_attributes() -> List[str]:
         """
         Returns a list of valid attributes that GalileoModelConfig accepts
         :return: List[str]
         """
         return GalileoModelLoggerAttributes.get_valid()
 
-    def validate(self) -> None:
+    def validate_and_format(self) -> None:
         """
         Validates that the current config is correct.
         * embs, probs, and ids must exist and be the same length
         :return:
         """
-        get_dq_logger().debug(
-            "Validating the output log.", split=self.split, epoch=self.epoch
-        )
         if len(self.logits):
-            self.probs = self.convert_logits_to_probs(self.logits).tolist()
+            self.probs = self.convert_logits_to_probs(self.logits)
         elif len(self.probs):
-            warnings.warn("Usage of probs is deprecated, use logits instead")
+            self.probs = self._convert_tensor_ndarray(self.probs)
 
         embs_len = len(self.embs)
         probs_len = len(self.probs)
         ids_len = len(self.ids)
 
         self.ids = self._convert_tensor_ndarray(self.ids)
+        self.embs = self._convert_tensor_ndarray(self.embs)
 
         assert all([embs_len, probs_len, ids_len]), (
             f"All of emb, probs, and ids for your logger must be set, but "
             f"got emb:{bool(embs_len)}, probs:{bool(probs_len)}, ids:{bool(ids_len)}"
         )
 
         assert embs_len == probs_len == ids_len, (
@@ -173,16 +165,14 @@
         )
 
         # We need to average the embeddings for the tokens within a span
         # so each span has only 1 embedding vector
         logged_sample_ids = []
         for sample_id, sample_emb, sample_prob in zip(self.ids, self.embs, self.probs):
             # This will return True if there was a prediction or gold span
-            sample_emb = self._convert_tensor_ndarray(sample_emb)
-            sample_prob = self._convert_tensor_ndarray(sample_prob)
             if self._process_sample(sample_id, sample_emb, sample_prob):
                 logged_sample_ids.append(sample_id)
 
         self.ids = logged_sample_ids
         if not self.ids:
             raise LogBatchError(
                 "No samples in this batch had any gold or prediction spans. "
@@ -195,17 +185,14 @@
         """Processes a sample. Returns whether or not the sample should be logged
 
         A sample should be logged only if there was at least 1 prediction span or 1
         gold span
 
         For inference mode, only prediction spans should be logged.
         """
-        get_dq_logger().debug(
-            "Processing a sample.", split=self.split, epoch=self.epoch
-        )
         # To extract metadata about the sample we are looking at
         sample_key = self.logger_config.get_sample_key(Split(self.split), sample_id)
 
         # Unpadded length of the sample. Used to extract true predicted spans
         # which are padded by the model
         sample_token_len = self.logger_config.sample_length[sample_key]
         # Remove padding from prob vector as well
@@ -242,22 +229,25 @@
             gold_sequence = self._construct_gold_sequence(
                 len(sample_prob), sample_gold_spans
             )
             gold_conf_prob, _ = self._extract_span_probs(
                 sample_gold_spans, sample_prob, NERProbMethod.confidence
             )
             gold_loss_prob, gold_loss_label = self._extract_span_probs(
-                sample_gold_spans, sample_prob, NERProbMethod.loss, gold_sequence
+                sample_gold_spans,
+                sample_prob,
+                NERProbMethod.loss,
+                gold_sequence_str=gold_sequence,
             )
-            argmax_indices: List[int] = sample_prob.argmax(axis=1).tolist()
-            pred_sequence: List[str] = [
-                self.logger_config.labels[x] for x in argmax_indices
-            ]
+            pred_sequence_idx = sample_prob.argmax(axis=1)
             pred_loss_prob, pred_gold_label = self._extract_span_probs(
-                sample_pred_spans, sample_prob, NERProbMethod.loss, pred_sequence
+                sample_pred_spans,
+                sample_prob,
+                NERProbMethod.loss,
+                gold_sequence_idx=pred_sequence_idx,
             )
 
             self.gold_spans.append(sample_gold_spans)
             self.gold_emb.append(gold_emb)
             self.gold_conf_prob.append(gold_conf_prob)
             self.gold_loss_prob.append(gold_loss_prob)
             self.pred_loss_prob.append(pred_loss_prob)
@@ -270,32 +260,30 @@
         self, spans: List[Dict], emb: np.ndarray
     ) -> List[np.ndarray]:
         """Get the embeddings for each span, on a per-sample basis
 
         We take the average of the token embeddings per span and use that as the span
         level embedding
         """
-        get_dq_logger().debug(
-            "Extracting span embeddings.", split=self.split, epoch=self.epoch
-        )
         embeddings = []
         for span in spans:
             start = span["start"]
             end = span["end"]
             span_embeddings = emb[start:end, :]
             avg_span_embedding = span_embeddings.mean(axis=0)
             embeddings.append(avg_span_embedding)
         return embeddings
 
     def _extract_span_probs(
         self,
         spans: List[Dict],
         prob: np.ndarray,
         method: NERProbMethod,
-        gold_sequence: Optional[List[str]] = None,
+        gold_sequence_str: Optional[List[str]] = None,
+        gold_sequence_idx: Optional[np.ndarray] = None,
     ) -> Tuple[List[np.ndarray], List[int]]:
         """Get the probs for each span, on a per-sample basis
 
         Parameters
         ----------
         spans
             The spans to extract probs for
@@ -308,28 +296,33 @@
         Returns
         -------
         List[np.ndarray]
             The probs for each span
         List[int]
             The gold label indices of token chosen for loss (needed for DEP calculation)
         """
-        get_dq_logger().debug(
-            "Extracting span probs.", split=self.split, epoch=self.epoch
-        )
         probs = []
         gold_labels = []
-        gold_sequence_str = gold_sequence or []
-        gold_sequence_idx = self.labels_to_idx(gold_sequence_str)
+        if gold_sequence_idx is None and gold_sequence_str is not None:
+            gold_sequence_idx = self.labels_to_idx(gold_sequence_str)
+
+        has_gold_sequence = (
+            gold_sequence_idx is not None and len(gold_sequence_idx) >= 0
+        )
 
         for span in spans:
             start = span["start"]
             end = span["end"]
             span_probs = prob[start:end, :]
+            # We ignore because if `has_gold_sequence` then has_gold_sequence must exist
+            # (see above), but mypy can't figure that out
             span_gold_seq = (
-                gold_sequence_idx[start:end] if gold_sequence_idx.size > 0 else None
+                gold_sequence_idx[start:end]  # type: ignore
+                if has_gold_sequence
+                else None
             )
             # We select a token prob to represent the span prob
             span_prob, gold_label = select_span_token_for_prob(
                 span_probs, method, span_gold_seq
             )
             probs.append(span_prob)
             # If method is 'loss' we return a list of gold labels
@@ -344,17 +337,14 @@
         """
         Extract prediction labels from probabilities, and generate pred spans
 
         If the schema is non-BIO, we just first convert them into BIO then extract spans
         """
         # use length of the tokens stored to strip the pads
         # Drop the spans post first PAD
-        get_dq_logger().debug(
-            "Extracting pred spans.", split=self.split, epoch=self.epoch
-        )
         argmax_indices: List[int] = pred_prob.argmax(axis=1)
         pred_sequence: List[str] = [
             self.logger_config.labels[x] for x in argmax_indices
         ]
 
         if self.logger_config.tagging_schema == TaggingSchema.BIO:
             pred_spans = self._extract_spans_bio(pred_sequence)
@@ -510,17 +500,14 @@
     ) -> List[str]:
         """
         Using gold spans and tagging schema, construct the underlying gold sequence
         e.g. gold_spans = [{start=5, end=8, label="nothing"}]
         gold_sequence = [O, O, O, O, O, B-nothing, I-nothing, I-nothing, O, O] for BIO
         gold_sequence = [O, O, O, O, O, B-nothing, I-nothing, L-nothing, O, O] for BILOU
         """
-        get_dq_logger().debug(
-            "Constructing a gold sequence", split=self.split, epoch=self.epoch
-        )
         gold_sequence = ["O"] * len_sequence
         for span in gold_spans:
             start = span["start"]
             end = span["end"]
             label = span["label"]
             if self.logger_config.tagging_schema == TaggingSchema.BIO:
                 gold_sequence[start:end] = [f"I-{label}"] * (end - start)
@@ -548,16 +535,14 @@
         will have repeating "sentence_id" values, which is OK. We will also loop
         through the data twice, once for prediction span information
         (one of pred_span, pred_emb, pred_prob per span) and once for gold span
         information (one of gold_span, gold_emb, gold_prob per span)
 
         NOTE: All spans are at the token level in this fn
         """
-        get_dq_logger().debug("Getting data dict.", split=self.split, epoch=self.epoch)
-
         if self.split == Split.inference:
             return self._get_data_dict_inference()
 
         data: defaultdict = defaultdict(list)
 
         # Loop through samples
         num_samples = len(self.ids)
@@ -805,17 +790,14 @@
         When indices don't match, the error is either span_shift or missed_label
         * span_shift: overlapping span start/end indices
         * missed_label: no overlap between span start/end indices
 
         In this function, we only look at spans that don't have pred/gold alignment,
         so the error can only be span_shift or missed_label.
         """
-        get_dq_logger().debug(
-            "Getting span error type.", split=self.split, epoch=self.epoch
-        )
         gold_start, gold_end = gold_span
         # We start by assuming missed_label (because it's the worst case)
         # and update if we see overlap
         error_type = NERErrorType.missed_label
         for pred_span in pred_spans:
             pred_start, pred_end = pred_span
             # We compare to the end of the spans non-inclusive because
@@ -834,22 +816,7 @@
     def __setattr__(self, key: Any, value: Any) -> None:
         if key not in self.get_valid_attributes():
             raise AttributeError(
                 f"{key} is not a valid attribute of {self.__logger_name__} logger. "
                 f"Only {self.get_valid_attributes()}"
             )
         super().__setattr__(key, value)
-
-    def convert_logits_to_probs(
-        self, sample_logits: Union[List[np.ndarray], np.ndarray]
-    ) -> np.ndarray:
-        """Converts logits to probs via softmax per sample"""
-        # axis ensures that in a matrix of probs with dims num_samples x num_classes
-        # we take the softmax for each sample
-        get_dq_logger().debug(
-            "Converting logits to probs.", split=self.split, epoch=self.epoch
-        )
-        token_probs = []
-        for token_logits in sample_logits:
-            token_probs.append(super().convert_logits_to_probs(token_logits))
-
-        return np.array(token_probs, dtype=object)
```

### Comparing `dataquality-0.8.9/dataquality/metrics.py` & `dataquality-0.9.0a0/dataquality/metrics.py`

 * *Files 6% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 
 def get_run_summary(
     project_name: str,
     run_name: str,
     split: Split,
     task: Optional[str] = None,
     inference_name: Optional[str] = None,
-    filter: Union[FilterParams, Dict] = None,
+    filter: Optional[Union[FilterParams, Dict]] = None,
 ) -> Dict:
     """Gets the summary for a run/split
 
     Calculates metrics (f1, recall, precision) overall (weighted) and per label.
     Also returns the top 50 rows of the dataframe (sorted by data_error_potential)
 
     :param project_name: The project name
@@ -121,15 +121,15 @@
 def get_metrics(
     project_name: str,
     run_name: str,
     split: Split,
     task: Optional[str] = None,
     inference_name: Optional[str] = None,
     category: str = "gold",
-    filter: Union[FilterParams, Dict] = None,
+    filter: Optional[Union[FilterParams, Dict]] = None,
 ) -> Dict[str, List]:
     """Calculates available metrics for a run/split, grouped by a particular category
 
     The category/column provided (can be gold, pred, or any categorical metadata column)
     will result in metrics per "group" or unique value of that category/column
 
     :param project_name: The project name
@@ -163,15 +163,15 @@
 def display_distribution(
     project_name: str,
     run_name: str,
     split: Split,
     task: Optional[str] = None,
     inference_name: Optional[str] = None,
     column: str = "data_error_potential",
-    filter: Union[FilterParams, Dict] = None,
+    filter: Optional[Union[FilterParams, Dict]] = None,
 ) -> None:
     """Displays the column distribution for a run. Plotly must be installed
 
     :param project_name: The project name
     :param run_name: The run name
     :param split: The split (training/test/validation/inference)
     :param task: (If multi-label only) the task name in question
@@ -264,15 +264,15 @@
     inference_name: str = "",
     file_type: FileType = FileType.arrow,
     include_embs: bool = False,
     include_probs: bool = False,
     include_token_indices: bool = False,
     hf_format: bool = False,
     tagging_schema: Optional[TaggingSchema] = None,
-    filter: Union[FilterParams, Dict] = None,
+    filter: Optional[Union[FilterParams, Dict]] = None,
     as_pandas: bool = True,
     include_data_embs: bool = False,
 ) -> Union[pd.DataFrame, DataFrame]:
     """Gets the dataframe for a run/split
 
     Downloads an arrow (or specified type) file to your machine and returns a loaded
     Vaex dataframe.
@@ -432,14 +432,15 @@
     """Process dataframe after export of run or edits.
 
     See `get_dataframe` and `get_edited_dataframe` for details"""
     split = conform_split(split)
     # See docstring. In this case, we need span-level data
     # You can't attach embeddings/probs to the huggingface data, since the HF format is
     # sample level, and the embeddings are span level
+
     embs = include_embs or include_data_embs
     if (embs or include_probs) and task_type == TaskType.text_ner and not hf_format:
         # In NER, the `probabilities` contains the span level data
         span_df = get_probabilities(project_name, run_name, split, inference_name)
         keep_cols = [i for i in span_df.get_column_names() if "prob" not in i]
         span_df = span_df[keep_cols]
         # These are the token (not char) indices, lets make that clear
@@ -450,18 +451,16 @@
             if i != "sample_id":
                 data_df.rename(i, f"sample_{i}")
         data_df = data_df.join(span_df, on="sample_id", allow_duplication=True)
 
     tasks = []
     if task_type == TaskType.text_multi_label:
         tasks = api_client.get_tasks_for_run(project_name, run_name)
-        labels = [
-            api_client.get_labels_for_run(project_name, run_name, task)
-            for task in tasks
-        ]
+        # Don't provide a task, get all task-labels
+        labels = get_labels_for_run(project_name, run_name)
         data_df = _index_df(data_df, labels, tasks)
         data_df = _clean_mltc_df(data_df)
     if task_type == TaskType.text_classification:
         labels_per_task = api_client.get_labels_for_run(project_name, run_name)
         data_df = _index_df(data_df, labels_per_task)
 
     if include_embs:
@@ -533,15 +532,15 @@
 
 
 def get_embeddings(
     project_name: str,
     run_name: str,
     split: Split,
     inference_name: str = "",
-    epoch: int = None,
+    epoch: Optional[int] = None,
 ) -> DataFrame:
     """Downloads the embeddings for a run/split at an epoch as a Vaex dataframe.
 
     If not provided, will take the embeddings from the final epoch. Note that only the
     n and n-1 epoch embeddings are available for download
 
     An hdf5 file will be downloaded to local and a Vaex dataframe will be returned
@@ -589,15 +588,15 @@
 
 
 def get_probabilities(
     project_name: str,
     run_name: str,
     split: Split,
     inference_name: str = "",
-    epoch: int = None,
+    epoch: Optional[int] = None,
 ) -> DataFrame:
     """Downloads the probabilities for a run/split at an epoch as a Vaex dataframe.
 
     If not provided, will take the probabilities from the final epoch.
 
     An hdf5 file will be downloaded to local and a Vaex dataframe will be returned
 
@@ -614,15 +613,15 @@
 
 
 def get_raw_data(
     project_name: str,
     run_name: str,
     split: Split,
     inference_name: str = "",
-    epoch: int = None,
+    epoch: Optional[int] = None,
 ) -> DataFrame:
     """Downloads the raw logged data for a run/split at an epoch as a Vaex dataframe.
 
     If not provided, will take the probabilities from the final epoch.
 
     An hdf5 file will be downloaded to local and a Vaex dataframe will be returned
 
@@ -640,29 +639,44 @@
     else:
         object_name = "data/data.hdf5"
     return _get_hdf5_file_for_epoch(
         project_name, run_name, split, object_name, inference_name, epoch
     )
 
 
-def get_xray_cards(
+def get_alerts(
     project_name: str, run_name: str, split: Split, inference_name: Optional[str] = None
 ) -> List[Dict[str, str]]:
-    """Get xray cards for a project/run/split
+    """Get alerts for a project/run/split
 
-    Xray cards are automatic insights calculated and provided by Galileo on your data
+    Alerts are automatic insights calculated and provided by Galileo on your data
     """
     split = conform_split(split)
-    return api_client.get_xray_cards(project_name, run_name, split, inference_name)
+    return api_client.get_alerts(project_name, run_name, split, inference_name)
 
 
 def get_labels_for_run(
     project_name: str, run_name: str, task: Optional[str] = None
-) -> List[str]:
-    """Gets labels for a given run. If multi-label, a task must be provided"""
+) -> List:
+    """Gets labels for a given run.
+
+    If multi-label, and a task is provided, this will get the labels for that task.
+    Otherwise, it will get all task-labels
+
+    In NER, the full label set with the tags for each label will be returned
+    """
+    project_id, run_id = api_client._get_project_run_id(project_name, run_name)
+    task_type = api_client.get_task_type(project_id, run_id)
+    if task_type == TaskType.text_ner:
+        labels_object = f"{project_id}/{run_id}/ner_labels/ner_labels.json"
+        labels_path = object_store.download_file(
+            labels_object, "/tmp/labels.json", config.results_bucket_name
+        )
+        with open(labels_path) as f:
+            return json.loads(f.read())
     return api_client.get_labels_for_run(project_name, run_name, task)
 
 
 def get_tasks_for_run(project_name: str, run_name: str) -> List[str]:
     """Gets task names for a multi-label run"""
     return api_client.get_tasks_for_run(project_name, run_name)
 
@@ -670,15 +684,15 @@
 @cached(_get_cache(), key=_cache_key)
 def _get_hdf5_file_for_epoch(
     project_name: str,
     run_name: str,
     split: Split,
     object_name: str,
     inference_name: str = "",
-    epoch: int = None,
+    epoch: Optional[int] = None,
 ) -> DataFrame:
     split = conform_split(split)
     emb = "emb" in object_name
     if split == Split.inference and inference_name:
         split_path = inference_name
     else:
         split_path = str(_validate_epoch(project_name, run_name, split, epoch, emb=emb))
@@ -686,15 +700,19 @@
     object_name = f"{project_id}/{run_id}/{split}/{split_path}/{object_name}"
     file_name = f"/tmp/{uuid4()}-{os.path.split(object_name)[-1]}"
     object_store.download_file(object_name, file_name)
     return vaex.open(file_name)
 
 
 def _validate_epoch(
-    project_name: str, run_name: str, split: Split, epoch: int = None, emb: bool = False
+    project_name: str,
+    run_name: str,
+    split: Split,
+    epoch: Optional[int] = None,
+    emb: bool = False,
 ) -> int:
     split = conform_split(split)
     epochs = get_epochs(project_name, run_name, split)
     last_epoch = epochs[-1]
     if not epochs:
         raise GalileoException(f"No epochs found for {project_name}/{run_name}")
     if epoch is None:
@@ -715,38 +733,38 @@
 def _index_df(df: DataFrame, labels: List, tasks: Optional[List] = None) -> DataFrame:
     """Indexes gold and pred columns"""
     # We do this so if this is TC (no tasks), we can still iterate with the same logic
     tasks = tasks or [None]
     for ind, task in enumerate(tasks):
         # If multi label, must do it per task. If TC, then it's just 1 list of labels
         task_labels = labels[ind] if task else labels
-        for col in ["gold", "pred"]:
-            if col not in df.get_column_names():
+        for col in ["gold", "pred", "label"]:
+            if col not in df.get_column_names() or df[col].dtype == int:
                 continue
             df_col = f"{col}_{task}" if task else col
             df[f"{df_col}_idx"] = df[df_col]
             df = df.ordinal_encode(f"{df_col}_idx", values=task_labels, lazy=True)
     return df
 
 
 def _rename_prob_cols(df: DataFrame, tasks: List[str]) -> DataFrame:
     for ind, task in enumerate(tasks):
         df.rename(f"prob_{ind}", f"prob_{task}")
     return df
 
 
-def _validate_filter(filter: Union[FilterParams, Dict] = None) -> Dict:
+def _validate_filter(filter: Optional[Union[FilterParams, Dict]] = None) -> Dict:
     # Validate the fields provided with pydantic before making request
     return FilterParams(**dict(filter or {})).dict()
 
 
 def _conform_edit(edit: Union[Edit, Dict]) -> Edit:
     if isinstance(edit, Edit):
         return edit
     return Edit(**edit)
 
 
 def _clean_mltc_df(df: DataFrame) -> DataFrame:
     """In MLTC, don't return the non-task-indexes gold/pred/dep columns"""
-    drop_cols = ["gold", "pred", "data_error_potential", "prob"]
+    drop_cols = ["gold", "label", "pred", "data_error_potential", "prob"]
     keep_cols = [col for col in df.get_column_names() if col not in drop_cols]
     return df[keep_cols]
```

### Comparing `dataquality-0.8.9/dataquality/schemas/condition.py` & `dataquality-0.9.0a0/dataquality/schemas/condition.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 }
 
 
 class ConditionFilter(BaseModel):
     """Filter a dataframe based on the column value
 
     Note that the column used for filtering is the same as the metric used
-      in the condition.
+    in the condition.
 
     :param operator: The operator to use for filtering (e.g. "gt", "lt", "eq", "neq")
         See `Operator`
     :param value: The value to compare against
     """
 
     metric: str
```

### Comparing `dataquality-0.8.9/dataquality/schemas/dataframe.py` & `dataquality-0.9.0a0/dataquality/schemas/dataframe.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from dataclasses import dataclass
 from enum import Enum, unique
 
 from pydantic import BaseModel
 from vaex.dataframe import DataFrame
 
 
-class BaseLoggerInOutFrames(BaseModel):
+class BaseLoggerDataFrames(BaseModel):
     prob: DataFrame
     emb: DataFrame
     data: DataFrame
 
     class Config:
         arbitrary_types_allowed = True
```

### Comparing `dataquality-0.8.9/dataquality/schemas/edit.py` & `dataquality-0.9.0a0/dataquality/schemas/edit.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.9/dataquality/schemas/hf.py` & `dataquality-0.9.0a0/dataquality/schemas/hf.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.9/dataquality/schemas/metrics.py` & `dataquality-0.9.0a0/dataquality/schemas/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,22 +78,22 @@
         meta_filter: Optional[List[MetaFilter]] = None  see MetaFilter class
         inference_filter: Optional[InferenceFilter] = None  see InferenceFilter class
         span_sample_ids: Optional[List[int]] = None  (NER only) filter for full samples
         span_text: Optional[str] = None  (NER only) filter only on span text
         exclude_ids: List[int] = []  opposite of `ids`
         lasso: Optional[LassoSelection] = None  see LassoSelection class
         class_filter: Optional[List[StrictStr]] = None  filter GT OR prediction
-        likely_mislabeled: Optional[List[StrictStr]] = None  Filter for only
+        likely_mislabeled: Optional[bool] = None  Filter for only
             likely_mislabeled samples. False/None will return all samples
         likely_mislabeled_dep_percentile: Optional[int] A percentile threshold for l
             ikely mislabeled. This field (ranged 0-100) determines the precision of the
             likely_mislabeled filter. The threshold is applied against the DEP
             distribution of the likely_mislabeled samples. A threshold of 0 returns all,
             100 returns 1 sample, and 50 will return the top 50% DEP samples that are
-            likely_mislabeled. Higher = more precision, lower = more recall. Default 50.
+            likely_mislabeled. Higher = more precision, lower = more recall. Default 0.
     """
 
     ids: List[int] = []
     similar_to: Optional[List[int]] = None
     num_similar_to: Optional[int] = None
     text_pat: Optional[StrictStr] = None
     regex: Optional[bool] = None
@@ -107,8 +107,8 @@
     span_sample_ids: Optional[List[int]] = None
     span_text: Optional[str] = None
     span_regex: Optional[bool] = None
     exclude_ids: List[int] = []
     lasso: Optional[LassoSelection] = None
     class_filter: Optional[List[StrictStr]] = None
     likely_mislabeled: Optional[bool] = None
-    likely_mislabeled_dep_percentile: Optional[int] = Field(50, ge=0, le=100)
+    likely_mislabeled_dep_percentile: Optional[int] = Field(0, ge=0, le=100)
```

### Comparing `dataquality-0.8.9/dataquality/schemas/ner.py` & `dataquality-0.9.0a0/dataquality/schemas/ner.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.9/dataquality/schemas/report.py` & `dataquality-0.9.0a0/dataquality/schemas/report.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.9/dataquality/schemas/route.py` & `dataquality-0.9.0a0/dataquality/schemas/route.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,34 +14,37 @@
     projects = "projects"
     runs = "runs"
     users = "users"
     cleanup = "cleanup"
     login = "login"
     current_user = "current_user"
     healthcheck = "healthcheck"
+    healthcheck_dq = "healthcheck/dq"
     slices = "slices"
     split_path = "split"
     splits = "splits"
     inference_names = "inference_names"
     jobs = "jobs"
     latest_job = "jobs/latest"
     presigned_url = "presigned_url"
     tasks = "tasks"
     labels = "labels"
     epochs = "epochs"
     summary = "insights/summary"
     groupby = "insights/groupby"
+    metrics = "metrics"
     distribution = "insights/distribution"
-    xray = "insights/xray"
+    alerts = "insights/alerts"
     export = "export"
     edits = "edits"
     export_edits = "edits/export"
     ampli = "ampli"
     notify = "notify/email"
     token = "get-token"
+    upload_file = "upload_file"
 
     @staticmethod
     def content_path(
         project_id: Optional[Union[str, UUID4]] = None,
         run_id: Optional[Union[str, UUID4]] = None,
         split: Optional[Union[str, Split]] = None,
     ) -> str:
```

### Comparing `dataquality-0.8.9/dataquality/schemas/split.py` & `dataquality-0.9.0a0/dataquality/schemas/split.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 from enum import Enum
 from typing import List, Union
 
 from dataquality.exceptions import GalileoException
 
 
 class Split(str, Enum):
-    training = "training"
     train = "training"
+    training = "training"
+    val = "validation"
+    valid = "validation"
     validation = "validation"
     test = "test"
     testing = "test"
     inference = "inference"
 
     @staticmethod
     def get_valid_attributes() -> List[str]:
         return list(map(lambda x: x.value, Split))
 
     @staticmethod
     def get_valid_keys() -> List[str]:
-        return ["train", "training", "test", "testing", "validation"]
+        return ["train", "training", "val", "valid", "validation", "test", "testing"]
 
 
 def conform_split(split: Union[str, Split]) -> Split:
     """Conforms split name to our naming conventions
 
     Raises GalileoException if split is invalid
     """
```

### Comparing `dataquality-0.8.9/dataquality/utils/ampli.py` & `dataquality-0.9.0a0/dataquality/utils/ampli.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,13 @@
     dq_finish = "dq_finish"
     dq_finished = "dq_finished"
     dq_set_labels = "dq_set_labels"
     dq_log_data = "dq_log_data"
     dq_login = "dq_login"
     dq_import_torch = "dq_import_torch"
     dq_import_tensorflow = "dq_import_tensorflow"
-    dq_import_spacy = "dq_import_spacy"
     dq_function_call = "dq_function_call"
     dq_general_exception = "dq_general_exception"
     dq_log_data_exception = "dq_log_data_exception"
     dq_galileo_warning = "dq_galileo_warning"
     dq_log_batch_error = "dq_log_batch_error"
     dq_validation_error = "dq_validation_error"
```

### Comparing `dataquality-0.8.9/dataquality/utils/auto_trainer.py` & `dataquality-0.9.0a0/dataquality/utils/auto_trainer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,28 @@
+from typing import Optional
+
 from datasets import DatasetDict
 from transformers import Trainer
 
 import dataquality as dq
 from dataquality.integrations.transformers_trainer import watch
 from dataquality.schemas.split import Split
 
 
 def do_train(
     trainer: Trainer,
     encoded_data: DatasetDict,
     wait: bool,
-    create_data_embs: bool = False,
-) -> None:
+    create_data_embs: Optional[bool] = None,
+) -> Trainer:
     watch(trainer)
     trainer.train()
     if Split.test in encoded_data:
         # We pass in a huggingface dataset but typing wise they expect a torch dataset
         trainer.predict(test_dataset=encoded_data[Split.test])  # type: ignore
 
     inf_names = [k for k in encoded_data if k not in Split.get_valid_keys()]
     for inf_name in inf_names:
         dq.set_split(Split.inference, inference_name=inf_name)
         trainer.predict(test_dataset=encoded_data[inf_name])
     dq.finish(wait=wait, create_data_embs=create_data_embs)
+    return trainer
```

### Comparing `dataquality-0.8.9/dataquality/utils/dq_logger.py` & `dataquality-0.9.0a0/dataquality/utils/dq_logger.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 from typing import Any, Optional, Tuple
 
 from pydantic import UUID4
 from requests import HTTPError
 
 from dataquality.clients.api import ApiClient
 from dataquality.clients.objectstore import ObjectStore
-from dataquality.core._config import ConfigData, config
+from dataquality.core._config import config, config_data
 from dataquality.utils.helpers import check_noop
 
-DQ_LOG_FILE_HOME = f"{ConfigData.DEFAULT_GALILEO_CONFIG_DIR}/out"
+DQ_LOG_FILE_HOME = f"{config_data.DEFAULT_GALILEO_CONFIG_DIR}/out"  # type: ignore
 DQ_LOG_FILE = "out.log"
 
 
 class CustomSplitAdapter(logging.LoggerAdapter):
     """
     This adapter appends the split to the message, if found. Otherwise, "None"
 
@@ -67,15 +67,15 @@
 def upload_dq_log_file() -> None:
     # For typing
     assert config.current_project_id and config.current_run_id
     obj_store = ObjectStore()
     obj_name = dq_log_object_name(config.current_project_id, config.current_run_id)
     file_path = dq_log_file_path()
     if os.path.isfile(file_path):
-        obj_store.create_project_run_object(
+        obj_store.create_object(
             object_name=obj_name,
             file_path=file_path,
             content_type="text/plain",
             progress=False,
         )
         remove_dq_log_file()
```

### Comparing `dataquality-0.8.9/dataquality/utils/helpers.py` & `dataquality-0.9.0a0/dataquality/utils/helpers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import os
 import webbrowser
 from functools import wraps
 from typing import Any, Callable, Dict, List, Optional, Tuple, TypeVar
 
 from typing_extensions import ParamSpec
 
+from dataquality.exceptions import GalileoException
+
 T = TypeVar("T")
 P = ParamSpec("P")
 GALILEO_DISABLED = "GALILEO_DISABLED"
 GALILEO_VERBOSE = "GALILEO_VERBOSE"
 
 
 def check_noop(func: Callable[P, T]) -> Callable[P, Optional[T]]:
@@ -81,28 +83,53 @@
 
 def map_indices_to_ids(id_map: List, indices: List) -> List:
     """Maps the indices to the ids
     :param id_map: The list used for mapping indices to ids
     :param indices: The indices to map
     :return: The ids
     """
-    return [id_map[i] for i in indices]
+    try:
+        return [id_map[i] for i in indices]
+    except IndexError:
+        raise GalileoException(
+            "The indicies of the model output are not matching the logged data "
+            "samples. If you are using RandomSampler or WeightedRandomSampler, "
+            "pass dataloader_random_sampling=True to the watch function"
+        )
 
 
 def open_console_url(link: Optional[str] = "") -> None:
     """Tries to open the console url in the browser, if possible.
 
     This will work in local environments like jupyter or a python script, but won't
     work in colab (because colab is running on a server, so there's no "browser" to
     interact with). This also prints out the link for users to click so even in those
     environments they still have something to interact with.
     """
     if not link:
         return
     try:
-
         webbrowser.open(link)
     # In some environments, webbrowser will raise. Other times it fails silently (colab)
     except Exception:
         pass
     finally:
         print(f"Click here to see your run! {link}")
+
+
+def gpu_available() -> bool:
+    import torch
+
+    return torch.cuda.is_available()
+
+
+def mps_available() -> bool:
+    """Checks for an MPS compatible GPU on Apple machines.
+
+    This will enabled Metal acceleration for model training when supported.
+    """
+    import torch
+
+    try:
+        return torch.backends.mps.is_available()
+    except Exception:
+        return False
```

### Comparing `dataquality-0.8.9/dataquality/utils/hf_tokenizer.py` & `dataquality-0.9.0a0/dataquality/utils/hf_tokenizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,19 @@
         self.gold_spans: List[Dict] = []
         self.current_gold_span_idx = -1
 
     def initialize_sample(self, k: int) -> None:
         self.previous_word_id = -1
         self.word_ids = self.tokenized_samples.word_ids(batch_index=k)
         # We check ds and ds.features to accomodate HF and arrow datasets
-        if HFCol.ner_tags in self.ds or HFCol.ner_tags in self.ds.features:
+        # Note we need to make sure that ds has an attr "features" to handle
+        # the weird case when type(ds) = datasets.formatting.formatting.LazyBatch
+        if HFCol.ner_tags in self.ds or (
+            hasattr(self.ds, "features") and HFCol.ner_tags in self.ds.features
+        ):
             existing_labels = [
                 self.idx_2_labels[label] for label in self.ds[HFCol.ner_tags][k]
             ]
             self.word_gold_spans = extract_gold_spans_at_word_level(
                 existing_labels, self.schema
             )
         # If ner_tags is not present, we know split must be 'inference'
@@ -139,15 +143,15 @@
         is_last_index = w_index_bpe == len(self.word_ids) - 1
         wid_is_last = wid != self.word_ids[w_index_bpe + 1] and wid == span_end_word
         return is_last_index or wid_is_last
 
     def _adjust_label_at_index(self, w_index_bpe: int, span_label_suffix: str) -> None:
         if self.schema == TaggingSchema.BILOU:
             self.adjusted_labels[w_index_bpe] = f"U-{span_label_suffix}"
-        if self.schema == TaggingSchema.BIOES:
+        elif self.schema == TaggingSchema.BIOES:
             self.adjusted_labels[w_index_bpe] = f"S-{span_label_suffix}"
         else:
             self.adjusted_labels[w_index_bpe] = f"B-{span_label_suffix}"
         self.adjusted_label_indices[w_index_bpe] = self.labels_2_idx[
             self.adjusted_labels[w_index_bpe]
         ]
         self.current_gold_span_idx += 1
@@ -170,15 +174,15 @@
                 SpanKey.label: span_label_suffix,
             }
         )
 
     def _adjust_last_bpe(self, w_index_bpe: int, span_label_suffix: str) -> None:
         if self.schema == TaggingSchema.BILOU:
             self.adjusted_labels[w_index_bpe] = f"L-{span_label_suffix}"
-        if self.schema == TaggingSchema.BIOES:
+        elif self.schema == TaggingSchema.BIOES:
             self.adjusted_labels[w_index_bpe] = f"E-{span_label_suffix}"
         else:
             self.adjusted_labels[w_index_bpe] = f"I-{span_label_suffix}"
         self.adjusted_label_indices[w_index_bpe] = self.labels_2_idx[
             self.adjusted_labels[w_index_bpe]
         ]
         # Update end indices
```

### Comparing `dataquality-0.8.9/dataquality/utils/keras.py` & `dataquality-0.9.0a0/dataquality/utils/keras.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,19 @@
     sample_weight = kwargs.get("sample_weight")
     x = tf.range(x_len)
     y = x
 
     if validation_split and validation_data is None:
         # Create the validation data using the training data. Only supported
         # for `Tensor` and `NumPy` input.
-        (x, y, sample_weight,), validation_data = data_adapter.train_validation_split(
+        (
+            x,
+            y,
+            sample_weight,
+        ), validation_data = data_adapter.train_validation_split(
             (x, y, sample_weight), validation_split=validation_split
         )
 
     if validation_data:
         (
             val_x,
             val_y,
```

### Comparing `dataquality-0.8.9/dataquality/utils/ml.py` & `dataquality-0.9.0a0/dataquality/utils/ml.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.9/dataquality/utils/name.py` & `dataquality-0.9.0a0/dataquality/utils/name.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,39 @@
 import random
+import re
+from typing import Optional
+from uuid import uuid4
+
+from dataquality.exceptions import GalileoException
+
+BAD_CHARS_REGEX = r"[^\w -]+"
+
+
+def validate_name(name: Optional[str], assign_random: bool = False) -> str:
+    """Validates project/run name ensuring only letters, numbers, space, - and _
+
+    If no name is provided, a random name is generated
+    """
+    if not name and assign_random:
+        name = random_name()
+
+    if not name:
+        raise GalileoException(
+            "Name is required. Set assign_random to True to generate a random name"
+        )
+
+    badchars = re.findall(BAD_CHARS_REGEX, name)
+    if badchars:
+        raise GalileoException(
+            "Only letters, numbers, whitespace, - and _ are allowed in a project "
+            f"or run name. Remove the following characters: {badchars}"
+        )
+
+    return name
+
 
 ADJECTIVES = [
     "able",
     "above",
     "absent",
     "absolute",
     "abstract",
@@ -1576,12 +1607,14 @@
     "violet",
     "white",
     "yellow",
 ]
 
 
 def random_name() -> str:
-    result = []
-    result.append(random.choice(ADJECTIVES))
-    result.append(random.choice(COLORS))
-    result.append(random.choice(ANIMALS))
+    result = [
+        random.choice(ADJECTIVES),
+        random.choice(COLORS),
+        random.choice(ANIMALS),
+        str(uuid4())[:5],
+    ]
     return "_".join(result).lower()
```

### Comparing `dataquality-0.8.9/dataquality/utils/profiler.py` & `dataquality-0.9.0a0/dataquality/utils/profiler.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.9/dataquality/utils/thread_pool.py` & `dataquality-0.9.0a0/dataquality/utils/thread_pool.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,67 +1,66 @@
 import os
+import threading
 from threading import Thread
 from time import sleep
-from typing import Any, Callable, Iterable, List
+from typing import Any, Callable, Iterable, List, Optional
 
 from dataquality.exceptions import GalileoException
 
+lock = threading.Lock()
+
 
 class ThreadPoolManager:
     """
     A class for managing the threaded logging calls throughout dataquality
     """
 
     THREADS: List[Thread] = []
     MAX_THREADS = os.cpu_count() or 10
 
     @staticmethod
-    def add_thread(target: Callable, args: Iterable[Any] = None) -> None:
+    def add_thread(target: Callable, args: Optional[Iterable[Any]] = None) -> None:
         """
         Start a new function in a thread and store that in the global list of threads
 
         :param target: The callable
         :param args: The arguments to the function
-        :return: None
         """
         ThreadPoolManager.wait_for_thread()
         thread = Thread(target=target, args=args or [])
         try:
             thread.start()
             ThreadPoolManager.THREADS.append(thread)
         # Push up to the user
         except Exception as e:
             raise GalileoException(e)
 
     @staticmethod
     def wait_for_threads() -> None:
         """
         Joins all currently active threads and waits for all to be done
-
-        :return: None
         """
         ThreadPoolManager._cleanup()
         # Waits for each thread to finish
         for i in ThreadPoolManager.THREADS:
             i.join()
         ThreadPoolManager._cleanup()
 
     @staticmethod
     def wait_for_thread() -> None:
         """
         Waits for an open slot in the ThreadPool for another thread.
         """
         ThreadPoolManager._cleanup()
         while len(ThreadPoolManager.THREADS) >= ThreadPoolManager.MAX_THREADS:
+            # this sleep is necessary to prevent the thread from hogging compute
             sleep(0.05)
             ThreadPoolManager._cleanup()
 
     @staticmethod
     def _cleanup() -> None:
         """
         Cleans up the ThreadPoolManager, removing any dead ones
-
-        :return: None
         """
         ThreadPoolManager.THREADS = [
             i for i in ThreadPoolManager.THREADS if i.is_alive()
         ]
```

### Comparing `dataquality-0.8.9/dataquality/utils/version.py` & `dataquality-0.9.0a0/dataquality/utils/version.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import requests
-from setuptools.version import pkg_resources  # type: ignore
 
 from dataquality import __version__ as dq_client_version
 from dataquality.core._config import config
 from dataquality.exceptions import GalileoException
 from dataquality.schemas.route import Route
 
 
@@ -14,34 +13,27 @@
     matching major versions.
 
     https://semver.org/#summary.
 
     Returns:
         None
     """
-    client_semver = _parse_version(_get_client_version())
-    server_semver = _parse_version(_get_api_version())
+    client_semver = _get_client_version()
+    server_semver = _get_api_version()
     try:
         assert _major_version(client_semver) == _major_version(server_semver)
     except AssertionError:
         raise GalileoException(
             "Major mismatch between client, "
             f"{client_semver}, and server {server_semver}."
         )
 
 
-def _major_version(v: pkg_resources.extern.packaging.version.Version) -> str:
-    if hasattr(v, "major"):
-        return str(v.major)
-    else:
-        return str(v.base_version).split(".")[0]
-
-
-def _parse_version(version: str) -> pkg_resources.extern.packaging.version.Version:
-    return pkg_resources.parse_version(version)
+def _major_version(v: str) -> str:
+    return str(v).split(".")[0]
 
 
 def _get_client_version() -> str:
     return dq_client_version
 
 
 def _get_api_version() -> str:
```

### Comparing `dataquality-0.8.9/tests/integrations/hf/test_hf_integration.py` & `dataquality-0.9.0a0/dataquality/dq_auto/text_classification.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,301 +1,263 @@
-import json
-import sys
-from typing import Callable, Dict, List
-from unittest import mock
+from typing import Dict, List, Optional, Union
 
-import datasets
 import numpy as np
-import pytest
-
-from dataquality.exceptions import GalileoException
-from dataquality.integrations.hf import (
-    _extract_labels_from_ds,
-    _validate_dataset,
-    get_dataloader,
-    infer_schema,
-    tokenize_adjust_labels,
-    tokenize_and_log_dataset,
-)
-from dataquality.schemas.ner import TaggingSchema
+import pandas as pd
+from datasets import ClassLabel, Dataset, DatasetDict
+from transformers import Trainer
+
+import dataquality as dq
+from dataquality import Analytics, ApiClient
+from dataquality.dq_auto.base_data_manager import BaseDatasetManager
+from dataquality.dq_auto.tc_trainer import get_trainer
 from dataquality.schemas.split import Split
-from dataquality.utils.hf_tokenizer import extract_gold_spans_at_word_level
-from tests.test_utils.hf_integration_constants import (
-    ADJUSTED_TOKEN_DATA,
-    UNADJUSTED_TOKEN_DATA,
-    BILOUSequence,
-    BIOESSequence,
-    BIOSequence,
-    mock_ds,
-    mock_tokenizer,
-    tag_names,
-)
-from tests.test_utils.hf_integration_constants_inference import (
-    ADJUSTED_TOKEN_DATA_INF,
-    label_names,
-    mock_ds_inf,
-    mock_tokenizer_inf,
-)
-
-
-@pytest.mark.parametrize(
-    "labels,schema",
-    [
-        (["B-PER", "I-PER", "B-ORG", "O"], TaggingSchema.BIO),
-        (["B-PER", "I-PER", "B-ORG", "U-ORG", "L-ORG", "O"], TaggingSchema.BILOU),
-        (["B-PER", "I-PER", "B-ORG", "S-ORG", "E-ORG", "O"], TaggingSchema.BIOES),
-        (["G", "A", "R", "B", "A", "G", "E"], "error"),
-    ],
-)
-def test_infer_schema(labels: List[str], schema: TaggingSchema) -> None:
-    if schema == "error":
-        with pytest.raises(GalileoException):
-            infer_schema(labels)
-    else:
-        assert infer_schema(labels) == schema
-
-
-def test_tokenize_adjust_labels() -> None:
-    output = tokenize_adjust_labels(mock_ds, mock_tokenizer, tag_names)
-    for k in ADJUSTED_TOKEN_DATA:
-        assert ADJUSTED_TOKEN_DATA[k] == output[k]
-
-
-@pytest.mark.parametrize(
-    "gold_sequence,gold_span",
-    list(zip(BIOSequence.gold_sequences, BIOSequence.gold_spans)),
-)
-def test_extract_gold_spans_at_word_level_bio(
-    gold_sequence: List[str], gold_span: List[Dict]
-) -> None:
-    assert (
-        extract_gold_spans_at_word_level(gold_sequence, TaggingSchema.BIO) == gold_span
-    )
-
-
-@pytest.mark.parametrize(
-    "gold_sequence,gold_span",
-    list(zip(BIOESSequence.gold_sequences, BIOESSequence.gold_spans)),
+from dataquality.schemas.task_type import TaskType
+from dataquality.utils.auto import (
+    add_class_label_to_dataset,
+    add_val_data_if_missing,
+    run_name_from_hf_dataset,
 )
-def test_extract_gold_spans_at_word_level_bioes(
-    gold_sequence: List[str], gold_span: List[Dict]
-) -> None:
-    assert (
-        extract_gold_spans_at_word_level(gold_sequence, TaggingSchema.BIOES)
-        == gold_span
-    )
+from dataquality.utils.auto_trainer import do_train
 
+a = Analytics(ApiClient, dq.config)
+a.log_import("auto_tc")
 
-@pytest.mark.parametrize(
-    "gold_sequence,gold_span",
-    list(zip(BILOUSequence.gold_sequences, BILOUSequence.gold_spans)),
-)
-def test_extract_gold_spans_at_word_level_bilou(
-    gold_sequence: List[str], gold_span: List[Dict]
-) -> None:
-    assert (
-        extract_gold_spans_at_word_level(gold_sequence, TaggingSchema.BILOU)
-        == gold_span
-    )
 
-
-def test_validate_dataset() -> None:
-    ds = datasets.Dataset.from_dict(
-        dict(
-            my_text=["sample1", "sample2", "sample3"],
-            my_labels=["A", "A", "B"],
-            my_id=[1, 2, 3],
+class TCDatasetManager(BaseDatasetManager):
+    DEMO_DATASETS = [
+        "rungalileo/newsgroups",
+        "rungalileo/trec6",
+        "rungalileo/conv_intent",
+        "rungalileo/emotion",
+        "rungalileo/amazon_polarity_30k",
+        "rungalileo/sst2",
+    ]
+
+    def _convert_pandas_object_dtype(self, df: pd.DataFrame) -> pd.DataFrame:
+        """Converts columns of object type to string type for huggingface
+
+        Huggingface DataSets cannot handle mixed-type columns as columns due to Arrow.
+        This casts those columns to strings
+        """
+        for c in df.columns:
+            if df[c].dtype == object:
+                df[c] = df[c].astype("str")
+        return df
+
+    def _convert_df_to_dataset(
+        self, df: pd.DataFrame, labels: Optional[List[str]] = None
+    ) -> Dataset:
+        """Converts a pandas dataframe to a well-formed huggingface dataset
+
+        The main thing happening here is that we are taking the pandas label column and
+        mapping it to a Dataset ClassLabel if possible. If not, it will get parsed later
+        or a validation error will be thrown if not possible in `_validate_dataset_dict`
+        """
+        df_copy = self._convert_pandas_object_dtype(df.copy())
+        # If there's no label column, we can't do any ClassLabel conversions. Validation
+        # of the hf DatasetDict will handle this missing label column if it's an
+        # issue. See `_validate_dataset_dict`
+        ds = Dataset.from_pandas(df_copy)
+        return add_class_label_to_dataset(ds, labels)
+
+    def _validate_dataset_dict(
+        self,
+        dd: DatasetDict,
+        inference_names: List[str],
+        labels: Optional[List[str]] = None,
+    ) -> DatasetDict:
+        """Validates the core components of the provided (or created) DatasetDict)
+
+        The DatasetDict that the user provides or that we create from the provided
+        train/test/val data must have the following:
+            * all keys must be one of our valid key names
+            * it must have a `text` column
+            * it must have a `label` column
+                * if the `label` column isn't a ClassLabel, we convert it to one
+
+        We then also convert the keys of the DatasetDict to our `Split` key enum so
+        we can access it easier in the future
+        """
+        clean_dd = super()._validate_dataset_dict(dd, inference_names, labels)
+        for key in list(clean_dd.keys()):
+            ds = clean_dd.pop(key)
+            assert "text" in ds.features, "Dataset must have column `text`"
+            if key not in inference_names:
+                assert "label" in ds.features, "Dataset must have column `label`"
+                if not isinstance(ds.features["label"], ClassLabel):
+                    ds = add_class_label_to_dataset(ds, labels)
+            if "id" not in ds.features:
+                ds = ds.add_column("id", list(range(ds.num_rows)))
+            clean_dd[key] = ds
+        return add_val_data_if_missing(clean_dd)
+
+
+def _get_labels(dd: DatasetDict, labels: Optional[List[str]] = None) -> List[str]:
+    """Gets the labels for this dataset from the dataset if not provided."""
+    if labels is not None and isinstance(labels, (list, np.ndarray)):
+        return list(labels)
+    train_labels = dd[Split.train].features["label"]
+    if hasattr(train_labels, "names"):
+        return train_labels.names
+    return sorted(set(dd[Split.train]["label"]))
+
+
+def _log_dataset_dict(dd: DatasetDict) -> None:
+    for key in dd:
+        ds = dd[key]
+        default_cols = ["text", "label", "id"]
+        meta = [i for i in ds.features if i not in default_cols]
+        if key in Split.get_valid_keys():
+            dq.log_dataset(ds, meta=meta, split=key)
+        else:
+            dq.log_dataset(ds, meta=meta, split=Split.inference, inference_name=key)
+
+
+def auto(
+    hf_data: Optional[Union[DatasetDict, str]] = None,
+    hf_inference_names: Optional[List[str]] = None,
+    train_data: Optional[Union[pd.DataFrame, Dataset, str]] = None,
+    val_data: Optional[Union[pd.DataFrame, Dataset, str]] = None,
+    test_data: Optional[Union[pd.DataFrame, Dataset, str]] = None,
+    inference_data: Optional[Dict[str, Union[pd.DataFrame, Dataset, str]]] = None,
+    max_padding_length: int = 200,
+    num_train_epochs: int = 15,
+    hf_model: str = "distilbert-base-uncased",
+    labels: Optional[List[str]] = None,
+    project_name: str = "auto_tc",
+    run_name: Optional[str] = None,
+    wait: bool = True,
+    create_data_embs: Optional[bool] = None,
+) -> Trainer:
+    """Automatically gets insights on a text classification dataset
+
+    Given either a pandas dataframe, file_path, or huggingface dataset path, this
+    function will load the data, train a huggingface transformer model, and
+    provide Galileo insights via a link to the Galileo Console
+
+    One of `hf_data`, `train_data` should be provided. If neither of those are, a
+    demo dataset will be loaded by Galileo for training.
+
+    :param hf_data: Union[DatasetDict, str] Use this param if you have huggingface
+        data in the hub or in memory. Otherwise see `train_data`, `val_data`,
+        and `test_data`. If provided, train_data, val_data, and test_data are ignored
+    :param hf_inference_names: A list of key names in `hf_data` to be run as inference
+        runs after training. If set, those keys must exist in `hf_data`
+    :param train_data: Optional training data to use. Can be one of
+        * Pandas dataframe
+        * Huggingface dataset
+        * Path to a local file
+        * Huggingface dataset hub path
+    :param val_data: Optional validation data to use. The validation data is what is
+        used for the evaluation dataset in huggingface, and what is used for early
+        stopping. If not provided, but test_data is, that will be used as the evaluation
+        set. If neither val nor test are available, the train data will be randomly
+        split 80/20 for use as evaluation data.
+        Can be one of
+        * Pandas dataframe
+        * Huggingface dataset
+        * Path to a local file
+        * Huggingface dataset hub path
+    :param test_data: Optional test data to use. The test data, if provided with val,
+        will be used after training is complete, as the held-out set. If no validation
+        data is provided, this will instead be used as the evaluation set.
+        Can be one of
+        * Pandas dataframe
+        * Huggingface dataset
+        * Path to a local file
+        * Huggingface dataset hub path
+    :param inference_data: Optional inference datasets to run with after training
+        completes. The structure is a dictionary with the key being the infeerence name
+        and the value one of
+        * Pandas dataframe
+        * Huggingface dataset
+        * Path to a local file
+        * Huggingface dataset hub path
+    :param max_padding_length: The max length for padding the input text
+        during tokenization. Default 200
+    :param hf_model: The pretrained AutoModel from huggingface that will be used to
+        tokenize and train on the provided data. Default distilbert-base-uncased
+    :param labels: Optional list of labels for this dataset. If not provided, they
+        will attempt to be extracted from the data
+    :param project_name: Optional project name. If not set, a random name will
+        be generated
+    :param run_name: Optional run name for this data. If not set, a random name will
+        be generated
+    :param wait: Whether to wait for Galileo to complete processing your run.
+        Default True
+    :param create_data_embs: Whether to create data embeddings for this run. Default
+        False
+
+    To see auto insights on a random, pre-selected dataset, simply run
+    ```python
+        from dataquality.auto.text_classification import auto
+
+        auto()
+    ```
+
+    An example using `auto` with a hosted huggingface dataset
+    ```python
+        from dataquality.auto.text_classification import auto
+
+        auto(hf_data="rungalileo/trec6")
+    ```
+
+    An example using `auto` with sklearn data as pandas dataframes
+    ```python
+        import pandas as pd
+        from sklearn.datasets import fetch_20newsgroups
+        from dataquality.auto.text_classification import auto
+
+        # Load the newsgroups dataset from sklearn
+        newsgroups_train = fetch_20newsgroups(subset='train')
+        newsgroups_test = fetch_20newsgroups(subset='test')
+        # Convert to pandas dataframes
+        df_train = pd.DataFrame(
+            {"text": newsgroups_train.data, "label": newsgroups_train.target}
         )
-    )
-    # Must be a DatasetDict, not Dataset
-    with pytest.raises(GalileoException) as e:
-        _validate_dataset(ds)
-    assert str(e.value) == (
-        f"Expected DatasetDict but got object of type {type(ds)}. "
-        f"If this is a dataset, you can create a dataset dict by running\n"
-        "dd = datasets.DatasetDict({'your_split': your_Dataset})"
-    )
-
-
-@pytest.mark.skipif(sys.version_info < (3, 8), reason="requires python3.8 or higher")
-@mock.patch("dataquality.log_dataset")
-def test_tokenize_and_log_dataset(
-    mock_log_dataset: mock.MagicMock, set_test_config
-) -> None:
-    """Tests the e2e function call, passing in a DatasetDict and receiving a
-
-    new DatasetDict, and that the datasets per split were logged correctly.
-    """
-    set_test_config(task_type="text_ner")
-    tokenize_output = tokenize_adjust_labels(mock_ds, mock_tokenizer, tag_names)
-    with mock.patch("dataquality.integrations.hf.tokenize_adjust_labels") as mock_tok:
-        mock_tok.return_value = tokenize_output
-        ds_dict = datasets.DatasetDict(
-            {
-                "train": mock_ds,
-                "test": mock_ds,
-                "validation": mock_ds,
-            }
+        df_test = pd.DataFrame(
+            {"text": newsgroups_test.data, "label": newsgroups_test.target}
         )
-        output = tokenize_and_log_dataset(ds_dict, mock_tokenizer)
-
-    for split in ds_dict.keys():
-        split_output = output[split]
-        for k in ADJUSTED_TOKEN_DATA:
-            token_data = ADJUSTED_TOKEN_DATA[k]
-            if k == "text_token_indices":
-                # We abuse token data because outputs are returning tuples but we want
-                # to compare lists
-                token_data = json.loads(json.dumps(token_data))
-            assert token_data == split_output[k]
-
-    assert mock_log_dataset.call_count == 3
-    for split in [Split.train, Split.test, Split.validation]:
-        mock_log_dataset.assert_any_call(mock.ANY, split=split, meta=[])
-
-
-@pytest.mark.skipif(sys.version_info < (3, 8), reason="requires python3.8 or higher")
-@mock.patch("dataquality.log_dataset")
-def test_tokenize_and_log_dataset_inference(
-    mock_log_dataset: mock.MagicMock, set_test_config
-) -> None:
-    """Tests the e2e function call, passing in a DatasetDict and receiving a
 
-    new DatasetDict, and that the datasets per split were logged correctly.
-    """
-    set_test_config(task_type="text_ner")
-    tokenize_output = tokenize_adjust_labels(mock_ds, mock_tokenizer, tag_names)
-    tokenize_output_inf = tokenize_adjust_labels(
-        mock_ds_inf, mock_tokenizer_inf, label_names
-    )
-    with mock.patch("dataquality.integrations.hf.tokenize_adjust_labels") as mock_tok:
-        mock_tok.side_effect = [tokenize_output, tokenize_output_inf]
-        ds_dict = datasets.DatasetDict(
-            {
-                "train": mock_ds,
-                "inf1": mock_ds_inf,
-            }
+        auto(
+             train_data=df_train,
+             test_data=df_test,
+             labels=newsgroups_train.target_names,
+             project_name="newsgroups_work",
+             run_name="run_1_raw_data"
         )
-        output = tokenize_and_log_dataset(ds_dict, mock_tokenizer, label_names)
+    ```
 
-    for split in ds_dict.keys():
-        expected_data = (
-            ADJUSTED_TOKEN_DATA_INF if split == "inf1" else ADJUSTED_TOKEN_DATA
-        )
-        split_output = output[split]
-        for k in expected_data:
-            token_data = expected_data[k]
-            if k == "text_token_indices":
-                # We abuse token data because outputs are returning tuples but we want
-                # to compare lists
-                token_data = json.loads(json.dumps(token_data))
-            assert token_data == split_output[k]
-
-    assert mock_log_dataset.call_count == 2
-    mock_log_dataset.assert_any_call(mock.ANY, split=Split.training, meta=[])
-    mock_log_dataset.assert_any_call(
-        mock.ANY, split=Split.inference, meta=[], inference_name="inf1"
+    An example of using `auto` with a local CSV file with `text` and `label` columns
+    ```python
+    from dataquality.auto.text_classification import auto
+
+    auto(
+         train_data="train.csv",
+         test_data="test.csv",
+         project_name="data_from_local",
+         run_name="run_1_raw_data"
     )
-
-
-def test_get_dataloader() -> None:
-    dataset = ADJUSTED_TOKEN_DATA.copy()
-    dataset["id"] = list(range(len(dataset["input_ids"])))
-    ds = datasets.Dataset.from_dict(dataset)
-    loader = get_dataloader(ds)
-    assert len(loader.dataset) == len(mock_ds)
-    assert sorted(list(loader.dataset[2].keys())) == sorted(
-        ["id", "input_ids", "attention_mask", "labels"]
+    ```
+    """
+    manager = TCDatasetManager()
+    dd = manager.get_dataset_dict(
+        hf_data,
+        hf_inference_names,
+        train_data,
+        val_data,
+        test_data,
+        inference_data,
+        labels,
     )
-
-
-def test_validate_dataset_no_tags() -> None:
-    dataset = UNADJUSTED_TOKEN_DATA.copy()
-    dataset.pop("ner_tags")
-    ds = datasets.Dataset.from_dict(dataset)
-    dd = datasets.DatasetDict({"train": ds})
-    with pytest.raises(GalileoException) as e:
-        _validate_dataset(dd)
-
-    assert str(e.value) == "Each dataset must have either ner_tags or tags"
-
-
-def test_validate_dataset_converts_tags_to_ner_tags() -> None:
-    dataset = UNADJUSTED_TOKEN_DATA.copy()
-    dataset["tags"] = dataset.pop("ner_tags")
-    ds = datasets.Dataset.from_dict(dataset)
-    dd = datasets.DatasetDict({"train": ds})
-    dd = _validate_dataset(dd)
-    assert "tags" not in dd["train"].features
-    assert "ner_tags" in dd["train"].features
-
-
-def test_extract_labels_from_ds_ner_labels() -> None:
-    dataset = UNADJUSTED_TOKEN_DATA.copy()
-    dataset["ner_labels"] = [["A", "B", "C"] for _ in range(len(dataset["ner_tags"]))]
-    ds = datasets.Dataset.from_dict(dataset)
-    dd = datasets.DatasetDict({"train": ds})
-    assert _extract_labels_from_ds(dd) == ["A", "B", "C"]
-
-
-def test_extract_labels_from_ds_no_labels() -> None:
-    dataset = ADJUSTED_TOKEN_DATA.copy()
-    ds = datasets.Dataset.from_dict(dataset)
-    dd = datasets.DatasetDict({"train": ds})
-    with pytest.raises(GalileoException) as e:
-        _extract_labels_from_ds(dd)
-    assert str(e.value).startswith("Could not extract labels from Dataset.")
-
-
-def test_tokenize_and_log_dataset_invalid_labels() -> None:
-    dd = datasets.DatasetDict({"train": mock_ds})
-    with pytest.raises(AssertionError) as e:
-        tokenize_and_log_dataset(dd, mock_tokenizer, np.array(["a", "b", "c"]))
-    assert str(e.value).startswith("label_names must be of type list, but got")
-
-
-@pytest.mark.skipif(sys.version_info < (3, 8), reason="requires python3.8 or higher")
-@mock.patch("dataquality.log_dataset")
-def test_tokenize_and_log_dataset_with_meta(
-    mock_log_dataset: mock.MagicMock, set_test_config
-) -> None:
-    """Tests that with meta columns, they will be logged"""
-    set_test_config(task_type="text_ner")
-    tokenize_output = tokenize_adjust_labels(mock_ds, mock_tokenizer, tag_names)
-
-    mock_ds_meta = mock_ds.add_column("test_meta_1", ["a", "b", "c", "d", "e"])
-    with mock.patch("dataquality.integrations.hf.tokenize_adjust_labels") as mock_tok:
-        mock_tok.return_value = tokenize_output
-        # Only test and val have meta, make sure they both get logged with meta
-        ds_dict = datasets.DatasetDict(
-            {"train": mock_ds, "test": mock_ds_meta, "validation": mock_ds_meta}
-        )
-        output = tokenize_and_log_dataset(ds_dict, mock_tokenizer, meta=["test_meta_1"])
-    for split in ds_dict.keys():
-        split_output = output[split]
-        for k in ADJUSTED_TOKEN_DATA:
-            token_data = ADJUSTED_TOKEN_DATA[k]
-            if k == "text_token_indices":
-                # We abuse token data because outputs are returning tuples but we want
-                # to compare lists
-                token_data = json.loads(json.dumps(token_data))
-            assert token_data == split_output[k]
-    assert mock_log_dataset.call_count == 3
-    call_args = mock_log_dataset.call_args_list
-
-    # Training has no meta
-    assert call_args[0][-1]["meta"] == []
-    # Test and val do have meta
-    assert call_args[1][-1]["meta"] == ["test_meta_1"]
-    assert call_args[2][-1]["meta"] == ["test_meta_1"]
-
-
-def test_validate_dataset_filters_empty_tokens(set_test_config: Callable) -> None:
-    set_test_config(task_type="text_ner")
-    empty_example = {
-        "tokens": [["Swansea", "1", "Lincoln", "2"], []],
-        "ner_tags": [[3, 0, 3, 0], []],
-    }
-    dd = datasets.DatasetDict({"train": datasets.Dataset.from_dict(empty_example)})
-    assert dd["train"].num_rows == 2
-    dd = _validate_dataset(dd)
-    assert dd["train"].num_rows == 1
+    labels = _get_labels(dd, labels)
+    dq.login()
+    a.log_function("auto/tc")
+    if not run_name and isinstance(hf_data, str):
+        run_name = run_name_from_hf_dataset(hf_data)
+    dq.init(TaskType.text_classification, project_name=project_name, run_name=run_name)
+    dq.set_labels_for_run(labels)
+    _log_dataset_dict(dd)
+    trainer, encoded_data = get_trainer(
+        dd, labels, hf_model, max_padding_length, num_train_epochs
+    )
+    return do_train(trainer, encoded_data, wait, create_data_embs)
```

### Comparing `dataquality-0.8.9/tests/test_dataquality.py` & `dataquality-0.9.0a0/tests/test_dataquality.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,29 +20,32 @@
 from dataquality.loggers.data_logger import BaseGalileoDataLogger
 from dataquality.loggers.model_logger import BaseGalileoModelLogger
 from dataquality.loggers.model_logger.text_classification import (
     TextClassificationModelLogger,
 )
 from dataquality.schemas.task_type import TaskType
 from dataquality.utils.thread_pool import ThreadPoolManager
-from tests.conftest import TEST_PATH
+from tests.conftest import TestSessionVariables
 from tests.test_utils.data_utils import (
     NUM_LOGS,
     NUM_RECORDS,
     _log_text_classification_data,
     validate_cleanup_data,
     validate_uploaded_data,
 )
 
 MAX_META_COLS = BaseGalileoDataLogger.MAX_META_COLS
 MAX_STR_LEN = BaseGalileoDataLogger.MAX_STR_LEN
+MAX_DOC_LEN = BaseGalileoDataLogger.MAX_DOC_LEN
 
 
 def test_threaded_logging_and_upload(
-    cleanup_after_use: Callable, set_test_config: Callable
+    cleanup_after_use: Callable,
+    set_test_config: Callable,
+    test_session_vars: TestSessionVariables,
 ) -> None:
     """
     Tests that threaded calls to upload still yield non-missing datasets
     """
     num_records = 32
     num_logs = 20
     num_embs = 50
@@ -51,24 +54,29 @@
     )
     try:
         # Equivalent to the users `finish` call, but we don't want to clean up files yet
         ThreadPoolManager.wait_for_threads()
         c = dataquality.get_data_logger("text_classification")
         c.validate_labels()
         c.upload()
-        validate_uploaded_data(num_records * num_logs)
+        validate_uploaded_data(
+            test_session_vars=test_session_vars,
+            expected_num_records=num_records * num_logs,
+        )
         c._cleanup()
-        validate_cleanup_data()
+        validate_cleanup_data(test_session_vars=test_session_vars)
     finally:
         # Mock finish() call without calling the API
         ThreadPoolManager.wait_for_threads()
 
 
 def test_multi_label_logging(
-    cleanup_after_use: Callable, set_test_config: Callable
+    cleanup_after_use: Callable,
+    set_test_config: Callable,
+    test_session_vars: TestSessionVariables,
 ) -> None:
     """
     Tests that threaded calls to upload still yield non-missing datasets
     """
     set_test_config(task_type=TaskType.text_multi_label)
     num_records = 32
     num_logs = 20
@@ -78,48 +86,57 @@
     )
     try:
         # Equivalent to the users `finish` call, but we don't want to clean up files yet
         ThreadPoolManager.wait_for_threads()
         c = dataquality.get_data_logger()
         c.validate_labels()
         c.upload()
-        validate_uploaded_data(num_records * num_logs, multi_label=True)
+        validate_uploaded_data(
+            test_session_vars=test_session_vars,
+            expected_num_records=num_records * num_logs,
+            multi_label=True,
+        )
         c._cleanup()
-        validate_cleanup_data()
+        validate_cleanup_data(test_session_vars=test_session_vars)
     finally:
         # Mock finish() call without calling the API
         ThreadPoolManager.wait_for_threads()
 
 
 def test_metadata_logging(
-    cleanup_after_use: Callable, set_test_config: Callable
+    cleanup_after_use: Callable,
+    set_test_config: Callable,
+    test_session_vars: TestSessionVariables,
 ) -> None:
     """
     Tests that logging metadata columns persist
     """
     meta_cols = ["test1", "meta2"]
     meta = {}
     for i in meta_cols:
         meta[i] = [random() for _ in range(NUM_RECORDS * NUM_LOGS)]
     _log_text_classification_data(meta=meta)
     try:
         # Equivalent to the users `finish` call, but we don't want to clean up files yet
         ThreadPoolManager.wait_for_threads()
         c = dataquality.get_data_logger()
         c.upload()
-        validate_uploaded_data(meta_cols=meta_cols)
+        validate_uploaded_data(test_session_vars=test_session_vars, meta_cols=meta_cols)
         c._cleanup()
-        validate_cleanup_data()
+        validate_cleanup_data(test_session_vars=test_session_vars)
     finally:
         # Mock finish() call without calling the API
         ThreadPoolManager.wait_for_threads()
 
 
 def test_metadata_logging_different_splits(
-    cleanup_after_use: Callable, set_test_config: Callable, input_data: Callable
+    cleanup_after_use: Callable,
+    set_test_config: Callable,
+    input_data: Callable,
+    test_session_vars: TestSessionVariables,
 ) -> None:
     """
     Tests that logging metadata columns only attach to the splits we log them for
     """
     training_data = input_data(meta={"training_meta": [1, 2]})
     dataquality.set_labels_for_run(training_data["labels"])
     dataquality.log_data_samples(**training_data)
@@ -134,16 +151,16 @@
         "epoch": 0,
     }
     dataquality.log_model_outputs(**output_data)
     output_data["split"] = "test"
     dataquality.log_model_outputs(**output_data)
     dataquality.get_data_logger().upload()
 
-    train_data = vaex.open(f"{TEST_PATH}/training/0/data/data.hdf5")
-    test_data = vaex.open(f"{TEST_PATH}/test/0/data/data.hdf5")
+    train_data = vaex.open(f"{test_session_vars.TEST_PATH}/training/0/data/data.hdf5")
+    test_data = vaex.open(f"{test_session_vars.TEST_PATH}/test/0/data/data.hdf5")
 
     assert "training_meta" in train_data.get_column_names()
     assert "training_meta" not in test_data.get_column_names()
 
     assert "test_meta" in test_data.get_column_names()
     assert "test_meta" not in train_data.get_column_names()
 
@@ -156,40 +173,42 @@
 ) -> None:
     """
     Tests our metadata logging validation
     """
     meta = {
         "test1": [random() for _ in range(NUM_RECORDS * NUM_LOGS)],
         "meta2": [random() for _ in range(NUM_RECORDS * NUM_LOGS)],
-        "bad_attr": [
+        "doc1": ["te" * MAX_STR_LEN for _ in range(NUM_RECORDS * NUM_LOGS)],
+        "doc2": ["te" * MAX_STR_LEN for _ in range(NUM_RECORDS * NUM_LOGS)],
+        "doc3": ["te" * MAX_STR_LEN for _ in range(NUM_RECORDS * NUM_LOGS)],
+        "too_many_doc": [
             "te" * MAX_STR_LEN for _ in range(NUM_RECORDS * NUM_LOGS)
+        ],  # 4th doc, ignored
+        "doc_too_long": [
+            "te" * MAX_DOC_LEN for _ in range(NUM_RECORDS * NUM_LOGS)
         ],  # String too long
         "another_bad_attr": ["test", "test", "test"],  # Wrong number of values
         # Right length, but can't contain a list
         "bad_attr_3": [[1]] + [random() for _ in range(NUM_RECORDS * NUM_LOGS - 1)],
         "gold": [random() for _ in range(NUM_RECORDS * NUM_LOGS)],  # Reserved key
     }
 
     # Too many metadata columns
     for i in range(MAX_META_COLS):
         meta[f"attr_{i}"] = [random() for _ in range(NUM_RECORDS * NUM_LOGS)]
 
-    _log_text_classification_data(meta=meta)
-    valid_meta_cols = ["test1", "meta2"]
-    valid_meta_cols += [f"attr_{i}" for i in range(MAX_META_COLS - len(meta))]
-    try:
-        # Equivalent to the users `finish` call, but we don't want to clean up files yet
-        c = dataquality.get_data_logger("text_classification")
-        c.upload()
-        validate_uploaded_data(meta_cols=valid_meta_cols)
-        c._cleanup()
-        validate_cleanup_data()
-    finally:
-        # Mock finish() call without calling the API
-        ThreadPoolManager.wait_for_threads()
+    c = dataquality.get_data_logger("text_classification")
+    c.meta = meta
+    c.validate_metadata(NUM_RECORDS * NUM_LOGS)
+
+    removed_cols = ["too_many_doc", "doc_too_long", "another_bad_attr", "bad_attr_3"]
+    for col in removed_cols:
+        assert col not in c.meta
+
+    assert len(c.meta) == MAX_META_COLS
 
 
 def test_logging_duplicate_ids(
     cleanup_after_use: Callable, set_test_config: Callable
 ) -> None:
     """
     Tests that logging duplicate ids triggers a failure
@@ -208,21 +227,25 @@
         )
     finally:
         # Mock finish() call without calling the API
         ThreadPoolManager.wait_for_threads()
 
 
 def test_logging_inference_run(
-    cleanup_after_use: Callable, set_test_config: Callable, input_data: Callable
+    cleanup_after_use: Callable,
+    set_test_config: Callable,
+    input_data: Callable,
+    test_session_vars: TestSessionVariables,
 ) -> None:
     """
     Tests that logging metadata columns only attach to the splits we log them for
     """
     inference_data = input_data(
-        split="inference", meta={"inference_meta_1": [3.14, 42]}
+        split="inference",
+        meta={"inference_meta_1": np.array([3.14, 42], dtype=np.float32)},
     )
     dataquality.log_data_samples(**inference_data)
     inference_data = input_data(split="inference", inference_name="last-week-customers")
     dataquality.log_data_samples(**inference_data)
 
     dataquality.set_split("inference", inference_name="all-customers")
     embs_1 = np.random.rand(2, 100)
@@ -242,53 +265,65 @@
         "ids": [1, 2],
     }
     dataquality.log_model_outputs(**output_data)
 
     ThreadPoolManager.wait_for_threads()
     dataquality.get_data_logger().upload()
 
-    inference_data_1 = vaex.open(f"{TEST_PATH}/inference/all-customers/data/data.hdf5")
+    inference_data_1 = vaex.open(
+        f"{test_session_vars.TEST_PATH}/inference/all-customers/data/data.hdf5"
+    )
     inference_data_2 = vaex.open(
-        f"{TEST_PATH}/inference/last-week-customers/data/data.hdf5"
+        f"{test_session_vars.TEST_PATH}/inference/last-week-customers/data/data.hdf5"
     )
 
     assert "inference_meta_1" in inference_data_1.get_column_names()
     assert "inference_meta_1" not in inference_data_2.get_column_names()
-    assert sorted(inference_data_1["inference_meta_1"].tolist()) == [3.14, 42]
+    # Compare each pair of float numbers within the tolerance level (1e-6)
+    actual = sorted(inference_data_1["inference_meta_1"].tolist())
+    expected = [3.14, 42]
+    assert all(a == pytest.approx(e, abs=1e-6) for a, e in zip(actual, expected))
 
-    inference_emb_1 = vaex.open(f"{TEST_PATH}/inference/all-customers/emb/emb.hdf5")
+    inference_emb_1 = vaex.open(
+        f"{test_session_vars.TEST_PATH}/inference/all-customers/emb/emb.hdf5"
+    )
     inference_emb_2 = vaex.open(
-        f"{TEST_PATH}/inference/last-week-customers/emb/emb.hdf5"
+        f"{test_session_vars.TEST_PATH}/inference/last-week-customers/emb/emb.hdf5"
     )
 
-    assert (inference_emb_1.emb.to_numpy() == embs_1).all()
-    assert (inference_emb_2.emb.to_numpy() == embs_2).all()
+    assert np.isclose(inference_emb_1.emb.to_numpy(), embs_1).all()
+    assert np.isclose(inference_emb_2.emb.to_numpy(), embs_2).all()
 
-    inference_prob_1 = vaex.open(f"{TEST_PATH}/inference/all-customers/prob/prob.hdf5")
+    inference_prob_1 = vaex.open(
+        f"{test_session_vars.TEST_PATH}/inference/all-customers/prob/prob.hdf5"
+    )
     inference_prob_2 = vaex.open(
-        f"{TEST_PATH}/inference/last-week-customers/prob/prob.hdf5"
+        f"{test_session_vars.TEST_PATH}/inference/last-week-customers/prob/prob.hdf5"
     )
 
     assert "logits" not in inference_prob_1.get_column_names()
     assert "logits" not in inference_prob_2.get_column_names()
     assert "prob" in inference_prob_1.get_column_names()
     assert "prob" in inference_prob_2.get_column_names()
 
-    assert (
-        inference_prob_1.prob.to_numpy()
-        == dataquality.get_model_logger()().convert_logits_to_probs(logits_1)
+    assert np.isclose(
+        inference_prob_1.prob.to_numpy(),
+        dataquality.get_model_logger().convert_logits_to_probs(logits_1),
     ).all()
-    assert (
-        inference_prob_2.prob.to_numpy()
-        == dataquality.get_model_logger()().convert_logits_to_probs(logits_2)
+    assert np.isclose(
+        inference_prob_2.prob.to_numpy(),
+        dataquality.get_model_logger().convert_logits_to_probs(logits_2),
     ).all()
 
 
 def test_logging_train_test_inference(
-    cleanup_after_use: Callable, set_test_config: Callable, input_data: Callable
+    cleanup_after_use: Callable,
+    set_test_config: Callable,
+    input_data: Callable,
+    test_session_vars: TestSessionVariables,
 ) -> None:
     """
     Tests that logging metadata columns only attach to the splits we log them for
     """
     dataquality.set_labels_for_run(["APPLE", "ORANGE"])
     training_data = input_data(meta={"training_meta": [1.414, 123]})
     dataquality.log_data_samples(**training_data)
@@ -321,76 +356,93 @@
         "ids": [1, 2],
     }
     dataquality.log_model_outputs(**output_data)
 
     ThreadPoolManager.wait_for_threads()
     dataquality.get_data_logger().upload()
 
-    train_data = vaex.open(f"{TEST_PATH}/training/0/data/data.hdf5")
-    test_data = vaex.open(f"{TEST_PATH}/test/0/data/data.hdf5")
-    inference_data = vaex.open(f"{TEST_PATH}/inference/all-customers/data/data.hdf5")
+    train_data = vaex.open(f"{test_session_vars.TEST_PATH}/training/0/data/data.hdf5")
+    test_data = vaex.open(f"{test_session_vars.TEST_PATH}/test/0/data/data.hdf5")
+    inference_data = vaex.open(
+        f"{test_session_vars.TEST_PATH}/inference/all-customers/data/data.hdf5"
+    )
 
     assert "training_meta" in train_data.get_column_names()
-    assert sorted(train_data["training_meta"].tolist()) == [1.414, 123]
+    # Compare each pair of float numbers within the tolerance level (1e-6)
+    actual = sorted(train_data["training_meta"].tolist())
+    expected = [1.414, 123]
+    assert all(a == pytest.approx(e, abs=1e-6) for a, e in zip(actual, expected))
+
     assert "test_meta" in test_data.get_column_names()
-    assert sorted(test_data["test_meta"].tolist()) == [3.14, 42]
+    actual = sorted(test_data["test_meta"].tolist())
+    expected = [3.14, 42]
+    assert all(a == pytest.approx(e, abs=1e-6) for a, e in zip(actual, expected))
+
+    train_emb_data = vaex.open(f"{test_session_vars.TEST_PATH}/training/0/emb/emb.hdf5")
+    test_emb_data = vaex.open(f"{test_session_vars.TEST_PATH}/test/0/emb/emb.hdf5")
+    inference_emb_data = vaex.open(
+        f"{test_session_vars.TEST_PATH}/inference/all-customers/emb/emb.hdf5"
+    )
 
-    train_emb_data = vaex.open(f"{TEST_PATH}/training/0/emb/emb.hdf5")
-    test_emb_data = vaex.open(f"{TEST_PATH}/test/0/emb/emb.hdf5")
-    inference_emb_data = vaex.open(f"{TEST_PATH}/inference/all-customers/emb/emb.hdf5")
-
-    assert (train_emb_data.emb.to_numpy() == train_embs).all()
-    assert (test_emb_data.emb.to_numpy() == test_embs).all()
-    assert (inference_emb_data.emb.to_numpy() == inf_embs).all()
+    assert np.isclose(train_emb_data.emb.to_numpy(), train_embs).all()
+    assert np.isclose(test_emb_data.emb.to_numpy(), test_embs).all()
+    assert np.isclose(inference_emb_data.emb.to_numpy(), inf_embs).all()
 
-    train_prob_data = vaex.open(f"{TEST_PATH}/training/0/prob/prob.hdf5")
-    test_prob_data = vaex.open(f"{TEST_PATH}/test/0/prob/prob.hdf5")
+    train_prob_data = vaex.open(
+        f"{test_session_vars.TEST_PATH}/training/0/prob/prob.hdf5"
+    )
+    test_prob_data = vaex.open(f"{test_session_vars.TEST_PATH}/test/0/prob/prob.hdf5")
     inference_prob_data = vaex.open(
-        f"{TEST_PATH}/inference/all-customers/prob/prob.hdf5"
+        f"{test_session_vars.TEST_PATH}/inference/all-customers/prob/prob.hdf5"
     )
 
     assert "training_meta" in train_data.get_column_names()
     assert "training_meta" not in test_data.get_column_names()
     assert "training_meta" not in inference_data.get_column_names()
 
     assert "test_meta" not in train_data.get_column_names()
     assert "test_meta" in test_data.get_column_names()
     assert "test_meta" not in inference_data.get_column_names()
 
     assert "logits" not in train_prob_data.get_column_names()
     assert "logits" not in test_prob_data.get_column_names()
     assert "logits" not in inference_prob_data.get_column_names()
 
-    assert (
-        train_prob_data.prob.to_numpy()
-        == dataquality.get_model_logger()().convert_logits_to_probs(train_logits)
+    assert np.isclose(
+        train_prob_data.prob.to_numpy(),
+        dataquality.get_model_logger().convert_logits_to_probs(train_logits),
     ).all()
-    assert (
-        test_prob_data.prob.to_numpy()
-        == dataquality.get_model_logger()().convert_logits_to_probs(test_logits)
+    assert np.isclose(
+        test_prob_data.prob.to_numpy(),
+        dataquality.get_model_logger().convert_logits_to_probs(test_logits),
     ).all()
-    assert (
-        inference_prob_data.prob.to_numpy()
-        == dataquality.get_model_logger()().convert_logits_to_probs(inf_logits)
+    assert np.isclose(
+        inference_prob_data.prob.to_numpy(),
+        dataquality.get_model_logger().convert_logits_to_probs(inf_logits),
     ).all()
 
 
 def test_prob_only(set_test_config) -> None:
     """Tests that the last_epoch is determined at the split level"""
     logger = dataquality.get_data_logger()
     logger.logger_config.last_epoch = 5
     train_split_runs = ["0", "1", "5", "3", "4"]
     val_split_runs = ["0", "1", "3", "4"]
     test_split_runs = ["0"]
 
-    assert logger.prob_only(train_split_runs, "training", "0")
-    assert not logger.prob_only(train_split_runs, "training", "5")
-    assert logger.prob_only(val_split_runs, "validation", "0")
-    assert not logger.prob_only(val_split_runs, "validation", "5")
-    assert not logger.prob_only(test_split_runs, "test", "0")
+    assert logger.prob_only(train_split_runs, "training", "0", last_epoch=None)
+    assert not logger.prob_only(train_split_runs, "training", "5", last_epoch=None)
+    # Last epoch of 9 is invalid because the largest epoch is 5
+    assert not logger.prob_only(test_split_runs, "test", "5", last_epoch=9)
+    assert not logger.prob_only(train_split_runs, "training", "3", last_epoch=4)
+    assert logger.prob_only(val_split_runs, "validation", "0", last_epoch=None)
+    assert not logger.prob_only(val_split_runs, "validation", "5", last_epoch=None)
+    assert not logger.prob_only(test_split_runs, "test", "0", last_epoch=None)
+    # Last epoch of 2 is invalid because the largest epoch is 0
+    assert not logger.prob_only(test_split_runs, "test", "0", last_epoch=2)
 
 
 @mock.patch.object(dataquality.clients.api.ApiClient, "get_presigned_url")
 @mock.patch.object(
     dataquality.clients.objectstore.ObjectStore, "_upload_file_from_local"
 )
 def test_log_invalid_model_outputs(
@@ -647,15 +699,15 @@
 )
 @mock.patch.object(
     dataquality.loggers.model_logger.base_model_logger.BaseGalileoModelLogger,
     "_get_data_dict",
 )
 @mock.patch.object(
     dataquality.loggers.model_logger.base_model_logger.BaseGalileoModelLogger,
-    "validate",
+    "validate_and_format",
 )
 def test_log_batch_error_warns(
     mock_validate: mock.MagicMock,
     mock_get_data: mock.MagicMock,
     mock_write: mock.MagicMock,
     set_test_config: Callable,
 ) -> None:
@@ -675,15 +727,15 @@
 )
 @mock.patch.object(
     dataquality.loggers.model_logger.base_model_logger.BaseGalileoModelLogger,
     "_get_data_dict",
 )
 @mock.patch.object(
     dataquality.loggers.model_logger.base_model_logger.BaseGalileoModelLogger,
-    "validate",
+    "validate_and_format",
 )
 def test_log_assertion_error_raises(
     mock_validate: mock.MagicMock,
     mock_get_data: mock.MagicMock,
     mock_write: mock.MagicMock,
     set_test_config: Callable,
     cleanup_after_use: Callable,
```

### Comparing `dataquality-0.8.9/tests/test_telemetrics.py` & `dataquality-0.9.0a0/tests/test_telemetrics.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.9/tests/test_utils/data_utils.py` & `dataquality-0.9.0a0/tests/test_utils/data_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,42 +7,47 @@
 import pandas as pd
 import vaex
 from sklearn.datasets import fetch_20newsgroups
 from tqdm import tqdm
 
 import dataquality
 from dataquality.schemas.split import Split
-from tests.conftest import LOCATION, SPLITS, SUBDIRS, TEST_PATH
+from tests.conftest import SPLITS, SUBDIRS, TestSessionVariables
 
 NUM_RECORDS = 50
 NUM_LOGS = 30
 MULTI_LABEL_NUM_TASKS = 4
 
 
 def validate_uploaded_data(
-    expected_num_records: int = None,
+    test_session_vars: TestSessionVariables,
+    expected_num_records: Optional[int] = None,
     meta_cols: Optional[List] = None,
     multi_label=False,
 ) -> None:
     """
     Checks for testing
     """
     expected_num_records = expected_num_records or NUM_RECORDS * NUM_LOGS
     meta_cols = meta_cols or {}
     for split in SPLITS:
         # Output data
         split_output_data = {}
         for subdir in SUBDIRS:
             # epoch = 0 for general testing
             try:
-                file_path = f"{TEST_PATH}/{split}/0/{subdir}/{subdir}.hdf5"
+                file_path = (
+                    f"{test_session_vars.TEST_PATH}/{split}/0/{subdir}/{subdir}.hdf5"
+                )
                 data = vaex.open(file_path)
             except FileNotFoundError:
                 # Handle autolog test
-                file_path = f"{TEST_PATH}/{split}/1/{subdir}/{subdir}.hdf5"
+                file_path = (
+                    f"{test_session_vars.TEST_PATH}/{split}/1/{subdir}/{subdir}.hdf5"
+                )
                 data = vaex.open(file_path)
 
             prob_cols = data.get_column_names(regex="prob*")
             for c in data.get_column_names():
                 if c in prob_cols + ["emb"]:
                     assert not np.isnan(data[c].values).any()
                 else:
@@ -77,21 +82,21 @@
                 len(prob.get_column_names(regex="prob*"))
                 == len(prob.get_column_names(regex="gold*"))
                 == len(data.get_column_names(regex="pred*"))
                 == MULTI_LABEL_NUM_TASKS
             )
 
 
-def validate_cleanup_data():
+def validate_cleanup_data(test_session_vars: TestSessionVariables):
     """
     Checks for testing
     """
     for split in SPLITS:
         # Ensure files were cleaned up
-        assert not os.path.isdir(f"{LOCATION}/{split}")
+        assert not os.path.isdir(f"{test_session_vars.LOCATION}/{split}")
 
 
 def _log_text_classification_data(
     num_records=NUM_RECORDS,
     num_logs=NUM_LOGS,
     unique_ids=True,
     num_embs=20,
```

### Comparing `dataquality-0.8.9/tests/test_utils/hf_integration_constants.py` & `dataquality-0.9.0a0/tests/test_utils/hf_integration_constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -455,19 +455,28 @@
 mock_batch_encoding.word_ids = lambda batch_index: BATCH_WORD_IDS[batch_index]
 mock_batch_encoding._encodings = [BatchTokens(tokens) for tokens in BATCH_TOKENS]
 
 # We mock the tokenizer so we don't need to use the real tokenizer from hf
 mock_tokenizer = mock.Mock()
 mock_tokenizer.batch_encode_plus.return_value = mock_batch_encoding
 
-# We mock the hf dataset so we don't need to download a dataset from hf
-mock_ds = datasets.Dataset.from_dict(UNADJUSTED_TOKEN_DATA)
 tag_names = [
     "O",
     "B-PER",
     "I-PER",
     "B-ORG",
     "I-ORG",
     "B-LOC",
     "I-LOC",
 ]
-mock_ds.features["ner_tags"].feature.names = tag_names
+# We mock the hf dataset so we don't need to download a dataset from hf
+mock_ds = datasets.Dataset.from_dict(
+    UNADJUSTED_TOKEN_DATA,
+    # features=datasets.Features({"ner_tags": datasets.Features(names=tag_names)}),
+)
+new_features = mock_ds.features.copy()
+new_features["ner_tags"] = datasets.Sequence(
+    feature=datasets.ClassLabel(names=tag_names),
+    length=-1,
+    id=None,
+)
+mock_ds = mock_ds.cast(new_features)
```

### Comparing `dataquality-0.8.9/tests/test_utils/hf_integration_constants_inference.py` & `dataquality-0.9.0a0/tests/test_utils/hf_integration_constants_inference.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.9/tests/test_utils/lightning_model.py` & `dataquality-0.9.0a0/tests/test_utils/lightning_model.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.8.9/tests/test_utils/mock_request.py` & `dataquality-0.9.0a0/tests/test_utils/mock_request.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, List, Union
+from typing import Dict, List, Optional, Union
 from uuid import uuid4
 
 import dataquality
 from dataquality import __version__
 
 config = dataquality.config
 
@@ -13,15 +13,15 @@
 
 
 class MockResponse:
     def __init__(
         self,
         json_data: Union[Dict, List],
         status_code: int,
-        headers: Dict = None,
+        headers: Optional[Dict] = None,
     ) -> None:
         self.headers = headers or {}
         self.json_data = json_data
         self.status_code = status_code
         if status_code in (200, 204):
             self.ok = True
         else:
@@ -51,14 +51,15 @@
 def mocked_login_requests(
     request_url: str,
     json: Dict = {},
     params: Dict = {},
     headers: Dict = {},
     data: Dict = {},
     timeout: Union[int, None] = None,
+    files: Union[Dict, None] = None,
 ) -> MockResponse:
     if request_url.endswith("login"):
         return MockResponse(
             {
                 "access_token": "mock_token",
             },
             200,
@@ -71,59 +72,77 @@
 def mocked_failed_login_requests(
     request_url: str,
     json: Dict = {},
     params: Dict = {},
     headers: Dict = {},
     data: Dict = {},
     timeout: Union[int, None] = None,
+    files: Union[Dict, None] = None,
 ) -> MockResponse:
     if request_url.endswith("login"):
         return MockResponse({"detail": "Incorrect login credentials."}, 404)
     return MockResponse({}, 404)
 
 
 def mocked_get_project_run(
     request_url: str,
     json: Dict,
     params: Dict,
     headers: Dict,
     data: Dict,
     timeout: Union[int, None] = None,
+    files: Union[Dict, None] = None,
 ) -> MockResponse:
     if request_url.endswith("current_user"):
         return MockResponse({"id": "user"}, 200)
     res = [
         {"id": uuid4(), "name": EXISTING_PROJECT, "project_id": uuid4()},
         {"id": uuid4(), "name": EXISTING_RUN, "project_id": uuid4()},
         {"id": uuid4(), "name": TMP_CREATE_NEW_PROJ_RUN, "project_id": uuid4()},
     ]
     return MockResponse(res, 200)
 
 
+def mocked_upload_image_dataset(
+    request_url: str,
+    json: Dict,
+    params: Dict,
+    headers: Dict,
+    data: Dict,
+    timeout: Union[int, None] = None,
+    files: Union[Dict, None] = None,
+) -> MockResponse:
+    if request_url.endswith("task_type=image_classfication"):
+        return MockResponse({"response": "done"}, 200)
+    return MockResponse({}, 400)
+
+
 def mocked_create_project_run(
     request_url: str,
     json: Dict,
     params: Dict,
     headers: Dict,
     data: Dict,
     timeout: Union[int, None] = None,
+    files: Union[Dict, None] = None,
 ) -> MockResponse:
     global TMP_CREATE_NEW_PROJ_RUN
     TMP_CREATE_NEW_PROJ_RUN = json["name"]
     res = {"id": uuid4(), "name": TMP_CREATE_NEW_PROJ_RUN}
     return MockResponse(res, 200)
 
 
 def mocked_missing_run(
     request_url: str,
     json: Dict,
     params: Dict,
     headers: Dict,
     data: Dict,
     timeout: Union[int, None] = None,
+    files: Union[Dict, None] = None,
 ) -> MockResponse:
     if request_url.endswith("current_user"):
         return MockResponse({"id": "user"}, 200)
     # Run does not exist
     if "run_name" in request_url:
         return MockResponse([], 204)
     # Project does exist
@@ -148,40 +167,43 @@
 def mocked_missing_project_name(
     request_url: str,
     json: Dict,
     params: Dict,
     headers: Dict,
     data: Dict,
     timeout: Union[int, None] = None,
+    files: Union[Dict, None] = None,
 ) -> MockResponse:
     if request_url.endswith("current_user"):
         return MockResponse({"id": "user"}, 200)
     return MockResponse([], 200)
 
 
 def mocked_delete_project_run(
     request_url: str,
     json: Dict,
     params: Dict,
     headers: Dict,
     data: Dict,
     timeout: Union[int, None] = None,
+    files: Union[Dict, None] = None,
 ) -> MockResponse:
     if request_url.endswith("current_user"):
         return MockResponse({"id": "user"}, 200)
     return MockResponse([{"id": uuid4(), "name": TMP_CREATE_NEW_PROJ_RUN}], 200)
 
 
 def mocked_delete_project_not_found(
     request_url: str,
     json: Dict,
     params: Dict,
     headers: Dict,
     data: Dict,
     timeout: Union[int, None] = None,
+    files: Union[Dict, None] = None,
 ) -> MockResponse:
     if request_url.endswith("current_user"):
         return MockResponse({"id": "user"}, 200)
     return MockResponse({"detail": "project not found"}, 404)
 
 
 def mocked_login() -> None:
```

### Comparing `dataquality-0.8.9/tests/test_utils/ner_constants.py` & `dataquality-0.9.0a0/tests/test_utils/ner_constants.py`

 * *Files identical despite different names*

