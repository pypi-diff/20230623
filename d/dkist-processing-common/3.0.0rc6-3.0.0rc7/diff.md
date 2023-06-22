# Comparing `tmp/dkist-processing-common-3.0.0rc6.tar.gz` & `tmp/dkist-processing-common-3.0.0rc7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist-processing-common-3.0.0rc6.tar", last modified: Thu Jun 22 20:47:57 2023, max compression
+gzip compressed data, was "dkist-processing-common-3.0.0rc7.tar", last modified: Thu Jun 22 22:57:51 2023, max compression
```

## Comparing `dkist-processing-common-3.0.0rc6.tar` & `dkist-processing-common-3.0.0rc7.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 20:47:57.832761 dkist-processing-common-3.0.0rc6/
--rw-rw-rw-   0 root         (0) root         (0)     2481 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      844 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      429 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/.readthedocs.yml
--rw-rw-rw-   0 root         (0) root         (0)    13348 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     4327 2023-06-22 20:47:57.832761 dkist-processing-common-3.0.0rc6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3732 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     2433 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 20:47:57.820761 dkist-processing-common-3.0.0rc6/changelog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/changelog/.gitempty
--rw-rw-rw-   0 root         (0) root         (0)      149 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/changelog/139.feature.2.rst
--rw-rw-rw-   0 root         (0) root         (0)       85 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/changelog/139.feature.rst
--rw-rw-rw-   0 root         (0) root         (0)      342 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/changelog/140.feature.rst
--rwxrwxrwx   0 root         (0) root         (0)      642 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/check_changelog_updated.sh
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 20:47:57.820761 dkist-processing-common-3.0.0rc6/dkist_processing_common/
--rw-rw-rw-   0 root         (0) root         (0)      317 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 20:47:57.824761 dkist-processing-common-3.0.0rc6/dkist_processing_common/_util/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/_util/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1572 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/_util/config.py
--rw-rw-rw-   0 root         (0) root         (0)     2409 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/_util/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     1178 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/_util/dkist_location.py
--rw-rw-rw-   0 root         (0) root         (0)     1580 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/_util/graphql.py
--rw-rw-rw-   0 root         (0) root         (0)     8215 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/_util/scratch.py
--rw-rw-rw-   0 root         (0) root         (0)     5641 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/_util/tags.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 20:47:57.824761 dkist-processing-common-3.0.0rc6/dkist_processing_common/codecs/
--rw-rw-rw-   0 root         (0) root         (0)      159 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/codecs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      495 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/codecs/bytes.py
--rw-rw-rw-   0 root         (0) root         (0)     2030 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/codecs/fits.py
--rw-rw-rw-   0 root         (0) root         (0)      900 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/codecs/iobase.py
--rw-rw-rw-   0 root         (0) root         (0)      939 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/codecs/json.py
--rw-rw-rw-   0 root         (0) root         (0)      197 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/codecs/path.py
--rw-rw-rw-   0 root         (0) root         (0)      679 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/codecs/str.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 20:47:57.824761 dkist-processing-common-3.0.0rc6/dkist_processing_common/fonts/
--rw-rw-rw-   0 root         (0) root         (0)   656568 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/fonts/Lato-Regular.ttf
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/fonts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7037 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/manual.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 20:47:57.824761 dkist-processing-common-3.0.0rc6/dkist_processing_common/models/
--rw-rw-rw-   0 root         (0) root         (0)       74 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4766 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/models/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     3453 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/models/fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)     4176 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/models/flower_pot.py
--rw-rw-rw-   0 root         (0) root         (0)     3514 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/models/graphql.py
--rw-rw-rw-   0 root         (0) root         (0)     1109 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/models/message.py
--rw-rw-rw-   0 root         (0) root         (0)     3408 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/models/parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     2225 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/models/quality.py
--rw-rw-rw-   0 root         (0) root         (0)     1096 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/models/quality_json_encoders.py
--rw-rw-rw-   0 root         (0) root         (0)     7510 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/models/tags.py
--rw-rw-rw-   0 root         (0) root         (0)      870 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/models/wavelength.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 20:47:57.828761 dkist-processing-common-3.0.0rc6/dkist_processing_common/parsers/
--rw-rw-rw-   0 root         (0) root         (0)       67 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/parsers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6381 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/parsers/cs_step.py
--rw-rw-rw-   0 root         (0) root         (0)     1827 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/parsers/dsps_repeat.py
--rw-rw-rw-   0 root         (0) root         (0)      706 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/parsers/experiment_id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)     1767 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/parsers/id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)      921 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/parsers/l0_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)     2451 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/parsers/l1_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)      677 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/parsers/proposal_id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)     1058 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/parsers/quality.py
--rw-rw-rw-   0 root         (0) root         (0)     1230 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/parsers/single_value_single_key_flower.py
--rw-rw-rw-   0 root         (0) root         (0)     5720 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/parsers/time.py
--rw-rw-rw-   0 root         (0) root         (0)     1669 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/parsers/unique_bud.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 20:47:57.828761 dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/
--rw-rw-rw-   0 root         (0) root         (0)      504 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11470 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)    11318 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/base.py
--rw-rw-rw-   0 root         (0) root         (0)     8689 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/l1_output_data.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 20:47:57.828761 dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/mixin/
--rw-rw-rw-   0 root         (0) root         (0)       68 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/mixin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3243 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/mixin/debug_frame.py
--rw-rw-rw-   0 root         (0) root         (0)     2033 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/mixin/fits.py
--rw-rw-rw-   0 root         (0) root         (0)     6887 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/mixin/globus.py
--rw-rw-rw-   0 root         (0) root         (0)     6813 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/mixin/input_dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     2421 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/mixin/interservice_bus.py
--rw-rw-rw-   0 root         (0) root         (0)    13374 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/mixin/metadata_store.py
--rw-rw-rw-   0 root         (0) root         (0)     3612 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/mixin/object_store.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 20:47:57.828761 dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/mixin/quality/
--rw-rw-rw-   0 root         (0) root         (0)      383 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/mixin/quality/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8287 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/mixin/quality/_base.py
--rw-rw-rw-   0 root         (0) root         (0)    47886 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/mixin/quality/_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     3153 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/output_data_base.py
--rw-rw-rw-   0 root         (0) root         (0)     8329 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/parse_l0_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     8859 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/quality_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     2368 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/teardown.py
--rw-rw-rw-   0 root         (0) root         (0)     4863 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/transfer_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     7979 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/trial_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)    18550 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 20:47:57.832761 dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    24490 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     3023 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)     3060 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_base.py
--rw-rw-rw-   0 root         (0) root         (0)     7501 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_codecs.py
--rw-rw-rw-   0 root         (0) root         (0)     4203 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2291 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_cs_step.py
--rw-rw-rw-   0 root         (0) root         (0)     4097 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_debug_frame.py
--rw-rw-rw-   0 root         (0) root         (0)      513 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_dkist_location.py
--rw-rw-rw-   0 root         (0) root         (0)     4682 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_fits.py
--rw-rw-rw-   0 root         (0) root         (0)     8808 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)    12959 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_fits_flowers.py
--rw-rw-rw-   0 root         (0) root         (0)     2258 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_flower_pot.py
--rw-rw-rw-   0 root         (0) root         (0)    19450 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_input_dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     3159 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_output_data_base.py
--rw-rw-rw-   0 root         (0) root         (0)     6276 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)    10476 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_parse_l0_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     3198 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_publish_catalog_messages.py
--rw-rw-rw-   0 root         (0) root         (0)     9168 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_quality.py
--rw-rw-rw-   0 root         (0) root         (0)    36336 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_quality_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    11282 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_scratch.py
--rw-rw-rw-   0 root         (0) root         (0)     4569 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_tags.py
--rw-rw-rw-   0 root         (0) root         (0)     5745 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_teardown.py
--rw-rw-rw-   0 root         (0) root         (0)     6666 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_transfer_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     2270 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_transfer_l1_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)    11883 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_trial_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)    10527 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_workflow_task_base.py
--rw-rw-rw-   0 root         (0) root         (0)    14952 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 20:47:57.820761 dkist-processing-common-3.0.0rc6/dkist_processing_common.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     4327 2023-06-22 20:47:57.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4899 2023-06-22 20:47:57.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-22 20:47:57.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      603 2023-06-22 20:47:57.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-06-22 20:47:57.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 20:47:57.832761 dkist-processing-common-3.0.0rc6/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4598 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     1890 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      113 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     4513 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)       29 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/docs/requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 20:47:57.832761 dkist-processing-common-3.0.0rc6/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1462 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      780 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1690 2023-06-22 20:47:57.832761 dkist-processing-common-3.0.0rc6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      102 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 22:57:51.379167 dkist-processing-common-3.0.0rc7/
+-rw-rw-rw-   0 root         (0) root         (0)     2481 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      844 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      429 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/.readthedocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)    13348 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4327 2023-06-22 22:57:51.379167 dkist-processing-common-3.0.0rc7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3732 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2433 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 22:57:51.367167 dkist-processing-common-3.0.0rc7/changelog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/changelog/.gitempty
+-rw-rw-rw-   0 root         (0) root         (0)      149 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/changelog/139.feature.2.rst
+-rw-rw-rw-   0 root         (0) root         (0)       85 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/changelog/139.feature.rst
+-rw-rw-rw-   0 root         (0) root         (0)      342 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/changelog/140.feature.rst
+-rwxrwxrwx   0 root         (0) root         (0)      642 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/check_changelog_updated.sh
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 22:57:51.367167 dkist-processing-common-3.0.0rc7/dkist_processing_common/
+-rw-rw-rw-   0 root         (0) root         (0)      317 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 22:57:51.371167 dkist-processing-common-3.0.0rc7/dkist_processing_common/_util/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/_util/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1572 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/_util/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2409 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/_util/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     1178 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/_util/dkist_location.py
+-rw-rw-rw-   0 root         (0) root         (0)     1580 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/_util/graphql.py
+-rw-rw-rw-   0 root         (0) root         (0)     8215 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/_util/scratch.py
+-rw-rw-rw-   0 root         (0) root         (0)     5641 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/_util/tags.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 22:57:51.371167 dkist-processing-common-3.0.0rc7/dkist_processing_common/codecs/
+-rw-rw-rw-   0 root         (0) root         (0)      159 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/codecs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      495 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/codecs/bytes.py
+-rw-rw-rw-   0 root         (0) root         (0)     2030 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/codecs/fits.py
+-rw-rw-rw-   0 root         (0) root         (0)      900 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/codecs/iobase.py
+-rw-rw-rw-   0 root         (0) root         (0)      939 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/codecs/json.py
+-rw-rw-rw-   0 root         (0) root         (0)      197 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/codecs/path.py
+-rw-rw-rw-   0 root         (0) root         (0)      679 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/codecs/str.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 22:57:51.371167 dkist-processing-common-3.0.0rc7/dkist_processing_common/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)   656568 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/fonts/Lato-Regular.ttf
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/fonts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7037 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/manual.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 22:57:51.371167 dkist-processing-common-3.0.0rc7/dkist_processing_common/models/
+-rw-rw-rw-   0 root         (0) root         (0)       74 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4766 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/models/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     3453 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/models/fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)     4176 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/models/flower_pot.py
+-rw-rw-rw-   0 root         (0) root         (0)     3514 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/models/graphql.py
+-rw-rw-rw-   0 root         (0) root         (0)     1109 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/models/message.py
+-rw-rw-rw-   0 root         (0) root         (0)     3408 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/models/parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     2225 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/models/quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     1096 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/models/quality_json_encoders.py
+-rw-rw-rw-   0 root         (0) root         (0)     7510 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/models/tags.py
+-rw-rw-rw-   0 root         (0) root         (0)      870 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/models/wavelength.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 22:57:51.375167 dkist-processing-common-3.0.0rc7/dkist_processing_common/parsers/
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/parsers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6381 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/parsers/cs_step.py
+-rw-rw-rw-   0 root         (0) root         (0)     1827 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/parsers/dsps_repeat.py
+-rw-rw-rw-   0 root         (0) root         (0)      706 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/parsers/experiment_id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)     1767 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/parsers/id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)      921 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/parsers/l0_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)     2451 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/parsers/l1_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)      677 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/parsers/proposal_id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)     1058 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/parsers/quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     1230 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/parsers/single_value_single_key_flower.py
+-rw-rw-rw-   0 root         (0) root         (0)     5720 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/parsers/time.py
+-rw-rw-rw-   0 root         (0) root         (0)     1669 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/parsers/unique_bud.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 22:57:51.375167 dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)      504 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11470 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)    11318 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     8689 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/l1_output_data.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 22:57:51.375167 dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/mixin/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/mixin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3243 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/mixin/debug_frame.py
+-rw-rw-rw-   0 root         (0) root         (0)     2033 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/mixin/fits.py
+-rw-rw-rw-   0 root         (0) root         (0)     6887 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/mixin/globus.py
+-rw-rw-rw-   0 root         (0) root         (0)     6813 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/mixin/input_dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     2421 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/mixin/interservice_bus.py
+-rw-rw-rw-   0 root         (0) root         (0)    13374 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/mixin/metadata_store.py
+-rw-rw-rw-   0 root         (0) root         (0)     3612 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/mixin/object_store.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 22:57:51.375167 dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/mixin/quality/
+-rw-rw-rw-   0 root         (0) root         (0)      383 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/mixin/quality/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8287 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/mixin/quality/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    47886 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/mixin/quality/_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     3153 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/output_data_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     8329 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/parse_l0_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     8859 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/quality_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     2368 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/teardown.py
+-rw-rw-rw-   0 root         (0) root         (0)     4863 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/transfer_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     6844 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/trial_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    18550 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 22:57:51.379167 dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    24490 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     3023 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)     3060 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     7501 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_codecs.py
+-rw-rw-rw-   0 root         (0) root         (0)     4203 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2291 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_cs_step.py
+-rw-rw-rw-   0 root         (0) root         (0)     4097 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_debug_frame.py
+-rw-rw-rw-   0 root         (0) root         (0)      513 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_dkist_location.py
+-rw-rw-rw-   0 root         (0) root         (0)     4682 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_fits.py
+-rw-rw-rw-   0 root         (0) root         (0)     8808 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)    12959 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_fits_flowers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2258 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_flower_pot.py
+-rw-rw-rw-   0 root         (0) root         (0)    19450 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_input_dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     3159 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_output_data_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     6276 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)    10476 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_parse_l0_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     3198 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_publish_catalog_messages.py
+-rw-rw-rw-   0 root         (0) root         (0)     9168 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_quality.py
+-rw-rw-rw-   0 root         (0) root         (0)    36336 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_quality_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    11282 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_scratch.py
+-rw-rw-rw-   0 root         (0) root         (0)     4569 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_tags.py
+-rw-rw-rw-   0 root         (0) root         (0)     5745 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_teardown.py
+-rw-rw-rw-   0 root         (0) root         (0)     6666 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_transfer_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     2270 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_transfer_l1_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    11883 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_trial_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    10527 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_workflow_task_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    14952 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 22:57:51.367167 dkist-processing-common-3.0.0rc7/dkist_processing_common.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     4327 2023-06-22 22:57:51.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4899 2023-06-22 22:57:51.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-22 22:57:51.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      603 2023-06-22 22:57:51.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-06-22 22:57:51.000000 dkist-processing-common-3.0.0rc7/dkist_processing_common.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 22:57:51.379167 dkist-processing-common-3.0.0rc7/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4598 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1890 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)       29 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/docs/requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 22:57:51.379167 dkist-processing-common-3.0.0rc7/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      780 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1690 2023-06-22 22:57:51.379167 dkist-processing-common-3.0.0rc7/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      102 2023-06-22 22:57:44.000000 dkist-processing-common-3.0.0rc7/setup.py
```

### Comparing `dkist-processing-common-3.0.0rc6/.gitignore` & `dkist-processing-common-3.0.0rc7/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/.pre-commit-config.yaml` & `dkist-processing-common-3.0.0rc7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/CHANGELOG.rst` & `dkist-processing-common-3.0.0rc7/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/PKG-INFO` & `dkist-processing-common-3.0.0rc7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-common
-Version: 3.0.0rc6
+Version: 3.0.0rc7
 Summary: Common task classes used by the DKIST Science Data Processing pipelines to process DKIST data.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-common/src/master/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/common
 Classifier: Programming Language :: Python
```

### Comparing `dkist-processing-common-3.0.0rc6/README.rst` & `dkist-processing-common-3.0.0rc7/README.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/bitbucket-pipelines.yml` & `dkist-processing-common-3.0.0rc7/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/check_changelog_updated.sh` & `dkist-processing-common-3.0.0rc7/check_changelog_updated.sh`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/_util/config.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/_util/config.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/_util/constants.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/_util/constants.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/_util/dkist_location.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/_util/dkist_location.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/_util/graphql.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/_util/graphql.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/_util/scratch.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/_util/scratch.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/_util/tags.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/_util/tags.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/codecs/fits.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/codecs/fits.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/codecs/iobase.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/codecs/iobase.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/codecs/json.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/codecs/json.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/codecs/str.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/codecs/str.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/fonts/Lato-Regular.ttf` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/fonts/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/manual.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/manual.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/models/constants.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/models/constants.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/models/fits_access.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/models/fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/models/flower_pot.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/models/flower_pot.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/models/graphql.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/models/graphql.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/models/message.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/models/message.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/models/parameters.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/models/parameters.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/models/quality.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/models/quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/models/quality_json_encoders.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/models/quality_json_encoders.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/models/tags.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/models/tags.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/models/wavelength.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/models/wavelength.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/parsers/cs_step.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/parsers/cs_step.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/parsers/dsps_repeat.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/parsers/dsps_repeat.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/parsers/experiment_id_bud.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/parsers/experiment_id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/parsers/id_bud.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/parsers/id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/parsers/l0_fits_access.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/parsers/l0_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/parsers/l1_fits_access.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/parsers/l1_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/parsers/proposal_id_bud.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/parsers/proposal_id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/parsers/quality.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/parsers/quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/parsers/single_value_single_key_flower.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/parsers/single_value_single_key_flower.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/parsers/time.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/parsers/time.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/parsers/unique_bud.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/parsers/unique_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/assemble_movie.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/base.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/l1_output_data.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/l1_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/mixin/debug_frame.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/mixin/debug_frame.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/mixin/fits.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/mixin/fits.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/mixin/globus.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/mixin/globus.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/mixin/input_dataset.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/mixin/input_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/mixin/interservice_bus.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/mixin/interservice_bus.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/mixin/metadata_store.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/mixin/metadata_store.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/mixin/object_store.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/mixin/object_store.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/mixin/quality/_base.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/mixin/quality/_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/mixin/quality/_metrics.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/mixin/quality/_metrics.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/output_data_base.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/output_data_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/parse_l0_input_data.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/parse_l0_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/quality_metrics.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/quality_metrics.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/teardown.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/teardown.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/transfer_input_data.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/transfer_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/trial_output_data.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/trial_output_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -88,64 +88,14 @@
         return self.metadata_store_recipe_run_configuration().get("trial_transfer_tag_lists", [])
 
     @abstractmethod
     def build_transfer_list(self) -> list[GlobusTransferItem]:
         """Build a list of all items on scratch to transfer to the trial location."""
         pass
 
-    def build_debug_frame_transfer_list(self) -> list[GlobusTransferItem]:
-        """Build a transfer list containing all frames tagged with DEBUG."""
-        debug_frame_paths = self.read(tags=[Tag.debug(), Tag.frame()])
-        transfer_items = []
-        for p in debug_frame_paths:
-            object_key = self.format_object_key(p)
-            destination_path = Path(self.destination_bucket, object_key)
-            item = GlobusTransferItem(
-                source_path=p,
-                destination_path=destination_path,
-            )
-            transfer_items.append(item)
-
-        return transfer_items
-
-    @property
-    def intermediate_task_names(self) -> list[str]:
-        """List specifying which TASK types to build when selecting INTERMEDIATE frames."""
-        return []
-
-    def build_intermediate_frame_transfer_list(self) -> list[GlobusTransferItem]:
-        """
-        Build a transfer list containing a subset of frames tagged with INTERMEDIATE.
-
-        More specifically, the intersection of INTERMEDIATE and the tasks defined in `intermediate_task_names`.
-        """
-        transfer_items = []
-        for task in self.intermediate_task_names:
-            with self.apm_task_step(f"Build intermediate manifest for {task}"):
-                logger.info(f"Building intermediate manifest for {task}")
-                transfer_items.extend(self._build_single_task_intermediate_manifest(task=task))
-
-        return transfer_items
-
-    def _build_single_task_intermediate_manifest(self, task: str) -> list[GlobusTransferItem]:
-        """Build a transfer list containing all frames tagged with INTERMEDIATE and the given TASK."""
-        transfer_items = []
-        task_frames = self.read(tags=[Tag.intermediate(), Tag.task(task)])
-
-        for p in task_frames:
-            destination_object_key = self.format_object_key(p)
-            destination_path = Path(self.destination_bucket, destination_object_key)
-            item = GlobusTransferItem(
-                source_path=p,
-                destination_path=destination_path,
-            )
-            transfer_items.append(item)
-
-        return transfer_items
-
     def build_transfer_list_from_tag_lists(
         self, tag_lists: list[str] | list[list[str]]
     ) -> list[GlobusTransferItem]:
         """
         Build a transfer list containing all files that are tagged with any of the sets of input tags.
 
         For example, if `tag_lists` is [list1, list2,... listn] then the resulting transfer list will contain:
@@ -175,19 +125,41 @@
                     source_path=p,
                     destination_path=destination_path,
                 )
                 transfer_items.append(item)
 
         return list(set(transfer_items))
 
+    def build_debug_frame_transfer_list(self) -> list[GlobusTransferItem]:
+        """Build a transfer list containing all frames tagged with DEBUG."""
+        transfer_items = self.build_transfer_list_from_tag_lists(
+            tag_lists=[Tag.debug(), Tag.frame()]
+        )
+        return transfer_items
+
+    @property
+    def intermediate_task_names(self) -> list[str]:
+        """List specifying which TASK types to build when selecting INTERMEDIATE frames."""
+        return []
+
+    def build_intermediate_frame_transfer_list(self) -> list[GlobusTransferItem]:
+        """
+        Build a transfer list containing a subset of frames tagged with INTERMEDIATE.
+
+        More specifically, the intersection of INTERMEDIATE and the tasks defined in `intermediate_task_names`.
+        """
+        tag_lists = [[Tag.intermediate(), Tag.task(task)] for task in self.intermediate_task_names]
+        transfer_items = self.build_transfer_list_from_tag_lists(tag_lists=tag_lists)
+        return transfer_items
+
     def transfer_all_trial_frames(self, transfer_items: list[GlobusTransferItem]) -> None:
         """Send a list of transfer items to Globus for transfer."""
         logger.info(
             f"Preparing globus transfer {len(transfer_items)} items: "
             f"recipe_run_id={self.recipe_run_id}. "
             f"transfer_items={transfer_items[:3]}..."
         )
 
         self.globus_transfer_scratch_to_object_store(
             transfer_items=transfer_items,
-            label=f"Transfer science frames for recipe_run_id {self.recipe_run_id}",
+            label=f"Transfer frames for trial run of recipe_run_id {self.recipe_run_id}",
         )
```

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/write_l1.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/tasks/write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/conftest.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_assemble_movie.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_base.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_codecs.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_codecs.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_constants.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_cs_step.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_cs_step.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_debug_frame.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_debug_frame.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_dkist_location.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_dkist_location.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_fits.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_fits.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_fits_access.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_fits_flowers.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_fits_flowers.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_flower_pot.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_flower_pot.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_input_dataset.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_input_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_output_data_base.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_output_data_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_parameters.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_parse_l0_input_data.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_parse_l0_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_publish_catalog_messages.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_publish_catalog_messages.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_quality.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_quality_mixin.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_quality_mixin.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_scratch.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_scratch.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_tags.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_teardown.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_teardown.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_transfer_input_data.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_transfer_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_transfer_l1_output_data.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_transfer_l1_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_trial_output_data.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_trial_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_workflow_task_base.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_workflow_task_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_write_l1.py` & `dkist-processing-common-3.0.0rc7/dkist_processing_common/tests/test_write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common.egg-info/PKG-INFO` & `dkist-processing-common-3.0.0rc7/dkist_processing_common.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-common
-Version: 3.0.0rc6
+Version: 3.0.0rc7
 Summary: Common task classes used by the DKIST Science Data Processing pipelines to process DKIST data.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-common/src/master/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/common
 Classifier: Programming Language :: Python
```

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common.egg-info/SOURCES.txt` & `dkist-processing-common-3.0.0rc7/dkist_processing_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/dkist_processing_common.egg-info/requires.txt` & `dkist-processing-common-3.0.0rc7/dkist_processing_common.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/docs/Makefile` & `dkist-processing-common-3.0.0rc7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/docs/conf.py` & `dkist-processing-common-3.0.0rc7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/docs/make.bat` & `dkist-processing-common-3.0.0rc7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/licenses/LICENSE.rst` & `dkist-processing-common-3.0.0rc7/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/pyproject.toml` & `dkist-processing-common-3.0.0rc7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc6/setup.cfg` & `dkist-processing-common-3.0.0rc7/setup.cfg`

 * *Files identical despite different names*

