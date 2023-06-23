# Comparing `tmp/bob.bio.base-8.0.0.tar.gz` & `tmp/bob.bio.base-8.0.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bob.bio.base-8.0.0.tar", last modified: Fri Jun 16 12:49:17 2023, max compression
+gzip compressed data, was "bob.bio.base-8.0.1b0.tar", last modified: Fri Jun 23 19:31:01 2023, max compression
```

## Comparing `bob.bio.base-8.0.0.tar` & `bob.bio.base-8.0.1b0.tar`

### file list

```diff
@@ -1,136 +1,136 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:49:17.819888 bob.bio.base-8.0.0/
--rw-rw-rw-   0 root         (0) root         (0)     1541 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      123 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3438 2023-06-16 12:49:17.819888 bob.bio.base-8.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2416 2023-06-16 12:43:44.000000 bob.bio.base-8.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:49:17.795889 bob.bio.base-8.0.0/doc/
--rw-rw-rw-   0 root         (0) root         (0)     1066 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/doc/annotators.rst
--rw-rw-rw-   0 root         (0) root         (0)    24372 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/doc/biometrics_intro.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:49:17.795889 bob.bio.base-8.0.0/doc/code_samples/
--rw-rw-rw-   0 root         (0) root         (0)     2457 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/doc/code_samples/pipeline_example.py
--rw-rw-rw-   0 root         (0) root         (0)     7503 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/doc/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     5440 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/doc/database_interface.rst
--rw-rw-rw-   0 root         (0) root         (0)     4411 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/doc/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     8159 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/doc/legacy.rst
--rw-rw-rw-   0 root         (0) root         (0)     1052 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/doc/links.rst
--rw-rw-rw-   0 root         (0) root         (0)     4351 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/doc/pipeline_score_norm.rst
--rw-rw-rw-   0 root         (0) root         (0)    31484 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/doc/pipeline_simple_features.rst
--rw-rw-rw-   0 root         (0) root         (0)    12635 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/doc/pipeline_simple_intro.rst
--rw-rw-rw-   0 root         (0) root         (0)     3735 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/doc/py_api.rst
--rw-rw-rw-   0 root         (0) root         (0)    14247 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/doc/vulnerability_analysis.rst
--rw-rw-rw-   0 root         (0) root         (0)     5790 2023-06-16 12:43:44.000000 bob.bio.base-8.0.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-16 12:49:17.819888 bob.bio.base-8.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      125 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:49:17.787889 bob.bio.base-8.0.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:49:17.795889 bob.bio.base-8.0.0/src/bob/
--rw-rw-rw-   0 root         (0) root         (0)      129 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:49:17.799888 bob.bio.base-8.0.0/src/bob/bio/
--rw-rw-rw-   0 root         (0) root         (0)      129 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:49:17.799888 bob.bio.base-8.0.0/src/bob/bio/base/
--rw-rw-rw-   0 root         (0) root         (0)      465 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:49:17.799888 bob.bio.base-8.0.0/src/bob/bio/base/algorithm/
--rw-rw-rw-   0 root         (0) root         (0)      698 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/algorithm/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7173 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/algorithm/distance.py
--rw-rw-rw-   0 root         (0) root         (0)    10231 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/algorithm/gmm.py
--rw-rw-rw-   0 root         (0) root         (0)     1596 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/algorithm/isv.py
--rw-rw-rw-   0 root         (0) root         (0)     1596 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/algorithm/jfa.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:49:17.799888 bob.bio.base-8.0.0/src/bob/bio/base/annotator/
--rw-rw-rw-   0 root         (0) root         (0)      976 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/annotator/Annotator.py
--rw-rw-rw-   0 root         (0) root         (0)      691 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/annotator/Callable.py
--rw-rw-rw-   0 root         (0) root         (0)     3731 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/annotator/FailSafe.py
--rw-rw-rw-   0 root         (0) root         (0)      724 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/annotator/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:49:17.799888 bob.bio.base-8.0.0/src/bob/bio/base/config/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 12:48:55.000000 bob.bio.base-8.0.0/src/bob/bio/base/config/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:49:17.799888 bob.bio.base-8.0.0/src/bob/bio/base/config/database/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 12:48:55.000000 bob.bio.base-8.0.0/src/bob/bio/base/config/database/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       80 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/config/database/atnt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:49:17.803888 bob.bio.base-8.0.0/src/bob/bio/base/config/dummy/
--rw-rw-rw-   0 root         (0) root         (0)       54 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/config/dummy/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      886 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/config/dummy/annotator.py
--rw-rw-rw-   0 root         (0) root         (0)      349 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/config/dummy/config.py
--rw-rw-rw-   0 root         (0) root         (0)       42 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/config/dummy/config2.py
--rw-rw-rw-   0 root         (0) root         (0)       80 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/config/dummy/database.py
--rw-rw-rw-   0 root         (0) root         (0)     1184 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/config/dummy/extractor.py
--rw-rw-rw-   0 root         (0) root         (0)      467 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/config/dummy/pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)     1150 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/config/dummy/preprocessor.py
--rw-rw-rw-   0 root         (0) root         (0)      407 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/config/dummy/samples_list.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:49:17.803888 bob.bio.base-8.0.0/src/bob/bio/base/database/
--rw-rw-rw-   0 root         (0) root         (0)     1062 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/database/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3142 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/database/atnt.py
--rw-rw-rw-   0 root         (0) root         (0)    21050 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/database/csv_database.py
--rw-rw-rw-   0 root         (0) root         (0)    36323 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/database/database.py
--rw-rw-rw-   0 root         (0) root         (0)     5114 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/database/file.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:49:17.807888 bob.bio.base-8.0.0/src/bob/bio/base/database/filelist/
--rw-rw-rw-   0 root         (0) root         (0)      677 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/database/filelist/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9611 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/database/filelist/models.py
--rw-rw-rw-   0 root         (0) root         (0)    38099 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/database/filelist/query.py
--rw-rw-rw-   0 root         (0) root         (0)    18189 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/database/legacy.py
--rw-rw-rw-   0 root         (0) root         (0)    19732 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/database/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:49:17.807888 bob.bio.base-8.0.0/src/bob/bio/base/extractor/
--rw-rw-rw-   0 root         (0) root         (0)     6600 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/extractor/Extractor.py
--rw-rw-rw-   0 root         (0) root         (0)      610 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/extractor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:49:17.807888 bob.bio.base-8.0.0/src/bob/bio/base/pipelines/
--rw-rw-rw-   0 root         (0) root         (0)     1674 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/pipelines/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16779 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/pipelines/abstract_classes.py
--rw-rw-rw-   0 root         (0) root         (0)    23824 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/pipelines/entry_points.py
--rw-rw-rw-   0 root         (0) root         (0)     8279 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/pipelines/pipelines.py
--rw-rw-rw-   0 root         (0) root         (0)    25442 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/pipelines/score_post_processor.py
--rw-rw-rw-   0 root         (0) root         (0)     5572 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/pipelines/score_writers.py
--rw-rw-rw-   0 root         (0) root         (0)    12829 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/pipelines/wrappers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:49:17.807888 bob.bio.base-8.0.0/src/bob/bio/base/preprocessor/
--rw-rw-rw-   0 root         (0) root         (0)     4782 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/preprocessor/Preprocessor.py
--rw-rw-rw-   0 root         (0) root         (0)      619 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/preprocessor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:49:17.807888 bob.bio.base-8.0.0/src/bob/bio/base/score/
--rw-rw-rw-   0 root         (0) root         (0)      287 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/score/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    23647 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/score/load.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:49:17.811888 bob.bio.base-8.0.0/src/bob/bio/base/script/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 12:48:55.000000 bob.bio.base-8.0.0/src/bob/bio/base/script/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7047 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/script/annotate.py
--rw-rw-rw-   0 root         (0) root         (0)      327 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/script/bio.py
--rw-rw-rw-   0 root         (0) root         (0)     7506 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/script/commands.py
--rw-rw-rw-   0 root         (0) root         (0)     2690 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/script/compare_samples.py
--rw-rw-rw-   0 root         (0) root         (0)    17409 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/script/error_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    11955 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/script/figure.py
--rw-rw-rw-   0 root         (0) root         (0)    10934 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/script/gen.py
--rw-rw-rw-   0 root         (0) root         (0)      272 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/script/pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)     7079 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/script/pipeline_score_norm.py
--rw-rw-rw-   0 root         (0) root         (0)     9271 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/script/pipeline_simple.py
--rw-rw-rw-   0 root         (0) root         (0)     6596 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/script/pipeline_train.py
--rw-rw-rw-   0 root         (0) root         (0)     6465 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/script/pipeline_transform.py
--rw-rw-rw-   0 root         (0) root         (0)     3713 2023-06-14 13:38:45.000000 bob.bio.base-8.0.0/src/bob/bio/base/script/resources.py
--rw-rw-rw-   0 root         (0) root         (0)      905 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/script/sort.py
--rw-rw-rw-   0 root         (0) root         (0)    16642 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/script/vuln_commands.py
--rw-rw-rw-   0 root         (0) root         (0)    42424 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/script/vuln_figure.py
--rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/script/vulnerability.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:49:17.815888 bob.bio.base-8.0.0/src/bob/bio/base/transformers/
--rw-rw-rw-   0 root         (0) root         (0)     1047 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/transformers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2029 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/transformers/extractor.py
--rw-rw-rw-   0 root         (0) root         (0)     1259 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/transformers/preprocessing.py
--rw-rw-rw-   0 root         (0) root         (0)     1321 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/transformers/preprocessor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:49:17.815888 bob.bio.base-8.0.0/src/bob/bio/base/utils/
--rw-rw-rw-   0 root         (0) root         (0)     3563 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5912 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/utils/annotations.py
--rw-rw-rw-   0 root         (0) root         (0)     6781 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/utils/io.py
--rw-rw-rw-   0 root         (0) root         (0)    12299 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/utils/resources.py
--rw-rw-rw-   0 root         (0) root         (0)     8932 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/src/bob/bio/base/wrappers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:49:17.799888 bob.bio.base-8.0.0/src/bob.bio.base.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3438 2023-06-16 12:49:17.000000 bob.bio.base-8.0.0/src/bob.bio.base.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3833 2023-06-16 12:49:17.000000 bob.bio.base-8.0.0/src/bob.bio.base.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 12:49:17.000000 bob.bio.base-8.0.0/src/bob.bio.base.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1997 2023-06-16 12:49:17.000000 bob.bio.base-8.0.0/src/bob.bio.base.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 12:49:17.000000 bob.bio.base-8.0.0/src/bob.bio.base.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      569 2023-06-16 12:49:17.000000 bob.bio.base-8.0.0/src/bob.bio.base.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-06-16 12:49:17.000000 bob.bio.base-8.0.0/src/bob.bio.base.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:49:17.819888 bob.bio.base-8.0.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1614 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/tests/test_algorithms.py
--rw-rw-rw-   0 root         (0) root         (0)     2408 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/tests/test_annotators.py
--rw-rw-rw-   0 root         (0) root         (0)    21381 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/tests/test_commands.py
--rw-rw-rw-   0 root         (0) root         (0)     2540 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/tests/test_database_implementations.py
--rw-rw-rw-   0 root         (0) root         (0)    24391 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/tests/test_filelist.py
--rw-rw-rw-   0 root         (0) root         (0)     5792 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/tests/test_gen.py
--rw-rw-rw-   0 root         (0) root         (0)     6500 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/tests/test_io.py
--rw-rw-rw-   0 root         (0) root         (0)    16743 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/tests/test_pipeline_post_process_score.py
--rw-rw-rw-   0 root         (0) root         (0)    17940 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/tests/test_pipeline_simple.py
--rw-rw-rw-   0 root         (0) root         (0)     4015 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/tests/test_pipeline_train.py
--rw-rw-rw-   0 root         (0) root         (0)     5444 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/tests/test_transformers.py
--rw-rw-rw-   0 root         (0) root         (0)      954 2023-06-12 19:25:08.000000 bob.bio.base-8.0.0/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:31:01.731152 bob.bio.base-8.0.1b0/
+-rw-rw-rw-   0 root         (0) root         (0)     1541 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      123 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3440 2023-06-23 19:31:01.731152 bob.bio.base-8.0.1b0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2416 2023-06-23 13:50:30.000000 bob.bio.base-8.0.1b0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:31:01.711152 bob.bio.base-8.0.1b0/doc/
+-rw-rw-rw-   0 root         (0) root         (0)     1066 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/doc/annotators.rst
+-rw-rw-rw-   0 root         (0) root         (0)    24372 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/doc/biometrics_intro.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:31:01.711152 bob.bio.base-8.0.1b0/doc/code_samples/
+-rw-rw-rw-   0 root         (0) root         (0)     2457 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/doc/code_samples/pipeline_example.py
+-rw-rw-rw-   0 root         (0) root         (0)     7503 2023-06-23 19:24:56.000000 bob.bio.base-8.0.1b0/doc/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     5440 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/doc/database_interface.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4411 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/doc/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     8159 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/doc/legacy.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/doc/links.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4351 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/doc/pipeline_score_norm.rst
+-rw-rw-rw-   0 root         (0) root         (0)    31484 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/doc/pipeline_simple_features.rst
+-rw-rw-rw-   0 root         (0) root         (0)    12635 2023-06-23 19:24:56.000000 bob.bio.base-8.0.1b0/doc/pipeline_simple_intro.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3735 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/doc/py_api.rst
+-rw-rw-rw-   0 root         (0) root         (0)    14247 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/doc/vulnerability_analysis.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5460 2023-06-23 19:24:56.000000 bob.bio.base-8.0.1b0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 19:31:01.731152 bob.bio.base-8.0.1b0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      125 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:31:01.703152 bob.bio.base-8.0.1b0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:31:01.711152 bob.bio.base-8.0.1b0/src/bob/
+-rw-rw-rw-   0 root         (0) root         (0)      129 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:31:01.711152 bob.bio.base-8.0.1b0/src/bob/bio/
+-rw-rw-rw-   0 root         (0) root         (0)      129 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:31:01.711152 bob.bio.base-8.0.1b0/src/bob/bio/base/
+-rw-rw-rw-   0 root         (0) root         (0)      465 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:31:01.715152 bob.bio.base-8.0.1b0/src/bob/bio/base/algorithm/
+-rw-rw-rw-   0 root         (0) root         (0)      698 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/algorithm/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7173 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/algorithm/distance.py
+-rw-rw-rw-   0 root         (0) root         (0)    10231 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/algorithm/gmm.py
+-rw-rw-rw-   0 root         (0) root         (0)     1596 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/algorithm/isv.py
+-rw-rw-rw-   0 root         (0) root         (0)     1596 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/algorithm/jfa.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:31:01.715152 bob.bio.base-8.0.1b0/src/bob/bio/base/annotator/
+-rw-rw-rw-   0 root         (0) root         (0)      976 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/annotator/Annotator.py
+-rw-rw-rw-   0 root         (0) root         (0)      691 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/annotator/Callable.py
+-rw-rw-rw-   0 root         (0) root         (0)     3731 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/annotator/FailSafe.py
+-rw-rw-rw-   0 root         (0) root         (0)      724 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/annotator/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:31:01.715152 bob.bio.base-8.0.1b0/src/bob/bio/base/config/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-23 19:30:38.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/config/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:31:01.715152 bob.bio.base-8.0.1b0/src/bob/bio/base/config/database/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-23 19:30:38.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/config/database/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       80 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/config/database/atnt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:31:01.715152 bob.bio.base-8.0.1b0/src/bob/bio/base/config/dummy/
+-rw-rw-rw-   0 root         (0) root         (0)       54 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/config/dummy/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      886 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/config/dummy/annotator.py
+-rw-rw-rw-   0 root         (0) root         (0)      349 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/config/dummy/config.py
+-rw-rw-rw-   0 root         (0) root         (0)       42 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/config/dummy/config2.py
+-rw-rw-rw-   0 root         (0) root         (0)       80 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/config/dummy/database.py
+-rw-rw-rw-   0 root         (0) root         (0)     1184 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/config/dummy/extractor.py
+-rw-rw-rw-   0 root         (0) root         (0)      467 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/config/dummy/pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)     1150 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/config/dummy/preprocessor.py
+-rw-rw-rw-   0 root         (0) root         (0)      407 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/config/dummy/samples_list.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:31:01.719152 bob.bio.base-8.0.1b0/src/bob/bio/base/database/
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/database/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3142 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/database/atnt.py
+-rw-rw-rw-   0 root         (0) root         (0)    21050 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/database/csv_database.py
+-rw-rw-rw-   0 root         (0) root         (0)    36323 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/database/database.py
+-rw-rw-rw-   0 root         (0) root         (0)     5114 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/database/file.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:31:01.719152 bob.bio.base-8.0.1b0/src/bob/bio/base/database/filelist/
+-rw-rw-rw-   0 root         (0) root         (0)      677 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/database/filelist/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9611 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/database/filelist/models.py
+-rw-rw-rw-   0 root         (0) root         (0)    38099 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/database/filelist/query.py
+-rw-rw-rw-   0 root         (0) root         (0)    18189 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/database/legacy.py
+-rw-rw-rw-   0 root         (0) root         (0)    19732 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/database/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:31:01.719152 bob.bio.base-8.0.1b0/src/bob/bio/base/extractor/
+-rw-rw-rw-   0 root         (0) root         (0)     6600 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/extractor/Extractor.py
+-rw-rw-rw-   0 root         (0) root         (0)      610 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/extractor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:31:01.723152 bob.bio.base-8.0.1b0/src/bob/bio/base/pipelines/
+-rw-rw-rw-   0 root         (0) root         (0)     1674 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/pipelines/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16779 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/pipelines/abstract_classes.py
+-rw-rw-rw-   0 root         (0) root         (0)    23824 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/pipelines/entry_points.py
+-rw-rw-rw-   0 root         (0) root         (0)     8279 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/pipelines/pipelines.py
+-rw-rw-rw-   0 root         (0) root         (0)    25442 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/pipelines/score_post_processor.py
+-rw-rw-rw-   0 root         (0) root         (0)     5572 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/pipelines/score_writers.py
+-rw-rw-rw-   0 root         (0) root         (0)    12829 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/pipelines/wrappers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:31:01.723152 bob.bio.base-8.0.1b0/src/bob/bio/base/preprocessor/
+-rw-rw-rw-   0 root         (0) root         (0)     4782 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/preprocessor/Preprocessor.py
+-rw-rw-rw-   0 root         (0) root         (0)      619 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/preprocessor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:31:01.723152 bob.bio.base-8.0.1b0/src/bob/bio/base/score/
+-rw-rw-rw-   0 root         (0) root         (0)      287 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/score/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    23647 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/score/load.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:31:01.727152 bob.bio.base-8.0.1b0/src/bob/bio/base/script/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-23 19:30:38.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/script/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7047 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/script/annotate.py
+-rw-rw-rw-   0 root         (0) root         (0)      327 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/script/bio.py
+-rw-rw-rw-   0 root         (0) root         (0)     7506 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/script/commands.py
+-rw-rw-rw-   0 root         (0) root         (0)     2690 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/script/compare_samples.py
+-rw-rw-rw-   0 root         (0) root         (0)    17409 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/script/error_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    11955 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/script/figure.py
+-rw-rw-rw-   0 root         (0) root         (0)    10934 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/script/gen.py
+-rw-rw-rw-   0 root         (0) root         (0)      272 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/script/pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)     7079 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/script/pipeline_score_norm.py
+-rw-rw-rw-   0 root         (0) root         (0)     9271 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/script/pipeline_simple.py
+-rw-rw-rw-   0 root         (0) root         (0)     6596 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/script/pipeline_train.py
+-rw-rw-rw-   0 root         (0) root         (0)     6465 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/script/pipeline_transform.py
+-rw-rw-rw-   0 root         (0) root         (0)     3713 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/script/resources.py
+-rw-rw-rw-   0 root         (0) root         (0)      905 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/script/sort.py
+-rw-rw-rw-   0 root         (0) root         (0)    16642 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/script/vuln_commands.py
+-rw-rw-rw-   0 root         (0) root         (0)    42424 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/script/vuln_figure.py
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/script/vulnerability.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:31:01.727152 bob.bio.base-8.0.1b0/src/bob/bio/base/transformers/
+-rw-rw-rw-   0 root         (0) root         (0)     1047 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/transformers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2029 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/transformers/extractor.py
+-rw-rw-rw-   0 root         (0) root         (0)     1259 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/transformers/preprocessing.py
+-rw-rw-rw-   0 root         (0) root         (0)     1321 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/transformers/preprocessor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:31:01.727152 bob.bio.base-8.0.1b0/src/bob/bio/base/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     3563 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5912 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/utils/annotations.py
+-rw-rw-rw-   0 root         (0) root         (0)     6781 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/utils/io.py
+-rw-rw-rw-   0 root         (0) root         (0)    12299 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/utils/resources.py
+-rw-rw-rw-   0 root         (0) root         (0)     8932 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/src/bob/bio/base/wrappers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:31:01.711152 bob.bio.base-8.0.1b0/src/bob.bio.base.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3440 2023-06-23 19:31:01.000000 bob.bio.base-8.0.1b0/src/bob.bio.base.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3833 2023-06-23 19:31:01.000000 bob.bio.base-8.0.1b0/src/bob.bio.base.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 19:31:01.000000 bob.bio.base-8.0.1b0/src/bob.bio.base.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1997 2023-06-23 19:31:01.000000 bob.bio.base-8.0.1b0/src/bob.bio.base.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 19:31:01.000000 bob.bio.base-8.0.1b0/src/bob.bio.base.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      372 2023-06-23 19:31:01.000000 bob.bio.base-8.0.1b0/src/bob.bio.base.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-06-23 19:31:01.000000 bob.bio.base-8.0.1b0/src/bob.bio.base.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:31:01.731152 bob.bio.base-8.0.1b0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1614 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/tests/test_algorithms.py
+-rw-rw-rw-   0 root         (0) root         (0)     2408 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/tests/test_annotators.py
+-rw-rw-rw-   0 root         (0) root         (0)    21381 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/tests/test_commands.py
+-rw-rw-rw-   0 root         (0) root         (0)     2540 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/tests/test_database_implementations.py
+-rw-rw-rw-   0 root         (0) root         (0)    24391 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/tests/test_filelist.py
+-rw-rw-rw-   0 root         (0) root         (0)     5792 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/tests/test_gen.py
+-rw-rw-rw-   0 root         (0) root         (0)     6500 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/tests/test_io.py
+-rw-rw-rw-   0 root         (0) root         (0)    16743 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/tests/test_pipeline_post_process_score.py
+-rw-rw-rw-   0 root         (0) root         (0)    17940 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/tests/test_pipeline_simple.py
+-rw-rw-rw-   0 root         (0) root         (0)     4015 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/tests/test_pipeline_train.py
+-rw-rw-rw-   0 root         (0) root         (0)     5444 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/tests/test_transformers.py
+-rw-rw-rw-   0 root         (0) root         (0)      954 2023-06-23 00:34:16.000000 bob.bio.base-8.0.1b0/tests/test_utils.py
```

### Comparing `bob.bio.base-8.0.0/LICENSE` & `bob.bio.base-8.0.1b0/LICENSE`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/PKG-INFO` & `bob.bio.base-8.0.1b0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: bob.bio.base
-Version: 8.0.0
+Version: 8.0.1b0
 Summary: Tools for running biometric recognition experiments
 Author-email: Manuel Gunther <siebenkopf@googlemail.com>
 License: BSD 3-Clause License
-Project-URL: documentation, https://www.idiap.ch/software/bob/docs/bob/bob.bio.base/v8.0.0/sphinx/
+Project-URL: documentation, https://www.idiap.ch/software/bob/docs/bob/bob.bio.base/master/sphinx/
 Project-URL: homepage, https://pypi.org/project/bob.bio.base/
 Project-URL: repository, https://gitlab.idiap.ch/bob/bob.bio.base
 Project-URL: changelog, https://gitlab.idiap.ch/bob/bob.bio.base/-/releases
 Keywords: bob,biometric recognition,evaluation
 Classifier: Framework :: Bob
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -19,17 +19,17 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: qa
 Provides-Extra: doc
 Provides-Extra: test
 License-File: LICENSE
 
-[![badge doc](https://img.shields.io/badge/docs-v8.0.0-orange.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.bio.base/v8.0.0/sphinx/index.html)
-[![badge pipeline](https://gitlab.idiap.ch/bob/bob.bio.base/badges/v8.0.0/pipeline.svg)](https://gitlab.idiap.ch/bob/bob.bio.base/commits/v8.0.0)
-[![badge coverage](https://gitlab.idiap.ch/bob/bob.bio.base/badges/v8.0.0/coverage.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.bio.base/v8.0.0/coverage)
+[![badge doc](https://img.shields.io/badge/docs-latest-orange.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.bio.base/master/sphinx/index.html)
+[![badge pipeline](https://gitlab.idiap.ch/bob/bob.bio.base/badges/master/pipeline.svg)](https://gitlab.idiap.ch/bob/bob.bio.base/commits/master)
+[![badge coverage](https://gitlab.idiap.ch/bob/bob.bio.base/badges/master/coverage.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.bio.base/master/coverage)
 [![badge gitlab](https://img.shields.io/badge/gitlab-project-0000c0.svg)](https://gitlab.idiap.ch/bob/bob.bio.base)
 
 # Tools to run biometric recognition experiments
 
 This package is part of the signal-processing and machine learning toolbox
 [Bob](https://www.idiap.ch/software/bob). It provides tools to run comparable
 and reproducible biometric recognition experiments on publicly available
```

### Comparing `bob.bio.base-8.0.0/README.md` & `bob.bio.base-8.0.1b0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-[![badge doc](https://img.shields.io/badge/docs-v8.0.0-orange.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.bio.base/v8.0.0/sphinx/index.html)
-[![badge pipeline](https://gitlab.idiap.ch/bob/bob.bio.base/badges/v8.0.0/pipeline.svg)](https://gitlab.idiap.ch/bob/bob.bio.base/commits/v8.0.0)
-[![badge coverage](https://gitlab.idiap.ch/bob/bob.bio.base/badges/v8.0.0/coverage.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.bio.base/v8.0.0/coverage)
+[![badge doc](https://img.shields.io/badge/docs-latest-orange.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.bio.base/master/sphinx/index.html)
+[![badge pipeline](https://gitlab.idiap.ch/bob/bob.bio.base/badges/master/pipeline.svg)](https://gitlab.idiap.ch/bob/bob.bio.base/commits/master)
+[![badge coverage](https://gitlab.idiap.ch/bob/bob.bio.base/badges/master/coverage.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.bio.base/master/coverage)
 [![badge gitlab](https://img.shields.io/badge/gitlab-project-0000c0.svg)](https://gitlab.idiap.ch/bob/bob.bio.base)
 
 # Tools to run biometric recognition experiments
 
 This package is part of the signal-processing and machine learning toolbox
 [Bob](https://www.idiap.ch/software/bob). It provides tools to run comparable
 and reproducible biometric recognition experiments on publicly available
```

### Comparing `bob.bio.base-8.0.0/doc/annotators.rst` & `bob.bio.base-8.0.1b0/doc/annotators.rst`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/doc/biometrics_intro.rst` & `bob.bio.base-8.0.1b0/doc/biometrics_intro.rst`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/doc/code_samples/pipeline_example.py` & `bob.bio.base-8.0.1b0/doc/code_samples/pipeline_example.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/doc/conf.py` & `bob.bio.base-8.0.1b0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/doc/database_interface.rst` & `bob.bio.base-8.0.1b0/doc/database_interface.rst`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/doc/index.rst` & `bob.bio.base-8.0.1b0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/doc/legacy.rst` & `bob.bio.base-8.0.1b0/doc/legacy.rst`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/doc/links.rst` & `bob.bio.base-8.0.1b0/doc/links.rst`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/doc/pipeline_score_norm.rst` & `bob.bio.base-8.0.1b0/doc/pipeline_score_norm.rst`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/doc/pipeline_simple_features.rst` & `bob.bio.base-8.0.1b0/doc/pipeline_simple_features.rst`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/doc/pipeline_simple_intro.rst` & `bob.bio.base-8.0.1b0/doc/pipeline_simple_intro.rst`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/doc/py_api.rst` & `bob.bio.base-8.0.1b0/doc/py_api.rst`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/doc/vulnerability_analysis.rst` & `bob.bio.base-8.0.1b0/doc/vulnerability_analysis.rst`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/pyproject.toml` & `bob.bio.base-8.0.1b0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
     requires = ["setuptools>=61.0.0", "wheel"]
     build-backend = "setuptools.build_meta"
 
 [project]
     name = "bob.bio.base"
-    version = "8.0.0"
+    version = "8.0.1b0"
     requires-python = ">=3.9"
     description = "Tools for running biometric recognition experiments"
     dynamic = ["readme"]
     license = {text = "BSD 3-Clause License"}
     authors = [
     {name = "Manuel Gunther", email = "siebenkopf@googlemail.com"},
     ]
@@ -20,57 +20,57 @@
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
         "Natural Language :: English",
         "Programming Language :: Python",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
     ]
     dependencies = [
-        "bob==12.0.0",
-        "bob.io.base==5.1.0",
-        "bob.learn.em==3.3.0",
-        "bob.measure==6.1.0",
-        "bob.pipelines==4.0.0",
-        "clapper==1.0.1",
-        "click==8.1.3",
-        "click-plugins==1.1.1",
-        "dask==2023.1.0",
-        "numpy==1.23.5",
-        "pandas==1.5.2",
-        "scipy==1.10.0",
-        "setuptools==66.0.0",
-        "tabulate==0.9.0",
+        "bob",
+        "bob.io.base",
+        "bob.learn.em",
+        "bob.measure",
+        "bob.pipelines",
+        "clapper",
+        "click",
+        "click-plugins",
+        "dask",
+        "numpy",
+        "pandas",
+        "scipy",
+        "setuptools",
+        "tabulate",
     ]
 
 [project.urls]
-    documentation = "https://www.idiap.ch/software/bob/docs/bob/bob.bio.base/v8.0.0/sphinx/"
+    documentation = "https://www.idiap.ch/software/bob/docs/bob/bob.bio.base/master/sphinx/"
     homepage = "https://pypi.org/project/bob.bio.base/"
     repository = "https://gitlab.idiap.ch/bob/bob.bio.base"
     changelog = "https://gitlab.idiap.ch/bob/bob.bio.base/-/releases"
 
 [project.optional-dependencies]
     qa = ["pre-commit"]
     doc = [
-        "sphinx==5.3.0",
-        "sphinx-rtd-theme==1.1.1",
-        "sphinx-autodoc-typehints==1.21.8",
-        "auto-intersphinx==1.0.2",
-        "sphinxcontrib-programoutput==0.17",
-        "matplotlib==3.6.2",
-        "dask-ml==2022.5.27",
+        "sphinx",
+        "sphinx_rtd_theme",
+        "sphinx-autodoc-typehints",
+        "auto-intersphinx",
+        "sphinxcontrib-programoutput",
+        "matplotlib",
+        "dask-ml",
         "bob.bio.face",
         "bob.bio.vein",
         "bob.bio.spear",
         "bob.bio.video",
         ]
     test = [
-        "pytest==7.2.1",
-        "pytest-cov==4.0.0",
-        "coverage==7.0.5",
-        "dask-ml==2022.5.27",
-        "matplotlib==3.6.2",
+        "pytest",
+        "pytest-cov",
+        "coverage",
+        "dask-ml",
+        "matplotlib",
         ]
 
 [tool.setuptools]
     zip-safe = false
     package-dir = {"" = "src"}
 
 [tool.setuptools.dynamic]
@@ -147,11 +147,7 @@
     addopts = [
     "--import-mode=append",
     "--cov-report=term-missing",
     "--cov=bob.bio.base",
     ]
     junit_logging = "all"
     junit_log_passing_tests = false
-
-[profile]
-    repository_url = "git@gitlab.idiap.ch:bob/dev-profile.git"
-    commit_hash = "ade723be1f11feddb7bece235de32cc98953dc07"
```

### Comparing `bob.bio.base-8.0.0/src/bob/bio/base/algorithm/__init__.py` & `bob.bio.base-8.0.1b0/src/bob/bio/base/algorithm/__init__.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/src/bob/bio/base/algorithm/distance.py` & `bob.bio.base-8.0.1b0/src/bob/bio/base/algorithm/distance.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/src/bob/bio/base/algorithm/gmm.py` & `bob.bio.base-8.0.1b0/src/bob/bio/base/algorithm/gmm.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/src/bob/bio/base/algorithm/isv.py` & `bob.bio.base-8.0.1b0/src/bob/bio/base/algorithm/isv.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/src/bob/bio/base/algorithm/jfa.py` & `bob.bio.base-8.0.1b0/src/bob/bio/base/algorithm/jfa.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/src/bob/bio/base/annotator/Annotator.py` & `bob.bio.base-8.0.1b0/src/bob/bio/base/annotator/Annotator.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/src/bob/bio/base/annotator/Callable.py` & `bob.bio.base-8.0.1b0/src/bob/bio/base/annotator/Callable.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/src/bob/bio/base/annotator/FailSafe.py` & `bob.bio.base-8.0.1b0/src/bob/bio/base/annotator/FailSafe.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/src/bob/bio/base/annotator/__init__.py` & `bob.bio.base-8.0.1b0/src/bob/bio/base/annotator/__init__.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/src/bob/bio/base/config/dummy/annotator.py` & `bob.bio.base-8.0.1b0/src/bob/bio/base/config/dummy/annotator.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/src/bob/bio/base/config/dummy/extractor.py` & `bob.bio.base-8.0.1b0/src/bob/bio/base/config/dummy/extractor.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/src/bob/bio/base/config/dummy/preprocessor.py` & `bob.bio.base-8.0.1b0/src/bob/bio/base/config/dummy/preprocessor.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/src/bob/bio/base/database/__init__.py` & `bob.bio.base-8.0.1b0/src/bob/bio/base/database/__init__.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/src/bob/bio/base/database/atnt.py` & `bob.bio.base-8.0.1b0/src/bob/bio/base/database/atnt.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/src/bob/bio/base/database/csv_database.py` & `bob.bio.base-8.0.1b0/src/bob/bio/base/database/csv_database.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/src/bob/bio/base/database/database.py` & `bob.bio.base-8.0.1b0/src/bob/bio/base/database/database.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/src/bob/bio/base/database/file.py` & `bob.bio.base-8.0.1b0/src/bob/bio/base/database/file.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/src/bob/bio/base/database/filelist/__init__.py` & `bob.bio.base-8.0.1b0/src/bob/bio/base/database/filelist/__init__.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/src/bob/bio/base/database/filelist/models.py` & `bob.bio.base-8.0.1b0/src/bob/bio/base/database/filelist/models.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/src/bob/bio/base/database/filelist/query.py` & `bob.bio.base-8.0.1b0/src/bob/bio/base/database/filelist/query.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/src/bob/bio/base/database/legacy.py` & `bob.bio.base-8.0.1b0/src/bob/bio/base/database/legacy.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/src/bob/bio/base/database/utils.py` & `bob.bio.base-8.0.1b0/src/bob/bio/base/database/utils.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/src/bob/bio/base/extractor/Extractor.py` & `bob.bio.base-8.0.1b0/src/bob/bio/base/extractor/Extractor.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/src/bob/bio/base/extractor/__init__.py` & `bob.bio.base-8.0.1b0/src/bob/bio/base/extractor/__init__.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/src/bob/bio/base/pipelines/__init__.py` & `bob.bio.base-8.0.1b0/src/bob/bio/base/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/src/bob/bio/base/pipelines/abstract_classes.py` & `bob.bio.base-8.0.1b0/src/bob/bio/base/pipelines/abstract_classes.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/src/bob/bio/base/pipelines/entry_points.py` & `bob.bio.base-8.0.1b0/src/bob/bio/base/pipelines/entry_points.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/src/bob/bio/base/pipelines/pipelines.py` & `bob.bio.base-8.0.1b0/src/bob/bio/base/pipelines/pipelines.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/src/bob/bio/base/pipelines/score_post_processor.py` & `bob.bio.base-8.0.1b0/src/bob/bio/base/pipelines/score_post_processor.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/src/bob/bio/base/pipelines/score_writers.py` & `bob.bio.base-8.0.1b0/src/bob/bio/base/pipelines/score_writers.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/src/bob/bio/base/pipelines/wrappers.py` & `bob.bio.base-8.0.1b0/src/bob/bio/base/pipelines/wrappers.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/src/bob/bio/base/preprocessor/Preprocessor.py` & `bob.bio.base-8.0.1b0/src/bob/bio/base/preprocessor/Preprocessor.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/src/bob/bio/base/preprocessor/__init__.py` & `bob.bio.base-8.0.1b0/src/bob/bio/base/preprocessor/__init__.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/src/bob/bio/base/score/load.py` & `bob.bio.base-8.0.1b0/src/bob/bio/base/score/load.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/src/bob/bio/base/script/annotate.py` & `bob.bio.base-8.0.1b0/src/bob/bio/base/script/annotate.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/src/bob/bio/base/script/commands.py` & `bob.bio.base-8.0.1b0/src/bob/bio/base/script/commands.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/src/bob/bio/base/script/compare_samples.py` & `bob.bio.base-8.0.1b0/src/bob/bio/base/script/compare_samples.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/src/bob/bio/base/script/error_utils.py` & `bob.bio.base-8.0.1b0/src/bob/bio/base/script/error_utils.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/src/bob/bio/base/script/figure.py` & `bob.bio.base-8.0.1b0/src/bob/bio/base/script/figure.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/src/bob/bio/base/script/gen.py` & `bob.bio.base-8.0.1b0/src/bob/bio/base/script/gen.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/src/bob/bio/base/script/pipeline_score_norm.py` & `bob.bio.base-8.0.1b0/src/bob/bio/base/script/pipeline_score_norm.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/src/bob/bio/base/script/pipeline_simple.py` & `bob.bio.base-8.0.1b0/src/bob/bio/base/script/pipeline_simple.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/src/bob/bio/base/script/pipeline_train.py` & `bob.bio.base-8.0.1b0/src/bob/bio/base/script/pipeline_train.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/src/bob/bio/base/script/pipeline_transform.py` & `bob.bio.base-8.0.1b0/src/bob/bio/base/script/pipeline_transform.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/src/bob/bio/base/script/resources.py` & `bob.bio.base-8.0.1b0/src/bob/bio/base/script/resources.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/src/bob/bio/base/script/sort.py` & `bob.bio.base-8.0.1b0/src/bob/bio/base/script/sort.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/src/bob/bio/base/script/vuln_commands.py` & `bob.bio.base-8.0.1b0/src/bob/bio/base/script/vuln_commands.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/src/bob/bio/base/script/vuln_figure.py` & `bob.bio.base-8.0.1b0/src/bob/bio/base/script/vuln_figure.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/src/bob/bio/base/transformers/__init__.py` & `bob.bio.base-8.0.1b0/src/bob/bio/base/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/src/bob/bio/base/transformers/extractor.py` & `bob.bio.base-8.0.1b0/src/bob/bio/base/transformers/extractor.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/src/bob/bio/base/transformers/preprocessing.py` & `bob.bio.base-8.0.1b0/src/bob/bio/base/transformers/preprocessing.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/src/bob/bio/base/transformers/preprocessor.py` & `bob.bio.base-8.0.1b0/src/bob/bio/base/transformers/preprocessor.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/src/bob/bio/base/utils/__init__.py` & `bob.bio.base-8.0.1b0/src/bob/bio/base/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/src/bob/bio/base/utils/annotations.py` & `bob.bio.base-8.0.1b0/src/bob/bio/base/utils/annotations.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/src/bob/bio/base/utils/io.py` & `bob.bio.base-8.0.1b0/src/bob/bio/base/utils/io.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/src/bob/bio/base/utils/resources.py` & `bob.bio.base-8.0.1b0/src/bob/bio/base/utils/resources.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/src/bob/bio/base/wrappers.py` & `bob.bio.base-8.0.1b0/src/bob/bio/base/wrappers.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/src/bob.bio.base.egg-info/PKG-INFO` & `bob.bio.base-8.0.1b0/src/bob.bio.base.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: bob.bio.base
-Version: 8.0.0
+Version: 8.0.1b0
 Summary: Tools for running biometric recognition experiments
 Author-email: Manuel Gunther <siebenkopf@googlemail.com>
 License: BSD 3-Clause License
-Project-URL: documentation, https://www.idiap.ch/software/bob/docs/bob/bob.bio.base/v8.0.0/sphinx/
+Project-URL: documentation, https://www.idiap.ch/software/bob/docs/bob/bob.bio.base/master/sphinx/
 Project-URL: homepage, https://pypi.org/project/bob.bio.base/
 Project-URL: repository, https://gitlab.idiap.ch/bob/bob.bio.base
 Project-URL: changelog, https://gitlab.idiap.ch/bob/bob.bio.base/-/releases
 Keywords: bob,biometric recognition,evaluation
 Classifier: Framework :: Bob
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -19,17 +19,17 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: qa
 Provides-Extra: doc
 Provides-Extra: test
 License-File: LICENSE
 
-[![badge doc](https://img.shields.io/badge/docs-v8.0.0-orange.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.bio.base/v8.0.0/sphinx/index.html)
-[![badge pipeline](https://gitlab.idiap.ch/bob/bob.bio.base/badges/v8.0.0/pipeline.svg)](https://gitlab.idiap.ch/bob/bob.bio.base/commits/v8.0.0)
-[![badge coverage](https://gitlab.idiap.ch/bob/bob.bio.base/badges/v8.0.0/coverage.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.bio.base/v8.0.0/coverage)
+[![badge doc](https://img.shields.io/badge/docs-latest-orange.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.bio.base/master/sphinx/index.html)
+[![badge pipeline](https://gitlab.idiap.ch/bob/bob.bio.base/badges/master/pipeline.svg)](https://gitlab.idiap.ch/bob/bob.bio.base/commits/master)
+[![badge coverage](https://gitlab.idiap.ch/bob/bob.bio.base/badges/master/coverage.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.bio.base/master/coverage)
 [![badge gitlab](https://img.shields.io/badge/gitlab-project-0000c0.svg)](https://gitlab.idiap.ch/bob/bob.bio.base)
 
 # Tools to run biometric recognition experiments
 
 This package is part of the signal-processing and machine learning toolbox
 [Bob](https://www.idiap.ch/software/bob). It provides tools to run comparable
 and reproducible biometric recognition experiments on publicly available
```

### Comparing `bob.bio.base-8.0.0/src/bob.bio.base.egg-info/SOURCES.txt` & `bob.bio.base-8.0.1b0/src/bob.bio.base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/src/bob.bio.base.egg-info/entry_points.txt` & `bob.bio.base-8.0.1b0/src/bob.bio.base.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/tests/test_algorithms.py` & `bob.bio.base-8.0.1b0/tests/test_algorithms.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/tests/test_annotators.py` & `bob.bio.base-8.0.1b0/tests/test_annotators.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/tests/test_commands.py` & `bob.bio.base-8.0.1b0/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/tests/test_database_implementations.py` & `bob.bio.base-8.0.1b0/tests/test_database_implementations.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/tests/test_filelist.py` & `bob.bio.base-8.0.1b0/tests/test_filelist.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/tests/test_gen.py` & `bob.bio.base-8.0.1b0/tests/test_gen.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/tests/test_io.py` & `bob.bio.base-8.0.1b0/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/tests/test_pipeline_post_process_score.py` & `bob.bio.base-8.0.1b0/tests/test_pipeline_post_process_score.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/tests/test_pipeline_simple.py` & `bob.bio.base-8.0.1b0/tests/test_pipeline_simple.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/tests/test_pipeline_train.py` & `bob.bio.base-8.0.1b0/tests/test_pipeline_train.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/tests/test_transformers.py` & `bob.bio.base-8.0.1b0/tests/test_transformers.py`

 * *Files identical despite different names*

### Comparing `bob.bio.base-8.0.0/tests/test_utils.py` & `bob.bio.base-8.0.1b0/tests/test_utils.py`

 * *Files identical despite different names*

