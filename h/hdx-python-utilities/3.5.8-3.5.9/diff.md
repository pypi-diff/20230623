# Comparing `tmp/hdx-python-utilities-3.5.8.tar.gz` & `tmp/hdx_python_utilities-3.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdx-python-utilities-3.5.8.tar", last modified: Tue Apr 11 03:19:41 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `hdx-python-utilities-3.5.8.tar` & `hdx_python_utilities-3.5.9.tar`

### file list

```diff
@@ -1,145 +1,122 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:19:41.780090 hdx-python-utilities-3.5.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:19:41.760089 hdx-python-utilities-3.5.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:19:41.760089 hdx-python-utilities-3.5.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/.github/workflows/run-python-tests.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1148 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/.readthedocs.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1079 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-04-11 03:19:41.780090 hdx-python-utilities-3.5.8/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     1713 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:19:41.764089 hdx-python-utilities-3.5.8/doc/
--rw-r--r--   0 runner    (1001) docker     (123)    35300 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/doc/main.md
--rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)      189 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1732 2023-04-11 03:19:41.780090 hdx-python-utilities-3.5.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:19:41.760089 hdx-python-utilities-3.5.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:19:41.760089 hdx-python-utilities-3.5.8/src/hdx/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:19:41.764089 hdx-python-utilities-3.5.8/src/hdx/utilities/
--rwxr-xr-x   0 runner    (1001) docker     (123)       59 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/src/hdx/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-11 03:19:41.000000 hdx-python-utilities-3.5.8/src/hdx/utilities/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/src/hdx/utilities/base_downloader.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      966 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/src/hdx/utilities/compare.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    35023 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/src/hdx/utilities/dateparse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15753 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/src/hdx/utilities/dictandlist.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    61799 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/src/hdx/utilities/downloader.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2187 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/src/hdx/utilities/easy_logging.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8054 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/src/hdx/utilities/email.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2203 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/src/hdx/utilities/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/src/hdx/utilities/errors_onexit.py
--rw-r--r--   0 runner    (1001) docker     (123)     8728 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/src/hdx/utilities/frictionless_wrapper.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2967 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/src/hdx/utilities/html.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4117 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/src/hdx/utilities/loader.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17574 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/src/hdx/utilities/path.py
--rw-r--r--   0 runner    (1001) docker     (123)    18738 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/src/hdx/utilities/retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)     9132 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/src/hdx/utilities/saver.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7647 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/src/hdx/utilities/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/src/hdx/utilities/state.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13872 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/src/hdx/utilities/text.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/src/hdx/utilities/typehint.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6838 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/src/hdx/utilities/useragent.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/src/hdx/utilities/uuid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:19:41.768089 hdx-python-utilities-3.5.8/src/hdx_python_utilities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-04-11 03:19:41.000000 hdx-python-utilities-3.5.8/src/hdx_python_utilities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-04-11 03:19:41.000000 hdx-python-utilities-3.5.8/src/hdx_python_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 03:19:41.000000 hdx-python-utilities-3.5.8/src/hdx_python_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-11 03:19:41.000000 hdx-python-utilities-3.5.8/src/hdx_python_utilities.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-11 03:19:41.000000 hdx-python-utilities-3.5.8/src/hdx_python_utilities.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 03:19:40.000000 hdx-python-utilities-3.5.8/src/hdx_python_utilities.egg-info/zip-safe
--rwxr-xr-x   0 runner    (1001) docker     (123)      229 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:19:41.760089 hdx-python-utilities-3.5.8/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:19:41.768089 hdx-python-utilities-3.5.8/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:19:41.768089 hdx-python-utilities-3.5.8/tests/fixtures/compare/
--rwxr-xr-x   0 runner    (1001) docker     (123)      122 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/compare/test_csv_processing.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)      125 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/compare/test_csv_processing2.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:19:41.768089 hdx-python-utilities-3.5.8/tests/fixtures/config/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/config/empty.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      482 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/config/hdx_config.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      390 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/config/hdx_config.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      172 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/config/hdx_email_configuration.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      135 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/config/hdx_email_configuration.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/config/json_csv.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      882 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/config/logging_config.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      805 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/config/logging_config.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)       23 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/config/project_configuration.json
--rwxr-xr-x   0 runner    (1001) docker     (123)       50 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/config/project_configuration.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      123 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/config/smtp_config.json
--rwxr-xr-x   0 runner    (1001) docker     (123)       97 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/config/smtp_config.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)       32 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/config/user_agent_config.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)       23 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/config/user_agent_config2.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)       73 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/config/user_agent_config3.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)       17 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/config/user_agent_config_wrong.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:19:41.772090 hdx-python-utilities-3.5.8/tests/fixtures/downloader/
--rwxr-xr-x   0 runner    (1001) docker     (123)       30 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/downloader/basicauth.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       67 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/downloader/extra_params.json
--rwxr-xr-x   0 runner    (1001) docker     (123)       46 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/downloader/extra_params.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      106 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/downloader/extra_params_tree.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)       83 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/downloader/test_csv_processing.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)       83 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/downloader/test_csv_processing_blanks.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/downloader/test_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6279 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/downloader/test_data.xlsx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:19:41.772090 hdx-python-utilities-3.5.8/tests/fixtures/downloader/test_data1.csv/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/downloader/test_data1.csv/empty.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/downloader/test_data2.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)      178 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/downloader/test_json_processing.json
--rwxr-xr-x   0 runner    (1001) docker     (123)  1626112 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/downloader/test_xls_processing.xls
--rwxr-xr-x   0 runner    (1001) docker     (123)   164046 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/downloader/test_xlsx_processing.xlsx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:19:41.772090 hdx-python-utilities-3.5.8/tests/fixtures/html/
--rwxr-xr-x   0 runner    (1001) docker     (123)  1622046 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/html/response.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:19:41.776090 hdx-python-utilities-3.5.8/tests/fixtures/loader/
--rwxr-xr-x   0 runner    (1001) docker     (123)        2 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/loader/empty.json
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/loader/empty.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:19:41.776090 hdx-python-utilities-3.5.8/tests/fixtures/retriever/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:19:41.776090 hdx-python-utilities-3.5.8/tests/fixtures/retriever/fallbacks/
--rwxr-xr-x   0 runner    (1001) docker     (123)       72 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/retriever/fallbacks/test.csv
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/retriever/fallbacks/test.json
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/retriever/fallbacks/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/retriever/fallbacks/test.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)       68 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/retriever/retriever-test.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)       68 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/retriever/test.csv
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/retriever/test.json
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/retriever/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/retriever/test.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)       84 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/retriever/test_hxl.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:19:41.776090 hdx-python-utilities-3.5.8/tests/fixtures/saver/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/saver/out.csv
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/saver/out.json
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/saver/out2.csv
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/saver/out2.json
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/saver/out5.json
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/saver/out6.json
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/saver/out7.json
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/saver/out8.csv
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/saver/out8.json
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/saver/pretty-false_sortkeys-false.json
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/saver/pretty-false_sortkeys-false.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/saver/pretty-false_sortkeys-true.json
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/saver/pretty-false_sortkeys-true.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/saver/pretty-true_sortkeys-false.json
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/saver/pretty-true_sortkeys-false.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/saver/pretty-true_sortkeys-true.json
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/saver/pretty-true_sortkeys-true.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:19:41.776090 hdx-python-utilities-3.5.8/tests/fixtures/state/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/state/last_build_date.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1550 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/fixtures/test_data.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:19:41.780090 hdx-python-utilities-3.5.8/tests/hdx/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1778 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/hdx/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:19:41.780090 hdx-python-utilities-3.5.8/tests/hdx/utilities/
--rwxr-xr-x   0 runner    (1001) docker     (123)      834 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/hdx/utilities/test_compare.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9698 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/hdx/utilities/test_dateparse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13565 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/hdx/utilities/test_dictandlist.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    47752 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/hdx/utilities/test_downloader.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      959 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/hdx/utilities/test_easy_logging.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5656 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/hdx/utilities/test_email.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      617 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/hdx/utilities/test_encoding.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      735 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/hdx/utilities/test_errors_onexit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2411 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/hdx/utilities/test_html.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5363 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/hdx/utilities/test_loader.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15246 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/hdx/utilities/test_path.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20894 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/hdx/utilities/test_retriever.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10273 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/hdx/utilities/test_saver.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1408 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/hdx/utilities/test_state.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14379 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/hdx/utilities/test_text.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3536 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/hdx/utilities/test_useragent.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      416 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/hdx/utilities/test_uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-11 03:19:21.000000 hdx-python-utilities-3.5.8/tests/hdx/utilities/utils.py
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/CONTRIBUTING.md
+-rwxr-xr-x   0        0        0     3966 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/requirements.txt
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/.config/black.toml
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/.config/coveragerc
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/.config/pre-commit-config.yaml
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/.config/pytest.ini
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/.config/ruff.toml
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/.github/workflows/run-python-tests.yml
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/documentation/.readthedocs.yaml
+-rw-r--r--   0        0        0    35300 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/documentation/main.md
+-rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/documentation/pydoc-markdown.yml
+-rwxr-xr-x   0        0        0       59 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/src/hdx/utilities/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/src/hdx/utilities/_version.py
+-rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/src/hdx/utilities/base_downloader.py
+-rwxr-xr-x   0        0        0      966 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/src/hdx/utilities/compare.py
+-rwxr-xr-x   0        0        0    35023 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/src/hdx/utilities/dateparse.py
+-rwxr-xr-x   0        0        0    15753 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/src/hdx/utilities/dictandlist.py
+-rwxr-xr-x   0        0        0    61800 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/src/hdx/utilities/downloader.py
+-rwxr-xr-x   0        0        0     2187 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/src/hdx/utilities/easy_logging.py
+-rwxr-xr-x   0        0        0     8054 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/src/hdx/utilities/email.py
+-rwxr-xr-x   0        0        0     2203 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/src/hdx/utilities/encoding.py
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/src/hdx/utilities/errors_onexit.py
+-rw-r--r--   0        0        0     8728 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/src/hdx/utilities/frictionless_wrapper.py
+-rwxr-xr-x   0        0        0     2967 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/src/hdx/utilities/html.py
+-rwxr-xr-x   0        0        0     4117 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/src/hdx/utilities/loader.py
+-rwxr-xr-x   0        0        0    17574 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/src/hdx/utilities/path.py
+-rw-r--r--   0        0        0    18738 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/src/hdx/utilities/retriever.py
+-rw-r--r--   0        0        0     9132 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/src/hdx/utilities/saver.py
+-rwxr-xr-x   0        0        0     7647 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/src/hdx/utilities/session.py
+-rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/src/hdx/utilities/state.py
+-rwxr-xr-x   0        0        0    13872 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/src/hdx/utilities/text.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/src/hdx/utilities/typehint.py
+-rwxr-xr-x   0        0        0     6838 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/src/hdx/utilities/useragent.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/src/hdx/utilities/uuid.py
+-rwxr-xr-x   0        0        0     1550 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/test_data.csv
+-rwxr-xr-x   0        0        0      122 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/compare/test_csv_processing.csv
+-rwxr-xr-x   0        0        0      125 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/compare/test_csv_processing2.csv
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/config/empty.yml
+-rwxr-xr-x   0        0        0      482 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/config/hdx_config.json
+-rwxr-xr-x   0        0        0      390 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/config/hdx_config.yml
+-rwxr-xr-x   0        0        0      172 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/config/hdx_email_configuration.json
+-rwxr-xr-x   0        0        0      135 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/config/hdx_email_configuration.yml
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/config/json_csv.yml
+-rwxr-xr-x   0        0        0      882 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/config/logging_config.json
+-rwxr-xr-x   0        0        0      805 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/config/logging_config.yml
+-rwxr-xr-x   0        0        0       23 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/config/project_configuration.json
+-rwxr-xr-x   0        0        0       50 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/config/project_configuration.yml
+-rwxr-xr-x   0        0        0      123 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/config/smtp_config.json
+-rwxr-xr-x   0        0        0       97 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/config/smtp_config.yml
+-rwxr-xr-x   0        0        0       32 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/config/user_agent_config.yml
+-rwxr-xr-x   0        0        0       23 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/config/user_agent_config2.yml
+-rwxr-xr-x   0        0        0       73 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/config/user_agent_config3.yml
+-rwxr-xr-x   0        0        0       17 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/config/user_agent_config_wrong.yml
+-rwxr-xr-x   0        0        0       30 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/downloader/basicauth.txt
+-rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/downloader/extra_params.json
+-rwxr-xr-x   0        0        0       46 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/downloader/extra_params.yml
+-rwxr-xr-x   0        0        0      106 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/downloader/extra_params_tree.yml
+-rwxr-xr-x   0        0        0       83 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/downloader/test_csv_processing.csv
+-rwxr-xr-x   0        0        0       83 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/downloader/test_csv_processing_blanks.csv
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/downloader/test_data.csv
+-rw-r--r--   0        0        0     6279 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/downloader/test_data.xlsx
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/downloader/test_data2.csv
+-rwxr-xr-x   0        0        0      178 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/downloader/test_json_processing.json
+-rwxr-xr-x   0        0        0  1626112 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/downloader/test_xls_processing.xls
+-rwxr-xr-x   0        0        0   164046 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/downloader/test_xlsx_processing.xlsx
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/downloader/test_data1.csv/empty.txt
+-rwxr-xr-x   0        0        0  1622046 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/html/response.html
+-rwxr-xr-x   0        0        0        2 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/loader/empty.json
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/loader/empty.yml
+-rwxr-xr-x   0        0        0       68 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/retriever/retriever-test.csv
+-rwxr-xr-x   0        0        0       68 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/retriever/test.csv
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/retriever/test.json
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/retriever/test.txt
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/retriever/test.yaml
+-rwxr-xr-x   0        0        0       84 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/retriever/test_hxl.csv
+-rwxr-xr-x   0        0        0       72 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/retriever/fallbacks/test.csv
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/retriever/fallbacks/test.json
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/retriever/fallbacks/test.txt
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/retriever/fallbacks/test.yaml
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/saver/out.csv
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/saver/out.json
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/saver/out2.csv
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/saver/out2.json
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/saver/out5.json
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/saver/out6.json
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/saver/out7.json
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/saver/out8.csv
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/saver/out8.json
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/saver/pretty-false_sortkeys-false.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/saver/pretty-false_sortkeys-false.yaml
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/saver/pretty-false_sortkeys-true.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/saver/pretty-false_sortkeys-true.yaml
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/saver/pretty-true_sortkeys-false.json
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/saver/pretty-true_sortkeys-false.yaml
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/saver/pretty-true_sortkeys-true.json
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/saver/pretty-true_sortkeys-true.yaml
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/fixtures/state/last_build_date.txt
+-rwxr-xr-x   0        0        0     1778 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/hdx/conftest.py
+-rwxr-xr-x   0        0        0      834 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/hdx/utilities/test_compare.py
+-rwxr-xr-x   0        0        0     9698 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/hdx/utilities/test_dateparse.py
+-rwxr-xr-x   0        0        0    13565 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/hdx/utilities/test_dictandlist.py
+-rwxr-xr-x   0        0        0    47752 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/hdx/utilities/test_downloader.py
+-rwxr-xr-x   0        0        0      959 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/hdx/utilities/test_easy_logging.py
+-rwxr-xr-x   0        0        0     5656 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/hdx/utilities/test_email.py
+-rwxr-xr-x   0        0        0      617 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/hdx/utilities/test_encoding.py
+-rwxr-xr-x   0        0        0      735 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/hdx/utilities/test_errors_onexit.py
+-rwxr-xr-x   0        0        0     2411 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/hdx/utilities/test_html.py
+-rwxr-xr-x   0        0        0     5363 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/hdx/utilities/test_loader.py
+-rwxr-xr-x   0        0        0    15246 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/hdx/utilities/test_path.py
+-rwxr-xr-x   0        0        0    20894 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/hdx/utilities/test_retriever.py
+-rwxr-xr-x   0        0        0    10273 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/hdx/utilities/test_saver.py
+-rwxr-xr-x   0        0        0     1408 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/hdx/utilities/test_state.py
+-rwxr-xr-x   0        0        0    14379 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/hdx/utilities/test_text.py
+-rwxr-xr-x   0        0        0     3536 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/hdx/utilities/test_useragent.py
+-rwxr-xr-x   0        0        0      416 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/hdx/utilities/test_uuid.py
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/tests/hdx/utilities/utils.py
+-rwxr-xr-x   0        0        0     1148 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/.gitignore
+-rwxr-xr-x   0        0        0     1079 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/LICENSE
+-rwxr-xr-x   0        0        0     1725 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/README.md
+-rw-r--r--   0        0        0     3231 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/pyproject.toml
+-rw-r--r--   0        0        0     3805 2020-02-02 00:00:00.000000 hdx_python_utilities-3.5.9/PKG-INFO
```

### Comparing `hdx-python-utilities-3.5.8/.github/workflows/publish.yml` & `hdx_python_utilities-3.5.9/.github/workflows/publish.yml`

 * *Files 19% similar despite different names*

```diff
@@ -6,25 +6,28 @@
 
 jobs:
   publish:
     runs-on: ubuntu-latest
 
     steps:
     - uses: actions/checkout@v3
-    - name: Get history and tags for SCM versioning to work
+    - name: Get history and tags for versioning to work
       run: |
         git fetch --prune --unshallow
         git fetch --depth=1 origin +refs/tags/*:refs/tags/*
     - name: Set up Python
       uses: actions/setup-python@v4
       with:
         python-version: '3.x'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        pip install --upgrade tox-gh-actions
-    - name: Publish with tox and twine
+        pip install --upgrade hatch
+    - name: Build with hatch
+      run: |
+        hatch build
+    - name: Publish with hatch
       env:
-        TWINE_USERNAME: ${{ secrets.TWINE_USERNAME }}
-        TWINE_PASSWORD: ${{ secrets.TWINE_PASSWORD }}
+        HATCH_INDEX_USER: ${{secrets.HATCH_INDEX_USER}}
+        HATCH_INDEX_AUTH: ${{secrets.HATCH_INDEX_AUTH}}
       run: |
-        tox -e publish
+        hatch publish
```

### Comparing `hdx-python-utilities-3.5.8/.github/workflows/run-python-tests.yml` & `hdx_python_utilities-3.5.9/.github/workflows/run-python-tests.yml`

 * *Files 18% similar despite different names*

```diff
@@ -20,20 +20,27 @@
     - name: Set up Python
       uses: actions/setup-python@v4
       with:
         python-version: '3.x'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        pip install --upgrade tox-gh-actions
-    - name: Test with tox/pytest
+        pip install --upgrade hatch
+    - name: Test with hatch/pytest
       run: |
-        tox
+        hatch run test:test
+    - name: Check styling
+      if: always()
+      run: |
+        hatch run lint:style
     - name: Publish Unit Test Results
       uses: EnricoMi/publish-unit-test-result-action@v2
       if: always()
       with:
         github_token: ${{ secrets.GITHUB_TOKEN }}
-        junit_files: .tox/*.xml
-    - name: Upload Coverage Results
-      uses: codecov/codecov-action@v3
-      if: success()
+        junit_files: test-results.xml
+    - name: Publish in Coveralls
+      uses: coverallsapp/github-action@v2
+      with:
+        github-token: ${{ secrets.GITHUB_TOKEN }}
+        flag-name: tests
+        format: lcov
```

### Comparing `hdx-python-utilities-3.5.8/.gitignore` & `hdx_python_utilities-3.5.9/.gitignore`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.8/LICENSE` & `hdx_python_utilities-3.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.8/README.md` & `hdx_python_utilities-3.5.9/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [![Build Status](https://github.com/OCHA-DAP/hdx-python-utilities/actions/workflows/run-python-tests.yml/badge.svg)](https://github.com/OCHA-DAP/hdx-python-utilities/actions/workflows/run-python-tests.yml)
-[![Coverage Status](https://codecov.io/gh/OCHA-DAP/hdx-python-utilities/branch/main/graph/badge.svg?token=JpWZc5js4y)](https://codecov.io/gh/OCHA-DAP/hdx-python-utilities)
+[![Coverage Status](https://coveralls.io/repos/github/OCHA-DAP/hdx-python-utilities/badge.svg?branch=main&ts=1)](https://coveralls.io/github/OCHA-DAP/hdx-python-utilities?branch=main)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![Downloads](https://img.shields.io/pypi/dm/hdx-python-utilities.svg)](https://pypistats.org/packages/hdx-python-utilities)
 
 The HDX Python Utilities Library provides a range of helpful utilities for Python developers.
 Note that these are not specific to HDX.
```

### Comparing `hdx-python-utilities-3.5.8/doc/main.md` & `hdx_python_utilities-3.5.9/documentation/main.md`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.8/src/hdx/utilities/base_downloader.py` & `hdx_python_utilities-3.5.9/src/hdx/utilities/base_downloader.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.8/src/hdx/utilities/compare.py` & `hdx_python_utilities-3.5.9/src/hdx/utilities/compare.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.8/src/hdx/utilities/dateparse.py` & `hdx_python_utilities-3.5.9/src/hdx/utilities/dateparse.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.8/src/hdx/utilities/dictandlist.py` & `hdx_python_utilities-3.5.9/src/hdx/utilities/dictandlist.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.8/src/hdx/utilities/downloader.py` & `hdx_python_utilities-3.5.9/src/hdx/utilities/downloader.py`

 * *Files 0% similar despite different names*

```diff
@@ -270,15 +270,15 @@
         self.response = None
         try:
             spliturl = urlsplit(url)
             if not spliturl.scheme:
                 if isfile(url):
                     url = Path(url).resolve().as_uri()
                 else:
-                    spliturl = spliturl._replace(scheme="http")
+                    spliturl = spliturl._replace(scheme="https")
                     url = urlunsplit(spliturl)
             if post:
                 full_url, parameters = self.get_url_params_for_post(
                     url, parameters
                 )
                 self.response = self.session.post(
                     full_url,
```

### Comparing `hdx-python-utilities-3.5.8/src/hdx/utilities/easy_logging.py` & `hdx_python_utilities-3.5.9/src/hdx/utilities/easy_logging.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.8/src/hdx/utilities/email.py` & `hdx_python_utilities-3.5.9/src/hdx/utilities/email.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.8/src/hdx/utilities/encoding.py` & `hdx_python_utilities-3.5.9/src/hdx/utilities/encoding.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.8/src/hdx/utilities/errors_onexit.py` & `hdx_python_utilities-3.5.9/src/hdx/utilities/errors_onexit.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.8/src/hdx/utilities/frictionless_wrapper.py` & `hdx_python_utilities-3.5.9/src/hdx/utilities/frictionless_wrapper.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.8/src/hdx/utilities/html.py` & `hdx_python_utilities-3.5.9/src/hdx/utilities/html.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.8/src/hdx/utilities/loader.py` & `hdx_python_utilities-3.5.9/src/hdx/utilities/loader.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.8/src/hdx/utilities/path.py` & `hdx_python_utilities-3.5.9/src/hdx/utilities/path.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.8/src/hdx/utilities/retriever.py` & `hdx_python_utilities-3.5.9/src/hdx/utilities/retriever.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.8/src/hdx/utilities/saver.py` & `hdx_python_utilities-3.5.9/src/hdx/utilities/saver.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.8/src/hdx/utilities/session.py` & `hdx_python_utilities-3.5.9/src/hdx/utilities/session.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.8/src/hdx/utilities/state.py` & `hdx_python_utilities-3.5.9/src/hdx/utilities/state.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.8/src/hdx/utilities/text.py` & `hdx_python_utilities-3.5.9/src/hdx/utilities/text.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.8/src/hdx/utilities/useragent.py` & `hdx_python_utilities-3.5.9/src/hdx/utilities/useragent.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.8/src/hdx/utilities/uuid.py` & `hdx_python_utilities-3.5.9/src/hdx/utilities/uuid.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.8/tests/fixtures/config/json_csv.yml` & `hdx_python_utilities-3.5.9/tests/fixtures/config/json_csv.yml`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.8/tests/fixtures/config/logging_config.json` & `hdx_python_utilities-3.5.9/tests/fixtures/config/logging_config.json`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.8/tests/fixtures/config/logging_config.yml` & `hdx_python_utilities-3.5.9/tests/fixtures/config/logging_config.yml`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.8/tests/fixtures/downloader/test_data.xlsx` & `hdx_python_utilities-3.5.9/tests/fixtures/downloader/test_data.xlsx`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.8/tests/fixtures/downloader/test_xls_processing.xls` & `hdx_python_utilities-3.5.9/tests/fixtures/downloader/test_xls_processing.xls`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.8/tests/fixtures/downloader/test_xlsx_processing.xlsx` & `hdx_python_utilities-3.5.9/tests/fixtures/downloader/test_xlsx_processing.xlsx`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.8/tests/fixtures/html/response.html` & `hdx_python_utilities-3.5.9/tests/fixtures/html/response.html`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.8/tests/fixtures/test_data.csv` & `hdx_python_utilities-3.5.9/tests/fixtures/test_data.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.8/tests/hdx/conftest.py` & `hdx_python_utilities-3.5.9/tests/hdx/conftest.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.8/tests/hdx/utilities/test_compare.py` & `hdx_python_utilities-3.5.9/tests/hdx/utilities/test_compare.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.8/tests/hdx/utilities/test_dateparse.py` & `hdx_python_utilities-3.5.9/tests/hdx/utilities/test_dateparse.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.8/tests/hdx/utilities/test_dictandlist.py` & `hdx_python_utilities-3.5.9/tests/hdx/utilities/test_dictandlist.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.8/tests/hdx/utilities/test_downloader.py` & `hdx_python_utilities-3.5.9/tests/hdx/utilities/test_downloader.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.8/tests/hdx/utilities/test_easy_logging.py` & `hdx_python_utilities-3.5.9/tests/hdx/utilities/test_easy_logging.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.8/tests/hdx/utilities/test_email.py` & `hdx_python_utilities-3.5.9/tests/hdx/utilities/test_email.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.8/tests/hdx/utilities/test_encoding.py` & `hdx_python_utilities-3.5.9/tests/hdx/utilities/test_encoding.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.8/tests/hdx/utilities/test_errors_onexit.py` & `hdx_python_utilities-3.5.9/tests/hdx/utilities/test_errors_onexit.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.8/tests/hdx/utilities/test_html.py` & `hdx_python_utilities-3.5.9/tests/hdx/utilities/test_html.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.8/tests/hdx/utilities/test_loader.py` & `hdx_python_utilities-3.5.9/tests/hdx/utilities/test_loader.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.8/tests/hdx/utilities/test_path.py` & `hdx_python_utilities-3.5.9/tests/hdx/utilities/test_path.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.8/tests/hdx/utilities/test_retriever.py` & `hdx_python_utilities-3.5.9/tests/hdx/utilities/test_retriever.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.8/tests/hdx/utilities/test_saver.py` & `hdx_python_utilities-3.5.9/tests/hdx/utilities/test_saver.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.8/tests/hdx/utilities/test_state.py` & `hdx_python_utilities-3.5.9/tests/hdx/utilities/test_state.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.8/tests/hdx/utilities/test_text.py` & `hdx_python_utilities-3.5.9/tests/hdx/utilities/test_text.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.8/tests/hdx/utilities/test_useragent.py` & `hdx_python_utilities-3.5.9/tests/hdx/utilities/test_useragent.py`

 * *Files identical despite different names*

### Comparing `hdx-python-utilities-3.5.8/tests/hdx/utilities/utils.py` & `hdx_python_utilities-3.5.9/tests/hdx/utilities/utils.py`

 * *Files identical despite different names*

