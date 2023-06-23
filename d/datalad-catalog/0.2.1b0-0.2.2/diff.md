# Comparing `tmp/datalad_catalog-0.2.1b0.tar.gz` & `tmp/datalad_catalog-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datalad_catalog-0.2.1b0.tar", last modified: Wed May 24 19:15:30 2023, max compression
+gzip compressed data, was "datalad_catalog-0.2.2.tar", last modified: Fri Jun 23 10:02:23 2023, max compression
```

## Comparing `datalad_catalog-0.2.1b0.tar` & `datalad_catalog-0.2.2.tar`

### file list

```diff
@@ -1,184 +1,168 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:15:30.341699 datalad_catalog-0.2.1b0/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/CONTRIBUTORS
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    19942 2023-05-24 19:15:30.341699 datalad_catalog-0.2.1b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19466 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:15:30.293699 datalad_catalog-0.2.1b0/_datalad_buildsupport/
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/_datalad_buildsupport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10699 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/_datalad_buildsupport/formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)     9752 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/_datalad_buildsupport/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:15:30.345699 datalad_catalog-0.2.1b0/datalad_catalog/
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-24 19:15:30.345699 datalad_catalog-0.2.1b0/datalad_catalog/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:15:30.297699 datalad_catalog-0.2.1b0/datalad_catalog/catalog/
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/catalog/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:15:30.301699 datalad_catalog-0.2.1b0/datalad_catalog/catalog/artwork/
--rw-r--r--   0 runner    (1001) docker     (123)    15465 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/catalog/artwork/404.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/catalog/artwork/catalog_logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/catalog/artwork/datalad_catalog_logo_1_dark.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/catalog/artwork/datalad_catalog_logo_1_light.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/catalog/artwork/datalad_logo_wide.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11021 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/catalog/artwork/ginfavicon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:15:30.305699 datalad_catalog-0.2.1b0/datalad_catalog/catalog/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/catalog/assets/app.js
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/catalog/assets/app_component_about.js
--rw-r--r--   0 runner    (1001) docker     (123)    29878 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/catalog/assets/app_component_dataset.js
--rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/catalog/assets/app_component_item.js
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/catalog/assets/app_component_notfound.js
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/catalog/assets/app_globals.js
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/catalog/assets/app_router.js
--rw-r--r--   0 runner    (1001) docker     (123)    76102 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/catalog/assets/bootstrap-vue.2.21.2.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   360511 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/catalog/assets/bootstrap-vue.2.21.2.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   163873 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/catalog/assets/bootstrap.5.1.3.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    17473 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/catalog/assets/brands.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    19671 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/catalog/assets/display_schema.js
--rw-r--r--   0 runner    (1001) docker     (123)   105536 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/catalog/assets/fa-brands-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    23940 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/catalog/assets/fa-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   154228 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/catalog/assets/fa-solid-900.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:15:30.305699 datalad_catalog-0.2.1b0/datalad_catalog/catalog/assets/favicon/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/catalog/assets/favicon/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/catalog/assets/favicon/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/catalog/assets/favicon/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    80388 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/catalog/assets/fontawesome.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/catalog/assets/jsonschema_authors.json
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/catalog/assets/jsonschema_catalog.json
--rw-r--r--   0 runner    (1001) docker     (123)     9169 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/catalog/assets/jsonschema_dataset.json
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/catalog/assets/jsonschema_file.json
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/catalog/assets/jsonschema_metadata_sources.json
--rw-r--r--   0 runner    (1001) docker     (123)    47938 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/catalog/assets/marked.4.0.17.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/catalog/assets/md5-2.3.0.js
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/catalog/assets/meta_entry.js
--rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/catalog/assets/style.css
--rw-r--r--   0 runner    (1001) docker     (123)    29206 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/catalog/assets/vue-router.3.5.3.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    94151 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/catalog/assets/vue.2.6.14.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/catalog/config.json
--rw-r--r--   0 runner    (1001) docker     (123)    16275 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/catalog/display_schema.html
--rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/catalog/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:15:30.305699 datalad_catalog-0.2.1b0/datalad_catalog/catalog/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/catalog/metadata/super.json
--rw-r--r--   0 runner    (1001) docker     (123)     6096 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/catalog/metadata-entry.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:15:30.309699 datalad_catalog-0.2.1b0/datalad_catalog/catalog/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    37243 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/catalog/templates/dataset-template.html
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/catalog/templates/item-template.html
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/catalog/templates/main-template.html
--rw-r--r--   0 runner    (1001) docker     (123)    31022 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:15:30.309699 datalad_catalog-0.2.1b0/datalad_catalog/config/
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/config/config.json
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/config/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:15:30.309699 datalad_catalog-0.2.1b0/datalad_catalog/extractors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/extractors/datacite_gin.py
--rw-r--r--   0 runner    (1001) docker     (123)     9863 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/meta_item.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:15:30.309699 datalad_catalog-0.2.1b0/datalad_catalog/schema/
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/schema/jsonschema_authors.json
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/schema/jsonschema_catalog.json
--rw-r--r--   0 runner    (1001) docker     (123)     9169 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/schema/jsonschema_dataset.json
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/schema/jsonschema_file.json
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/schema/jsonschema_metadata_sources.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:15:30.313699 datalad_catalog-0.2.1b0/datalad_catalog/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:15:30.317699 datalad_catalog-0.2.1b0/datalad_catalog/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/tests/data/catalog_metadata_dataset.json
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/tests/data/catalog_metadata_dataset.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/tests/data/catalog_metadata_dataset2.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)     6728 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/tests/data/catalog_metadata_dataset_updated.json
--rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/tests/data/catalog_metadata_dataset_updated_min.json
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/tests/data/catalog_metadata_invalid.json
--rw-r--r--   0 runner    (1001) docker     (123)     9896 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/tests/data/catalog_metadata_valid.json
--rw-r--r--   0 runner    (1001) docker     (123)     8877 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/tests/data/metadata_bids_dataset.json
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/tests/data/metadata_bids_dataset.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)     9438 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/tests/data/metadata_bids_dataset2.json
--rw-r--r--   0 runner    (1001) docker     (123)     7934 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/tests/data/metadata_bids_dataset2.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)     8711 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/tests/data/metadata_core.json
--rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/tests/data/metadata_core.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/tests/data/metadata_core_dataset.json
--rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/tests/data/metadata_datacite_gin.json
--rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/tests/data/metadata_datacite_gin.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)     8677 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/tests/data/metadata_datacite_gin2.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)    13503 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/tests/data/metadata_studyminimeta.json
--rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/tests/data/metadata_studyminimeta.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/tests/data/metadata_translate_nonsense.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/tests/data/metadata_translate_wrongname.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/tests/data/metadata_translate_wrongversion.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/tests/data/test_config_file.json
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/tests/data/test_config_file.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/tests/data/test_config_file_catalog.json
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/tests/data/test_config_file_dataset.json
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/tests/data/test_config_file_workflow.json
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/tests/data/workflow_generated_meta_dir.json
--rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/tests/data/workflow_generated_meta_sub.json
--rw-r--r--   0 runner    (1001) docker     (123)     7460 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/tests/data/workflow_generated_meta_super.json
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/tests/register.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/tests/test_action_add.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/tests/test_action_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/tests/test_action_setsuper.py
--rw-r--r--   0 runner    (1001) docker     (123)    13839 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/tests/test_add_update_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/tests/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/tests/test_catalog_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/tests/test_meta_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/tests/test_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/tests/test_translate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/tests/test_webcatalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    19429 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/tests/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     5192 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:15:30.317699 datalad_catalog-0.2.1b0/datalad_catalog/translators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/translators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7557 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/translators/bids_dataset_translator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/translators/datacite_gin_translator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/translators/metalad_core_translator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7677 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/translators/metalad_studyminimeta_translator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    29225 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/webcatalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     9983 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/datalad_catalog/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:15:30.297699 datalad_catalog-0.2.1b0/datalad_catalog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19942 2023-05-24 19:15:30.000000 datalad_catalog-0.2.1b0/datalad_catalog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7100 2023-05-24 19:15:30.000000 datalad_catalog-0.2.1b0/datalad_catalog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 19:15:30.000000 datalad_catalog-0.2.1b0/datalad_catalog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-24 19:15:30.000000 datalad_catalog-0.2.1b0/datalad_catalog.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-24 19:15:30.000000 datalad_catalog-0.2.1b0/datalad_catalog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-24 19:15:30.000000 datalad_catalog-0.2.1b0/datalad_catalog.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:15:30.317699 datalad_catalog-0.2.1b0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:15:30.321699 datalad_catalog-0.2.1b0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:15:30.341699 datalad_catalog-0.2.1b0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)   548128 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/docs/source/_static/catalog_screenshot.png
--rw-r--r--   0 runner    (1001) docker     (123)   457781 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/docs/source/_static/datacat0_hero.svg
--rw-r--r--   0 runner    (1001) docker     (123)   457833 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/docs/source/_static/datacat0_hero_lightbg.svg
--rw-r--r--   0 runner    (1001) docker     (123)  1197513 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/docs/source/_static/datacat1_the_challenge.svg
--rw-r--r--   0 runner    (1001) docker     (123)   793508 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/docs/source/_static/datacat2_the_opportunity.svg
--rw-r--r--   0 runner    (1001) docker     (123)  1692043 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/docs/source/_static/datacat3_the_toolset.svg
--rw-r--r--   0 runner    (1001) docker     (123)  1692147 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/docs/source/_static/datacat3_the_toolset_lightbg.svg
--rw-r--r--   0 runner    (1001) docker     (123)  1736126 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/docs/source/_static/datacat4_the_catalog.svg
--rw-r--r--   0 runner    (1001) docker     (123)  1736178 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/docs/source/_static/datacat4_the_catalog_lightbg.svg
--rw-r--r--   0 runner    (1001) docker     (123)   370286 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/docs/source/_static/datacat_logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)   638140 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/docs/source/_static/datalad_catalog_demo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    61542 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/docs/source/_static/datalad_catalog_functionality.svg
--rw-r--r--   0 runner    (1001) docker     (123)  2103419 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/docs/source/_static/datalad_catalog_logo_1_dark.svg
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/docs/source/_static/datalad_logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:15:30.293699 datalad_catalog-0.2.1b0/docs/source/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:15:30.341699 datalad_catalog-0.2.1b0/docs/source/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/docs/source/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/docs/source/catalog_config.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/docs/source/catalog_schema.rst
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/docs/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/docs/source/command_line_reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/docs/source/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/docs/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/docs/source/metadata_formats.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/docs/source/overview.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9760 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/docs/source/pipeline_description.rst
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/docs/source/python_module_reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/docs/source/resources.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/docs/source/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-24 19:15:30.345699 datalad_catalog-0.2.1b0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      372 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-05-24 19:15:15.000000 datalad_catalog-0.2.1b0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:02:23.256195 datalad_catalog-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/CONTRIBUTORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    19844 2023-06-23 10:02:23.256195 datalad_catalog-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19370 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:02:23.220192 datalad_catalog-0.2.2/_datalad_buildsupport/
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/_datalad_buildsupport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/_datalad_buildsupport/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9752 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/_datalad_buildsupport/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:02:23.256195 datalad_catalog-0.2.2/datalad_catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-23 10:02:23.256195 datalad_catalog-0.2.2/datalad_catalog/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:02:23.224192 datalad_catalog-0.2.2/datalad_catalog/catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/catalog/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:02:23.224192 datalad_catalog-0.2.2/datalad_catalog/catalog/artwork/
+-rw-r--r--   0 runner    (1001) docker     (123)    15465 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/catalog/artwork/404.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/catalog/artwork/catalog_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/catalog/artwork/datalad_catalog_logo_1_dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/catalog/artwork/datalad_catalog_logo_1_light.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/catalog/artwork/datalad_logo_wide.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11021 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/catalog/artwork/ginfavicon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:02:23.228193 datalad_catalog-0.2.2/datalad_catalog/catalog/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/catalog/assets/app.js
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/catalog/assets/app_component_about.js
+-rw-r--r--   0 runner    (1001) docker     (123)    22971 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/catalog/assets/app_component_dataset.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/catalog/assets/app_component_item.js
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/catalog/assets/app_component_notfound.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/catalog/assets/app_globals.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/catalog/assets/app_router.js
+-rw-r--r--   0 runner    (1001) docker     (123)    76102 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/catalog/assets/bootstrap-vue.2.21.2.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   360511 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/catalog/assets/bootstrap-vue.2.21.2.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   163873 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/catalog/assets/bootstrap.5.1.3.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    17473 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/catalog/assets/brands.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    19663 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/catalog/assets/display_schema.js
+-rw-r--r--   0 runner    (1001) docker     (123)   105536 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/catalog/assets/fa-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    23940 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/catalog/assets/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   154228 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/catalog/assets/fa-solid-900.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:02:23.232193 datalad_catalog-0.2.2/datalad_catalog/catalog/assets/favicon/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/catalog/assets/favicon/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/catalog/assets/favicon/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/catalog/assets/favicon/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    80388 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/catalog/assets/fontawesome.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/catalog/assets/jsonschema_authors.json
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/catalog/assets/jsonschema_catalog.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7070 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/catalog/assets/jsonschema_dataset.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/catalog/assets/jsonschema_extractors.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/catalog/assets/jsonschema_file.json
+-rw-r--r--   0 runner    (1001) docker     (123)    47938 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/catalog/assets/marked.4.0.17.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/catalog/assets/md5-2.3.0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/catalog/assets/meta_entry.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/catalog/assets/style.css
+-rw-r--r--   0 runner    (1001) docker     (123)    29206 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/catalog/assets/vue-router.3.5.3.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    94151 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/catalog/assets/vue.2.6.14.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/catalog/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16275 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/catalog/display_schema.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/catalog/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:02:23.232193 datalad_catalog-0.2.2/datalad_catalog/catalog/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/catalog/metadata/super.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6096 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/catalog/metadata-entry.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:02:23.232193 datalad_catalog-0.2.2/datalad_catalog/catalog/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    35922 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/catalog/templates/dataset-template.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/catalog/templates/item-template.html
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/catalog/templates/main-template.html
+-rw-r--r--   0 runner    (1001) docker     (123)    28071 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:02:23.232193 datalad_catalog-0.2.2/datalad_catalog/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/config/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/config/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:02:23.232193 datalad_catalog-0.2.2/datalad_catalog/extractors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/extractors/datacite_gin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9805 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/meta_item.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:02:23.232193 datalad_catalog-0.2.2/datalad_catalog/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/schema/_bidsdataset2catalog.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/schema/_datacitegin2catalog.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/schema/_metaladcore2catalog_dataset.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/schema/_metaladcore2catalog_file.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/schema/_studyminimeta2catalog.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/schema/jsonschema_authors.json
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/schema/jsonschema_catalog.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7070 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/schema/jsonschema_dataset.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/schema/jsonschema_extractors.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/schema/jsonschema_file.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:02:23.236193 datalad_catalog-0.2.2/datalad_catalog/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:02:23.236193 datalad_catalog-0.2.2/datalad_catalog/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     5360 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/tests/data/catalog_metadata_dataset.json
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/tests/data/catalog_metadata_invalid.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9652 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/tests/data/catalog_metadata_valid.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8876 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/tests/data/metadata_bids_dataset.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/tests/data/metadata_bids_dataset.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)     9438 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/tests/data/metadata_bids_dataset2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7933 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/tests/data/metadata_bids_dataset2.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)     8711 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/tests/data/metadata_core.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/tests/data/metadata_core.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/tests/data/metadata_core_dataset.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5331 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/tests/data/metadata_datacite_gin.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/tests/data/metadata_datacite_gin.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)    13503 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/tests/data/metadata_studyminimeta.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/tests/data/metadata_studyminimeta.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/tests/data/test_config_file.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/tests/data/test_config_file.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/tests/data/workflow_generated_meta_dir.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/tests/data/workflow_generated_meta_sub.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/tests/data/workflow_generated_meta_super.json
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/tests/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/tests/test_action_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/tests/test_action_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/tests/test_action_setsuper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/tests/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/tests/test_catalog_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8928 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/tests/test_multisource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/tests/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/tests/test_translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/tests/test_webcatalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17952 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/tests/test_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19582 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/webcatalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9691 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/datalad_catalog/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:02:23.224192 datalad_catalog-0.2.2/datalad_catalog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19844 2023-06-23 10:02:23.000000 datalad_catalog-0.2.2/datalad_catalog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6276 2023-06-23 10:02:23.000000 datalad_catalog-0.2.2/datalad_catalog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 10:02:23.000000 datalad_catalog-0.2.2/datalad_catalog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-23 10:02:23.000000 datalad_catalog-0.2.2/datalad_catalog.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-23 10:02:23.000000 datalad_catalog-0.2.2/datalad_catalog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-23 10:02:23.000000 datalad_catalog-0.2.2/datalad_catalog.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:02:23.236193 datalad_catalog-0.2.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:02:23.240194 datalad_catalog-0.2.2/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:02:23.256195 datalad_catalog-0.2.2/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)   548128 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/docs/source/_static/catalog_screenshot.png
+-rw-r--r--   0 runner    (1001) docker     (123)   457781 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/docs/source/_static/datacat0_hero.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   457833 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/docs/source/_static/datacat0_hero_lightbg.svg
+-rw-r--r--   0 runner    (1001) docker     (123)  1197513 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/docs/source/_static/datacat1_the_challenge.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   793508 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/docs/source/_static/datacat2_the_opportunity.svg
+-rw-r--r--   0 runner    (1001) docker     (123)  1692043 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/docs/source/_static/datacat3_the_toolset.svg
+-rw-r--r--   0 runner    (1001) docker     (123)  1692147 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/docs/source/_static/datacat3_the_toolset_lightbg.svg
+-rw-r--r--   0 runner    (1001) docker     (123)  1736126 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/docs/source/_static/datacat4_the_catalog.svg
+-rw-r--r--   0 runner    (1001) docker     (123)  1736178 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/docs/source/_static/datacat4_the_catalog_lightbg.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   370286 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/docs/source/_static/datacat_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   638140 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/docs/source/_static/datalad_catalog_demo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    61542 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/docs/source/_static/datalad_catalog_functionality.svg
+-rw-r--r--   0 runner    (1001) docker     (123)  2103419 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/docs/source/_static/datalad_catalog_logo_1_dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/docs/source/_static/datalad_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:02:23.220192 datalad_catalog-0.2.2/docs/source/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:02:23.256195 datalad_catalog-0.2.2/docs/source/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/docs/source/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/docs/source/catalog_schema.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/docs/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/docs/source/command_line_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/docs/source/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/docs/source/metadata_formats.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/docs/source/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8408 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/docs/source/pipeline_description.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/docs/source/python_module_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/docs/source/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-06-23 10:02:23.256195 datalad_catalog-0.2.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1146 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-06-23 10:02:08.000000 datalad_catalog-0.2.2/versioneer.py
```

### Comparing `datalad_catalog-0.2.1b0/LICENSE` & `datalad_catalog-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.1b0/PKG-INFO` & `datalad_catalog-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datalad_catalog
-Version: 0.2.1b0
+Version: 0.2.2
 Summary: DataLad Catalog
 Home-page: https://github.com/datalad/datalad-catalog
 Author: DataLad Developers
 Author-email: team@datalad.org
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: BSD License
@@ -22,17 +22,15 @@
 [![GitHub release](https://img.shields.io/github/release/datalad/datalad-catalog.svg)](https://GitHub.com/datalad/datalad-catalog/releases/)
 [![PyPI version fury.io](https://badge.fury.io/py/datalad-catalog.svg)](https://pypi.python.org/pypi/datalad-catalog/)
 [![docs](https://github.com/datalad/datalad-catalog/actions/workflows/docbuild.yml/badge.svg)](https://github.com/datalad/datalad-catalog/actions/workflows/docbuild.yml)
 [![Build status](https://ci.appveyor.com/api/projects/status/github/datalad/datalad-catalog?branch=main&svg=true)](https://ci.appveyor.com/project/mih/datalad-catalog/branch/main)
 [![codecov.io](https://codecov.io/github/datalad/datalad-catalog/coverage.svg?branch=main)](https://codecov.io/github/datalad/datalad-catalog?branch=main)
 [![crippled-filesystems](https://github.com/datalad/datalad-catalog/actions/workflows/test_crippledfs.yml/badge.svg)](https://github.com/datalad/datalad-catalog/actions/workflows/test_crippledfs.yml)
 [![pages-build-deployment](https://github.com/datalad/datalad-catalog/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/datalad/datalad-catalog/actions/workflows/pages/pages-build-deployment)
-[![push_catalog_to_gh_pages](https://github.com/datalad/datalad-catalog/actions/workflows/deploy_demo.yml/badge.svg)](https://github.com/datalad/datalad-catalog/actions/workflows/deploy_demo.yml)
-[![DOI](https://zenodo.org/badge/371040885.svg)](https://zenodo.org/badge/latestdoi/371040885)
-<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
+[![push_catalog_to_gh_pages](https://github.com/datalad/datalad-catalog/actions/workflows/deploy_demo.yml/badge.svg)](https://github.com/datalad/datalad-catalog/actions/workflows/deploy_demo.yml)<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
 [![All Contributors](https://img.shields.io/badge/all_contributors-11-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 
 <picture>
   <source media="(prefers-color-scheme: light)" srcset="docs/source/_static/datacat0_hero.svg">
   <source media="(prefers-color-scheme: dark)" srcset="docs/source/_static/datacat0_hero_lightbg.svg">
```

### Comparing `datalad_catalog-0.2.1b0/README.md` & `datalad_catalog-0.2.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,17 +6,15 @@
 [![GitHub release](https://img.shields.io/github/release/datalad/datalad-catalog.svg)](https://GitHub.com/datalad/datalad-catalog/releases/)
 [![PyPI version fury.io](https://badge.fury.io/py/datalad-catalog.svg)](https://pypi.python.org/pypi/datalad-catalog/)
 [![docs](https://github.com/datalad/datalad-catalog/actions/workflows/docbuild.yml/badge.svg)](https://github.com/datalad/datalad-catalog/actions/workflows/docbuild.yml)
 [![Build status](https://ci.appveyor.com/api/projects/status/github/datalad/datalad-catalog?branch=main&svg=true)](https://ci.appveyor.com/project/mih/datalad-catalog/branch/main)
 [![codecov.io](https://codecov.io/github/datalad/datalad-catalog/coverage.svg?branch=main)](https://codecov.io/github/datalad/datalad-catalog?branch=main)
 [![crippled-filesystems](https://github.com/datalad/datalad-catalog/actions/workflows/test_crippledfs.yml/badge.svg)](https://github.com/datalad/datalad-catalog/actions/workflows/test_crippledfs.yml)
 [![pages-build-deployment](https://github.com/datalad/datalad-catalog/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/datalad/datalad-catalog/actions/workflows/pages/pages-build-deployment)
-[![push_catalog_to_gh_pages](https://github.com/datalad/datalad-catalog/actions/workflows/deploy_demo.yml/badge.svg)](https://github.com/datalad/datalad-catalog/actions/workflows/deploy_demo.yml)
-[![DOI](https://zenodo.org/badge/371040885.svg)](https://zenodo.org/badge/latestdoi/371040885)
-<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
+[![push_catalog_to_gh_pages](https://github.com/datalad/datalad-catalog/actions/workflows/deploy_demo.yml/badge.svg)](https://github.com/datalad/datalad-catalog/actions/workflows/deploy_demo.yml)<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
 [![All Contributors](https://img.shields.io/badge/all_contributors-11-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 
 <picture>
   <source media="(prefers-color-scheme: light)" srcset="docs/source/_static/datacat0_hero.svg">
   <source media="(prefers-color-scheme: dark)" srcset="docs/source/_static/datacat0_hero_lightbg.svg">
```

### Comparing `datalad_catalog-0.2.1b0/_datalad_buildsupport/__init__.py` & `datalad_catalog-0.2.2/_datalad_buildsupport/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.1b0/_datalad_buildsupport/formatters.py` & `datalad_catalog-0.2.2/_datalad_buildsupport/formatters.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     def _mk_title(self, prog):
         name_version = "{0} {1}".format(prog, self._version)
         return '.TH "{0}" "{1}" "{2}" "{3}"\n'.format(
             prog, self._section, self._today, name_version)
 
     def _mk_name(self, prog, desc):
         """
-        this method is in consistent with others ... it relies on
+        this method is in consitent with others ... it relies on
         distribution
         """
         desc = desc.splitlines()[0] if desc else 'it is in the name'
         # ensure starting lower case
         desc = desc[0].lower() + desc[1:]
         return '.SH NAME\n%s \\- %s\n' % (self._bold(prog), desc)
```

### Comparing `datalad_catalog-0.2.1b0/_datalad_buildsupport/setup.py` & `datalad_catalog-0.2.2/_datalad_buildsupport/setup.py`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/__init__.py` & `datalad_catalog-0.2.2/datalad_catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/catalog/README.md` & `datalad_catalog-0.2.2/datalad_catalog/catalog/README.md`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/catalog/artwork/404.svg` & `datalad_catalog-0.2.2/datalad_catalog/catalog/artwork/404.svg`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/catalog/artwork/catalog_logo.svg` & `datalad_catalog-0.2.2/datalad_catalog/catalog/artwork/catalog_logo.svg`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/catalog/artwork/datalad_catalog_logo_1_dark.svg` & `datalad_catalog-0.2.2/datalad_catalog/catalog/artwork/datalad_catalog_logo_1_dark.svg`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/catalog/artwork/datalad_catalog_logo_1_light.svg` & `datalad_catalog-0.2.2/datalad_catalog/catalog/artwork/datalad_catalog_logo_1_light.svg`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/catalog/artwork/datalad_logo_wide.svg` & `datalad_catalog-0.2.2/datalad_catalog/catalog/artwork/datalad_logo_wide.svg`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/catalog/artwork/ginfavicon.png` & `datalad_catalog-0.2.2/datalad_catalog/catalog/artwork/ginfavicon.png`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/catalog/assets/app.js` & `datalad_catalog-0.2.2/datalad_catalog/catalog/assets/app.js`

 * *Files 18% similar despite different names*

#### js-beautify {}

```diff
@@ -4,31 +4,37 @@
 
 // Start Vue instance
 var datacat = new Vue({
     el: "#datacat",
     data: {
         selectedDataset: {},
         logo_path: "",
-        links: {},
-        dataset_options: {},
-        config_ready: false,
     },
     methods: {
         gotoHome() {
             router.push({
                 name: "home"
             });
         },
         gotoAbout() {
             router.push({
                 name: "about"
             });
         },
         gotoExternal(dest) {
-            window.open(dest);
+            const destinations = {
+                github: "https://github.com/datalad/datalad-catalog",
+                docs: "https://docs.datalad.org/projects/catalog/en/latest/",
+                twitter: "https://twitter.com/datalad",
+            };
+            if (dest in destinations) {
+                window.open(destinations[dest]);
+            } else {
+                window.open(dest);
+            }
         },
         async load() {
             // Load templates
             await Promise.all(
                 Object.keys(template_paths).map(async (key, index) => {
                     url = template_dir + "/" + template_paths[key]
                     fetch(url).
@@ -54,18 +60,14 @@
                         "WARNING: config.json file could not be loaded; using defaults."
                     );
                     return default_config;
                 }
             })
             .then((responseJson) => {
                 obj = responseJson;
-                // set social links
-                this.social_links = obj.social_links
-                // set dataset options
-                this.dataset_options = obj.dataset_options
                 // Set color scheme
                 const style_text =
                     ":root{--link-color: " +
                     responseJson.link_color +
                     "; --link-hover-color: " +
                     responseJson.link_hover_color +
                     ";}";
@@ -77,15 +79,14 @@
                 // Set logo
                 if (obj.logo_path) {
                     this.logo_path = obj.logo_path;
                 } else {
                     this.logo_path = default_config.logo_path;
                 }
                 // Settings for multiple property sources
-                this.config_ready = true
             })
             .catch((error) => {
                 console.log("Config file error:");
                 console.log(error);
                 this.logo_path = default_config.logo_path;
             });
     },
```

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/catalog/assets/app_component_dataset.js` & `datalad_catalog-0.2.2/datalad_catalog/catalog/assets/app_component_dataset.js`

 * *Files 20% similar despite different names*

#### js-beautify {}

```diff
@@ -101,20 +101,20 @@
                     if (
                         !dataset.hasOwnProperty("license") ||
                         !dataset["license"].hasOwnProperty("name") ||
                         !dataset["license"]["name"]
                     ) {
                         disp_dataset["license"] = "not available";
                     }
-                    // Most recent metadata update
-                    sorted_metadata_sources = dataset.metadata_sources.sources.sort(
-                        (a, b) => b.source_time - a.source_time
+                    // Latest extracted time
+                    sorted_extractors = dataset.extractors_used.sort(
+                        (a, b) => b.extraction_time - a.extraction_time
                     );
-                    disp_dataset.last_updated = this.getDateFromUTCseconds(
-                        sorted_metadata_sources[0].source_time
+                    disp_dataset.metadata_extracted = this.getDateFromUTCseconds(
+                        sorted_extractors[0].extraction_time
                     );
                     // ID, version and location
                     disp_dataset.file_path =
                         "metadata/" +
                         getRelativeFilePath(
                             dataset.dataset_id,
                             dataset.dataset_version,
@@ -139,18 +139,15 @@
                                 disp_dataset.is_github = true;
                                 disp_dataset.url = dataset.url[i];
                                 disp_dataset.url = disp_dataset.url.replace('git@github.com:', 'https://github.com');
                             }
                             if (dataset.url[i].toLowerCase().indexOf("gin.g-node") >= 0) {
                                 disp_dataset.is_gin = true;
                                 disp_dataset.url = dataset.url[i];
-                                disp_dataset.url = disp_dataset.url.replace('ssh://', '');
                                 disp_dataset.url = disp_dataset.url.replace('git@gin.g-node.org:', 'https://gin.g-node.org');
-                                disp_dataset.url = disp_dataset.url.replace('git@gin.g-node.org', 'https://gin.g-node.org');
-                                disp_dataset.url = disp_dataset.url.replace('.git', '');
                             }
                         }
                         if (!disp_dataset.url) {
                             disp_dataset.url = dataset.url[0];
                         }
                     } else {
                         disp_dataset.url = dataset.url;
@@ -169,39 +166,14 @@
                     if (
                         (dataset.hasOwnProperty("description") &&
                             dataset["description"] instanceof String) ||
                         typeof dataset["description"] === "string"
                     ) {
                         this.description_ready = true;
                     }
-                    // Create href mailto for request access contact
-                    if (
-                        dataset.hasOwnProperty("access_request_contact") &&
-                        dataset["access_request_contact"]
-                    ) {
-                        var email_to = dataset.access_request_contact.email
-                        var email_subject = "Access request: " + disp_dataset.short_name
-
-                        disp_dataset.access_request_mailto =
-                            "mailto:" +
-                            email_to +
-                            "?subject=" +
-                            email_subject +
-                            "&body=Dear%20" +
-                            dataset.access_request_contact.givenName +
-                            "%20" +
-                            dataset.access_request_contact.familyName;
-                    }
-                    // Rendering options for dataset page
-                    if (this.$root.hasOwnProperty("dataset_options") && this.$root.dataset_options.hasOwnProperty("include_metadata_export")) {
-                        disp_dataset.show_export = this.$root.dataset_options.include_metadata_export
-                    } else {
-                        disp_dataset.show_export = false
-                    }
-                    // Write main derived variable and set to ready
                     this.displayData = disp_dataset;
                     this.display_ready = true;
                 }
             },
         },
         computed: {
             filteredSubdatasets() {
@@ -246,39 +218,30 @@
                             1 :
                             -1
                         );
                     }
                 } else {
                     if (this.sort_modified) {
                         sorted = subdatasets.sort((a, b) =>
-                            a.source_time > b.source_time ? 1 : -1
+                            a.extraction_time > b.extraction_time ? 1 : -1
                         );
                     } else {
                         sorted = subdatasets.sort((a, b) =>
-                            a.source_time < b.source_time ? 1 : -1
+                            a.extraction_time < b.extraction_time ? 1 : -1
                         );
                     }
                 }
                 return sorted;
             },
         },
         methods: {
-            newTabActivated(newTabIndex, prevTabIndex, bvEvent) {
-                if (newTabIndex == 1) {
-                    this.getFiles()
-                }
-            },
             copyCloneCommand(index) {
                 // https://stackoverflow.com/questions/60581285/execcommand-is-now-obsolete-whats-the-alternative
                 // https://www.sitepoint.com/clipboard-api/
                 selectText = document.getElementById("clone_code").textContent;
-                selectText = '\n      ' + selectText + '  \n\n  '
-                console.log(selectText)
-                selectText = selectText.replace(/^\s+|\s+$/g, '');
-                console.log(selectText)
                 navigator.clipboard
                     .writeText(selectText)
                     .then(() => {})
                     .catch((error) => {
                         alert(`Copy failed! ${error}`);
                     });
                 this.showCopyTooltip = true;
@@ -301,37 +264,30 @@
                 this.showCopyCiteTooltip = true;
             },
             hideCiteTooltipLater() {
                 setTimeout(() => {
                     this.showCopyCiteTooltip = false;
                 }, 1000);
             },
-            async selectDataset(event, obj, objId, objVersion, objPath) {
-                var newBrowserTab = event.ctrlKey || event.metaKey || (event.button == 1)
+            async selectDataset(obj, objId, objVersion, objPath) {
                 if (obj != null) {
                     objId = obj.dataset_id;
                     objVersion = obj.dataset_version;
                     objPath = obj.path;
                 }
                 file = getFilePath(objId, objVersion, objPath);
                 fileExists = await checkFileExists(file);
                 if (fileExists) {
-                    const route_info = {
+                    router.push({
                         name: "dataset",
                         params: {
                             dataset_id: objId,
                             dataset_version: objVersion,
                         },
-                    }
-                    if (newBrowserTab) {
-                        const routeData = router.resolve(route_info);
-                        window.open(routeData.href, '_blank');
-                    } else {
-                        router.push(route_info);
-                    }
+                    });
                 } else {
                     console.log(this.$root.subNotAvailable);
                     this.$root.$emit("bv::show::modal", "modal-3", "#btnShow");
                 }
             },
             selectDescription(desc) {
                 if (desc.content.startsWith("path:")) {
@@ -444,15 +400,14 @@
             onClose() {
                 this.popoverShow = false;
             },
             validator(tag) {
                 return this.tag_options_available.indexOf(tag) >= 0;
             },
             getFiles() {
-                this.files_ready = false;
                 this.$root.selectedDataset.tree = this.$root.selectedDataset["children"];
                 this.files_ready = true;
             },
             async getNodeChildren() {
                 this.files_ready = false;
                 file_hash = this.selectedDataset.children;
                 file = metadata_dir + "/" + file_hash + ".json";
@@ -480,52 +435,19 @@
                                 this.citation_busy = false;
                             });
                     } else {
                         this.invalid_doi = true;
                     }
                 }
             },
-            tabsChanged(currentTabs, previousTabs) {
-                this.setCorrectTab(
-                    this.$root.selectedDataset.has_subdatasets,
-                    this.$root.selectedDataset.has_files
-                )
-            },
-            setCorrectTab(has_subdatasets, has_files) {
-                // now set the correct tab:
-                var tabs = this.$refs['alltabs'].$children.filter(
-                    child => typeof child.$vnode.key === 'string' || child.$vnode.key instanceof String
-                ).map(child => child.$vnode.key)
-                var tab_param = this.$route.params.tab_name;
-                if (!tab_param) {
-                    if (has_subdatasets) {
-                        this.tabIndex = 0;
-                    } else {
-                        if (has_files) {
-                            this.tabIndex = 1;
-                        } else {
-                            if (tabs.length > 2) {
-                                this.tabIndex = 2;
-                            } else {
-                                this.tabIndex = 0;
-                            }
-                        }
-                    }
-                } else {
-                    selectTab = tabs.indexOf(tab_param)
-                    if (selectTab >= 0) {
-                        this.tabIndex = selectTab;
-                    } else {
-                        this.tabIndex = 0;
-                    }
-                }
-            }
         },
         async beforeRouteUpdate(to, from, next) {
-            this.tabIndex = 0;
+            if (this.tabIndex != 1) {
+                this.tabIndex = 0;
+            }
             this.subdatasets_ready = false;
             this.dataset_ready = false;
 
             file = getFilePath(to.params.dataset_id, to.params.dataset_version, null);
             response = await fetch(file);
             text = await response.text();
             this.$root.selectedDataset = JSON.parse(text);
@@ -554,19 +476,19 @@
                 this.$root.selectedDataset.hasOwnProperty("subdatasets") &&
                 this.$root.selectedDataset.subdatasets instanceof Array &&
                 this.$root.selectedDataset.subdatasets.length > 0
             ) {
                 subds_json = await grabSubDatasets(this.$root);
                 subds_json.forEach((subds, index) => {
                     if (subds_json[index] != "unavailable") {
-                        sorted_metadata_sources = subds_json[index].metadata_sources.sources.sort(
-                            (a, b) => b.source_time - a.source_time
+                        sorted_extractors = subds_json[index].extractors_used.sort(
+                            (a, b) => b.extraction_time - a.extraction_time
                         );
-                        this.$root.selectedDataset.subdatasets[index].source_time =
-                            sorted_metadata_sources[0].source_time;
+                        this.$root.selectedDataset.subdatasets[index].extraction_time =
+                            sorted_extractors[0].extraction_time;
                         this.$root.selectedDataset.subdatasets[index].name = subds_json[index]
                             .name ?
                             subds_json[index].name :
                             "";
                         this.$root.selectedDataset.subdatasets[index].short_name = subds_json[
                                 index
                             ].short_name ?
@@ -592,84 +514,46 @@
                             subds_json[index].keywords :
                             [];
                         this.$root.selectedDataset.subdatasets[index].available = "true";
                     } else {
                         this.$root.selectedDataset.subdatasets[index].available = "false";
                     }
                 });
-                subdatasets_available = this.$root.selectedDataset.subdatasets.filter(
-                    (obj) => obj.available == "true"
-                );
-                subdatasets_unavailable = this.$root.selectedDataset.subdatasets.filter(
-                    (obj) => obj.available == "false"
-                );
-                this.$root.selectedDataset.subdatasets_count = this.$root.selectedDataset.subdatasets.length
-                this.$root.selectedDataset.subdatasets_available_count = subdatasets_available.length
-                this.$root.selectedDataset.subdatasets_unavailable_count = subdatasets_unavailable.length
                 this.subdatasets_ready = true;
-                this.$root.selectedDataset.has_subdatasets = true;
+                console.log(this.subdatasets_ready);
             } else {
                 this.$root.selectedDataset.subdatasets = [];
-                this.$root.selectedDataset.subdatasets_count = 0
-                this.$root.selectedDataset.subdatasets_available_count = 0
-                this.$root.selectedDataset.subdatasets_unavailable_count = 0
                 this.subdatasets_ready = true;
-                this.$root.selectedDataset.has_subdatasets = false;
-            }
-            // Now check file content
-            this.files_ready = false;
-            this.$root.selectedDataset.tree = this.$root.selectedDataset["children"];
-            this.files_ready = true;
-            if (
-                this.$root.selectedDataset.hasOwnProperty("tree") &&
-                this.$root.selectedDataset.tree instanceof Array &&
-                this.$root.selectedDataset.tree.length > 0
-            ) {
-                this.$root.selectedDataset.has_files = true;
-            } else {
-                this.$root.selectedDataset.has_files = false;
             }
-            // now set the correct tab:
-            this.setCorrectTab(
-                this.$root.selectedDataset.has_subdatasets,
-                this.$root.selectedDataset.has_files
-            )
             next();
         },
         async created() {
             file = getFilePath(
                 this.$route.params.dataset_id,
                 this.$route.params.dataset_version,
                 null
             );
             var app = this.$root;
             response = await fetch(file);
-            // Reroute to 404 if the dataset file is not found
-            if (response.status == 404) {
-                router.push({
-                    name: "404",
-                });
-                return;
-            }
             text = await response.text();
             app.selectedDataset = JSON.parse(text);
             this.dataset_ready = true;
             if (
                 this.$root.selectedDataset.hasOwnProperty("subdatasets") &&
                 this.$root.selectedDataset.subdatasets instanceof Array &&
                 this.$root.selectedDataset.subdatasets.length > 0
             ) {
                 subds_json = await grabSubDatasets(app);
                 subds_json.forEach((subds, index) => {
                     if (subds_json[index] != "unavailable") {
-                        sorted_metadata_sources = subds_json[index].metadata_sources.sources.sort(
-                            (a, b) => b.source_time - a.source_time
+                        sorted_extractors = subds_json[index].extractors_used.sort(
+                            (a, b) => b.extraction_time - a.extraction_time
                         );
-                        this.$root.selectedDataset.subdatasets[index].source_time =
-                            sorted_metadata_sources[0].source_time;
+                        this.$root.selectedDataset.subdatasets[index].extraction_time =
+                            sorted_extractors[0].extraction_time;
                         this.$root.selectedDataset.subdatasets[index].name =
                             subds_json[index].name;
                         this.$root.selectedDataset.subdatasets[index].short_name =
                             subds_json[index].short_name;
                         this.$root.selectedDataset.subdatasets[index].doi =
                             subds_json[index].doi;
                         this.$root.selectedDataset.subdatasets[index].license =
@@ -679,50 +563,19 @@
                         this.$root.selectedDataset.subdatasets[index].keywords =
                             subds_json[index].keywords;
                         this.$root.selectedDataset.subdatasets[index].available = "true";
                     } else {
                         this.$root.selectedDataset.subdatasets[index].available = "false";
                     }
                 });
-                subdatasets_available = this.$root.selectedDataset.subdatasets.filter(
-                    (obj) => obj.available == "true"
-                );
-                subdatasets_unavailable = this.$root.selectedDataset.subdatasets.filter(
-                    (obj) => obj.available == "false"
-                );
-                this.$root.selectedDataset.subdatasets_count = this.$root.selectedDataset.subdatasets.length
-                this.$root.selectedDataset.subdatasets_available_count = subdatasets_available.length
-                this.$root.selectedDataset.subdatasets_unavailable_count = subdatasets_unavailable.length
                 this.subdatasets_ready = true;
-                this.$root.selectedDataset.has_subdatasets = true;
             } else {
                 this.$root.selectedDataset.subdatasets = [];
-                this.$root.selectedDataset.subdatasets_count = 0
-                this.$root.selectedDataset.subdatasets_available_count = 0
-                this.$root.selectedDataset.subdatasets_unavailable_count = 0
                 this.subdatasets_ready = true;
-                this.$root.selectedDataset.has_subdatasets = false;
-            }
-            // Now check file content
-            this.files_ready = false;
-            this.$root.selectedDataset.tree = this.$root.selectedDataset["children"];
-            this.files_ready = true;
-            if (
-                this.$root.selectedDataset.hasOwnProperty("tree") &&
-                this.$root.selectedDataset.tree instanceof Array &&
-                this.$root.selectedDataset.tree.length > 0
-            ) {
-                this.$root.selectedDataset.has_files = true;
-            } else {
-                this.$root.selectedDataset.has_files = false;
             }
-            this.setCorrectTab(
-                this.$root.selectedDataset.has_subdatasets,
-                this.$root.selectedDataset.has_files
-            )
         },
         mounted() {
             this.tag_options_filtered = this.tag_options;
             this.tag_options_available = this.tag_options;
         }
     }
 })
```

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/catalog/assets/app_component_item.js` & `datalad_catalog-0.2.2/datalad_catalog/catalog/assets/app_component_item.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -11,15 +11,14 @@
             props: {
                 item: [Object, Array, String, Number],
             },
             data: function() {
                 return {
                     isOpen: false,
                     files_ready: false,
-                    spinner_on: null,
                     children: [],
                 };
             },
             computed: {
                 isFolder: function() {
                     return this.item.type === "directory";
                 },
@@ -37,16 +36,14 @@
                 },
             },
             methods: {
                 async toggle() {
                     if (this.isFolder) {
                         tempIsOpen = !this.isOpen;
                         if (tempIsOpen && !this.item.hasOwnProperty("children")) {
-                            this.files_ready = false;
-                            this.spinner_on = true;
                             obj = await this.getChildren(this.item);
                             this.item.children = obj["children"];
                             // go through all children, set state to enabled
                             // then set disabled state for subdatasets that aren't part of catalog
                             await Promise.all(
                                 this.item.children.map(async (child, index) => {
                                     child['state'] = 'enabled'
@@ -56,44 +53,36 @@
                                         if (!fileExists) {
                                             child['state'] = 'disabled'
                                         }
                                     }
                                 })
                             );
                             this.files_ready = true;
-                            this.spinner_on = false;
                         }
                         this.isOpen = !this.isOpen;
                     }
                 },
-                async selectDataset(event, obj, objId, objVersion) {
-                    var newBrowserTab = event.ctrlKey || event.metaKey || (event.button == 1)
+                async selectDataset(obj, objId, objVersion) {
                     if (obj != null) {
                         objId = obj.dataset_id;
                         objVersion = obj.dataset_version;
                     }
                     // This check should not be necessary, because unavailable
                     // subdatasets are already disabled, but the check is left here
                     // to cover any other possible reasons for a file being unavailable
                     file = getFilePath(objId, objVersion, "");
                     fileExists = await checkFileExists(file);
                     if (fileExists) {
-                        const route_info = {
+                        router.push({
                             name: "dataset",
                             params: {
                                 dataset_id: objId,
                                 dataset_version: objVersion,
                             },
-                        }
-                        if (newBrowserTab) {
-                            const routeData = router.resolve(route_info);
-                            window.open(routeData.href, '_blank');
-                        } else {
-                            router.push(route_info);
-                        }
+                        });
                     } else {
                         console.log(this.$root.subNotAvailable);
                         this.$root.$emit("bv::show::modal", "modal-3", "#btnShow");
                     }
                 },
                 formatBytes(bytes, decimals = 2) {
                     if (bytes === 0) return "0 Bytes";
```

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/catalog/assets/app_globals.js` & `datalad_catalog-0.2.2/datalad_catalog/catalog/assets/app_globals.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -9,23 +9,14 @@
 const SPLIT_INDEX = 3;
 const SHORT_NAME_LENGTH = 0; // number of characters in name to display, zero if all
 const default_config = {
     catalog_name: "DataCat",
     link_color: "#fba304",
     link_hover_color: "#af7714",
     logo_path: "artwork/catalog_logo.svg",
-    social_links: {
-        about: null,
-        documentation: null,
-        github: null,
-        twitter: null,
-    },
-    dataset_options: {
-        include_metadata_export: true,
-    }
 };
 const template_dir = "./templates";
 
 /*************/
 // Functions //
 /*************/
```

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/catalog/assets/app_router.js` & `datalad_catalog-0.2.2/datalad_catalog/catalog/assets/app_router.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -32,15 +32,15 @@
                 }
             }
         };
         rawFile.open("GET", superfile, false);
         rawFile.send();
     },
 }, {
-    path: "/dataset/:dataset_id/:dataset_version/:tab_name?",
+    path: "/dataset/:dataset_id/:dataset_version",
     component: datasetView,
     name: "dataset",
 }, {
     path: "/about",
     component: aboutPage,
     name: "about"
 }, {
```

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/catalog/assets/bootstrap-vue.2.21.2.min.css` & `datalad_catalog-0.2.2/datalad_catalog/catalog/assets/bootstrap-vue.2.21.2.min.css`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/catalog/assets/bootstrap-vue.2.21.2.min.js` & `datalad_catalog-0.2.2/datalad_catalog/catalog/assets/bootstrap-vue.2.21.2.min.js`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/catalog/assets/bootstrap.5.1.3.min.css` & `datalad_catalog-0.2.2/datalad_catalog/catalog/assets/bootstrap.5.1.3.min.css`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/catalog/assets/brands.min.css` & `datalad_catalog-0.2.2/datalad_catalog/catalog/assets/brands.min.css`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/catalog/assets/display_schema.js` & `datalad_catalog-0.2.2/datalad_catalog/catalog/assets/display_schema.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 /**************/
 // Components //
 /**************/
 
 const dataset_schema_file = "./assets/jsonschema_dataset.json";
 const authors_schema_file = "./assets/jsonschema_authors.json";
 const file_schema_file = "./assets/jsonschema_file.json";
-const sources_schema_file = "./assets/jsonschema__metadata_sources.json";
+const extractors_schema_file = "./assets/jsonschema_extractors.json";
 const catalog_schema_file = "./assets/jsonschema_catalog.json";
 
 const TYPES = [
     "string",
     "number",
     "integer",
     "object",
@@ -31,15 +31,15 @@
 
 
 schema_files = {
     // "jsonschema_catalog": catalog_schema_file,
     "jsonschema_dataset": dataset_schema_file,
     "jsonschema_file": file_schema_file,
     "jsonschema_authors": authors_schema_file,
-    "jsonschema__metadata_sources": sources_schema_file,
+    "jsonschema_extractors": extractors_schema_file,
 }
 
 schema_keywords = ["$schema", "$id"]
 instance_keywords = ["type"]
 schema_annotations = ["title", "description", "default", "examples", "readOnly", "writeOnly", "deprecated"]
 additional_schema_keywords = ["$ref", "$defs"]
 // validation_keywords = ["properties", "additionalProperties", "required", "items", "multipleOf", "maximum", "minimum", "exclusiveMaximum", "exclusiveMinimum", "minItems", "maxItems", "uniqueItems"]
```

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/catalog/assets/fa-brands-400.woff2` & `datalad_catalog-0.2.2/datalad_catalog/catalog/assets/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/catalog/assets/fa-regular-400.woff2` & `datalad_catalog-0.2.2/datalad_catalog/catalog/assets/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/catalog/assets/fa-solid-900.woff2` & `datalad_catalog-0.2.2/datalad_catalog/catalog/assets/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/catalog/assets/favicon/favicon.ico` & `datalad_catalog-0.2.2/datalad_catalog/catalog/assets/favicon/favicon.ico`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/catalog/assets/fontawesome.min.css` & `datalad_catalog-0.2.2/datalad_catalog/catalog/assets/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/catalog/assets/jsonschema_authors.json` & `datalad_catalog-0.2.2/datalad_catalog/catalog/assets/jsonschema_authors.json`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/catalog/assets/jsonschema_catalog.json` & `datalad_catalog-0.2.2/datalad_catalog/catalog/assets/jsonschema_catalog.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8571428571428571%*

 * *Differences: {'delete': "['version']"}*

```diff
@@ -25,10 +25,9 @@
             "then": {
                 "$ref": "https://datalad.org/catalog.file.schema.json"
             }
         }
     ],
     "description": "The main catalog schema",
     "title": "catalog",
-    "type": "object",
-    "version": "1.0.0"
+    "type": "object"
 }
```

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/catalog/assets/jsonschema_dataset.json` & `datalad_catalog-0.2.2/datalad_catalog/catalog/assets/jsonschema_dataset.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9853869047619047%*

 * *Differences: {"'properties'": "{'additional_display': {'description': 'Additonal items to display in tabs on "*

 * *                 "dataset page'}, 'top_display': {'description': 'Additonal items to display at "*

 * *                 "the top of the dataset page (along with keywords, description, etc)'}, "*

 * *                 "'extractors_used': OrderedDict([('$ref', "*

 * *                 "'https://datalad.org/catalog.extractors.schema.json')]), delete: "*

 * *                 "['access_request_contact', 'access_request_url', 'metadata_so […]*

```diff
@@ -1,78 +1,14 @@
 {
     "$id": "https://datalad.org/catalog.dataset.schema.json",
     "$schema": "https://json-schema.org/draft/2020-12/schema",
     "description": "A dataset in a DataLad Catalog",
     "properties": {
-        "access_request_contact": {
-            "description": "The contact details of the person/office from which to request access to the dataset content",
-            "properties": {
-                "email": {
-                    "description": "Email address of the author, such as johndoe@example.com",
-                    "format": "email",
-                    "title": "Email",
-                    "type": "string"
-                },
-                "familyName": {
-                    "description": "The author's last/family name, such as 'Doe'",
-                    "title": "Family name",
-                    "type": "string"
-                },
-                "givenName": {
-                    "description": "The author's given name, such as 'John'",
-                    "title": "Given name",
-                    "type": "string"
-                },
-                "honorificSuffix": {
-                    "description": "Title of the author, such as 'Dr.'",
-                    "title": "Honorific suffix",
-                    "type": "string"
-                },
-                "identifiers": {
-                    "description": "Identifiers for the person",
-                    "items": {
-                        "properties": {
-                            "identifier": {
-                                "description": "The actual identifier, such as the ORCID ID '0000-1212-5566'",
-                                "title": "Identifier",
-                                "type": "string"
-                            },
-                            "type": {
-                                "description": "Type of identifier, such as 'ORCID'",
-                                "title": "Type",
-                                "type": "string"
-                            }
-                        },
-                        "type": "object"
-                    },
-                    "title": "Identifiers",
-                    "type": "array"
-                },
-                "name": {
-                    "description": "A concatenation of the honorificSuffix, givenName and familyName properties, such as 'Dr. John Doe'",
-                    "title": "Name",
-                    "type": "string"
-                }
-            },
-            "required": [
-                "givenName",
-                "familyName",
-                "email"
-            ],
-            "title": "Access Request Contact",
-            "type": "object"
-        },
-        "access_request_url": {
-            "description": "The url of the online location from which to request access to the dataset content",
-            "format": "uri",
-            "title": "Access Request URL",
-            "type": "string"
-        },
         "additional_display": {
-            "description": "Additional items to display in tabs on dataset page",
+            "description": "Additonal items to display in tabs on dataset page",
             "items": {
                 "properties": {
                     "content": {
                         "description": "The content that will appear in the tab when opened, specified as key-value pairs",
                         "title": "Content",
                         "type": "object"
                     },
@@ -119,14 +55,17 @@
             ]
         },
         "doi": {
             "description": "The dataset's digital object identifier",
             "title": "DOI",
             "type": "string"
         },
+        "extractors_used": {
+            "$ref": "https://datalad.org/catalog.extractors.schema.json"
+        },
         "funding": {
             "description": "Sources of funding for the dataset",
             "items": {
                 "properties": {
                     "description": {
                         "description": "Free form description of grant or funding",
                         "title": "Description",
@@ -184,17 +123,14 @@
                     "description": "A URL where a description of the license can be viewed",
                     "title": "URL",
                     "type": "string"
                 }
             },
             "type": "object"
         },
-        "metadata_sources": {
-            "$ref": "https://datalad.org/catalog.metadata_sources.schema.json"
-        },
         "name": {
             "description": "The long name of the dataset",
             "title": "Name",
             "type": "string"
         },
         "publications": {
             "description": "Publications related to the dataset",
@@ -276,15 +212,15 @@
                 "type": "object"
             },
             "title": "Subdatasets",
             "type": "array",
             "uniqueItems": true
         },
         "top_display": {
-            "description": "Additional items to display at the top of the dataset page (along with keywords, description, etc)",
+            "description": "Additonal items to display at the top of the dataset page (along with keywords, description, etc)",
             "items": {
                 "properties": {
                     "name": {
                         "description": "Name of the item that will appear as part of the top display",
                         "title": "Name",
                         "type": "string"
                     },
```

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/catalog/assets/jsonschema_file.json` & `datalad_catalog-0.2.2/datalad_catalog/catalog/assets/jsonschema_file.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9837301587301587%*

 * *Differences: {"'properties'": "{'additional_display': {'description': 'Additonal items to display on the file "*

 * *                 "level'}, 'extractors_used': OrderedDict([('$ref', "*

 * *                 "'https://datalad.org/catalog.extractors.schema.json')]), delete: "*

 * *                 "['metadata_sources']}"}*

```diff
@@ -1,14 +1,14 @@
 {
     "$id": "https://datalad.org/catalog.file.schema.json",
     "$schema": "https://json-schema.org/draft/2020-12/schema",
     "description": "A file in a DataLad Catalog",
     "properties": {
         "additional_display": {
-            "description": "Additional items to display on the file level",
+            "description": "Additonal items to display on the file level",
             "items": {
                 "properties": {
                     "content": {
                         "description": "The content that will appear when selecting the file, specified as key-value pairs",
                         "title": "Content",
                         "type": "object"
                     },
@@ -39,16 +39,16 @@
             "type": "string"
         },
         "dataset_version": {
             "description": "The parent dataset VERSION",
             "title": "Dataset version",
             "type": "string"
         },
-        "metadata_sources": {
-            "$ref": "https://datalad.org/catalog.metadata_sources.schema.json"
+        "extractors_used": {
+            "$ref": "https://datalad.org/catalog.extractors.schema.json"
         },
         "path": {
             "description": "The path of the file relative to its parent dataset",
             "title": "Path",
             "type": "string"
         },
         "type": {
```

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/catalog/assets/marked.4.0.17.min.js` & `datalad_catalog-0.2.2/datalad_catalog/catalog/assets/marked.4.0.17.min.js`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/catalog/assets/md5-2.3.0.js` & `datalad_catalog-0.2.2/datalad_catalog/catalog/assets/md5-2.3.0.js`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/catalog/assets/meta_entry.js` & `datalad_catalog-0.2.2/datalad_catalog/catalog/assets/meta_entry.js`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/catalog/assets/style.css` & `datalad_catalog-0.2.2/datalad_catalog/catalog/assets/style.css`

 * *Files 1% similar despite different names*

```diff
@@ -42,18 +42,14 @@
 }
 
 body {
   font-family: Menlo, Consolas, monospace;
   color: #444;
 }
 
-a:hover {
-  cursor: pointer;
-}
-
 .item {
   cursor: pointer;
   font-family: Menlo, Consolas, monospace;
 }
 
 .bold {
   font-weight: bold;
```

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/catalog/assets/vue-router.3.5.3.min.js` & `datalad_catalog-0.2.2/datalad_catalog/catalog/assets/vue-router.3.5.3.min.js`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/catalog/assets/vue.2.6.14.min.js` & `datalad_catalog-0.2.2/datalad_catalog/catalog/assets/vue.2.6.14.min.js`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/catalog/config.json` & `datalad_catalog-0.2.2/datalad_catalog/config/config.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.375%*

 * *Differences: {"'logo_path'": "''",*

 * * "'property_source'": "OrderedDict([('dataset', OrderedDict([('dataset_id', 'metalad_core'), "*

 * *                      "('dataset_version', 'metalad_core'), ('type', 'metalad_core'), ('children', "*

 * *                      "'merge'), ('name', 'metalad_studyminimeta'), ('short_name', ''), "*

 * *                      "('description', ['metalad_studyminimeta', 'datacite_gin', 'readme.md']), "*

 * *                      "('doi', ''), ('url', 'merge'), ('authors', 'merge'), ('keywords', 'merge'), "*

 * *      […]*

```diff
@@ -1,44 +1,32 @@
 {
     "catalog_name": "DataCat",
-    "dataset_options": {
-        "include_metadata_export": true
-    },
     "link_color": "#fba304",
     "link_hover_color": "#af7714",
-    "property_sources": {
+    "logo_path": "",
+    "property_source": {
         "dataset": {
-            "additional_display": {
-                "rule": "merge",
-                "source": []
-            },
-            "authors": {
-                "rule": "merge",
-                "source": [
-                    "metalad_studyminimeta"
-                ]
-            },
-            "description": {
-                "rule": "priority",
-                "source": [
-                    "metalad_studyminimeta",
-                    "bids_dataset"
-                ]
-            },
-            "keywords": {
-                "rule": "merge",
-                "source": "any"
-            },
-            "top_display": {
-                "rule": "merge",
-                "source": []
-            }
-        },
-        "file": {}
-    },
-    "social_links": {
-        "about": null,
-        "documentation": "https://docs.datalad.org/projects/catalog/en/latest/",
-        "github": "https://github.com/datalad/datalad-catalog",
-        "twitter": "https://twitter.com/datalad"
+            "additional_display": "merge",
+            "authors": "merge",
+            "children": "merge",
+            "dataset_id": "metalad_core",
+            "dataset_version": "metalad_core",
+            "description": [
+                "metalad_studyminimeta",
+                "datacite_gin",
+                "readme.md"
+            ],
+            "doi": "",
+            "extractors_used": "merge",
+            "funding": "merge",
+            "keywords": "merge",
+            "license": "",
+            "name": "metalad_studyminimeta",
+            "publications": "merge",
+            "short_name": "",
+            "subdatasets": "merge",
+            "top_display": "merge",
+            "type": "metalad_core",
+            "url": "merge"
+        }
     }
 }
```

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/catalog/display_schema.html` & `datalad_catalog-0.2.2/datalad_catalog/catalog/display_schema.html`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/catalog/index.html` & `datalad_catalog-0.2.2/datalad_catalog/catalog/index.html`

 * *Files 6% similar despite different names*

```diff
@@ -16,43 +16,43 @@
     <link rel="stylesheet" type="text/css" href="assets/style.css"/>
     <link rel="stylesheet" type="text/css" href="assets/fontawesome.min.css"/>
     <link rel="stylesheet" type="text/css" href="assets/brands.min.css"/>
     <link type="text/css" rel="stylesheet" href="assets/bootstrap.5.1.3.min.css"/>
     <link type="text/css" rel="stylesheet" href="assets/bootstrap-vue.2.21.2.min.css"/>
 
     <!-- Required scripts -->
-    <!-- <script src="https://unpkg.com/vue@2.6.14/dist/vue.js"></script> -->
-    <script src="assets/vue.2.6.14.min.js"></script>
+    <script src="https://unpkg.com/vue@2.6.14/dist/vue.js"></script>
+    <!-- <script src="assets/vue.2.6.14.min.js"></script> -->
     <script src="assets/bootstrap-vue.2.21.2.min.js"></script>
     <script src="assets/vue-router.3.5.3.min.js"></script>
     <script src="assets/md5-2.3.0.js"></script>
     <script src="assets/marked.4.0.17.min.js"></script>
     
   </head>
 
   <body id="mainbody">
     <!-- The application root element -->
     <b-container id="datacat" >
-      <b-container v-if="config_ready" style="margin-top:20px;">
+      <b-container style="margin-top:20px;">
         <b-row align-v="end">
           <b-col cols="9">
             <span v-show="logo_path"><a @click="gotoHome"><img :src="logo_path" class="d-inline-block" alt="datalad" style="width:100%;"></a></span>
           </b-col>
           <b-col cols="1"></b-col>
           <b-col cols="2" align-h="end">
             <b-navbar toggleable="lg" type="light" variant="outline-dark">
           
               <b-navbar-toggle target="navbar-toggle-collapse">
               </b-navbar-toggle>
               <b-collapse id="navbar-toggle-collapse" is-nav>
                 <b-navbar-nav class="ml-auto mb-0 xlfont">
-                  <b-nav-item v-if="social_links['about']" v-b-tooltip.hover title="About" @click="gotoExternal(social_links['about'])"><i class="fas fa-info-circle"></i></b-nav-item>
-                  <b-nav-item v-if="social_links['documentation']" v-b-tooltip.hover title="Read documentation" @click="gotoExternal(social_links['documentation'])"><i class="fas fa-file-alt"></i></b-nav-item>
-                  <b-nav-item v-if="social_links['github']" v-b-tooltip.hover title="View code base" @click="gotoExternal(social_links['github'])"><i class="fab fa-github"></i></b-nav-item>
-                  <b-nav-item v-if="social_links['twitter']" v-b-tooltip.hover title="Follow DataLad!" @click="gotoExternal(social_links['twitter'])"><i class="fab fa-twitter"></i></b-nav-item>
+                  <b-nav-item v-b-tooltip.hover title="About" @click="gotoAbout"><i class="fas fa-info-circle"></i></b-nav-item>
+                  <b-nav-item v-b-tooltip.hover title="Read documentation" @click="gotoExternal('docs')"><i class="fas fa-file-alt"></i></b-nav-item>
+                  <b-nav-item v-b-tooltip.hover title="View code base" @click="gotoExternal('github')"><i class="fab fa-github"></i></b-nav-item>
+                  <b-nav-item v-b-tooltip.hover title="Follow DataLad!" @click="gotoExternal('twitter')"><i class="fab fa-twitter"></i></b-nav-item>
                 </b-navbar-nav>
               </b-collapse>
             </b-navbar>
           </b-col>
         </b-row>
       </b-container>
       <br>
```

#### html2text {}

```diff
@@ -7,23 +7,22 @@
 
 
 
 
 
 
 
+
 click="gotoHome">
 src="logo_path" class="d-inline-block" alt="datalad" style="width:100%;">
 
-hover title="About" @click="gotoExternal(social_links['about'])">
-hover title="Read documentation" @click="gotoExternal(social_links
-['documentation'])">
-hover title="View code base" @click="gotoExternal(social_links['github'])">
-hover title="Follow DataLad!" @click="gotoExternal(social_links['twitter'])">
-
+hover title="About" @click="gotoAbout">
+hover title="Read documentation" @click="gotoExternal('docs')">
+hover title="View code base" @click="gotoExternal('github')">
+hover title="Follow DataLad!" @click="gotoExternal('twitter')">
 
 selected-dataset="selectedDataset">
```

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/catalog/metadata-entry.html` & `datalad_catalog-0.2.2/datalad_catalog/catalog/metadata-entry.html`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/catalog/templates/dataset-template.html` & `datalad_catalog-0.2.2/datalad_catalog/catalog/templates/dataset-template.html`

 * *Files 1% similar despite different names*

```diff
@@ -9,37 +9,32 @@
         <!-- DATASET AUTHORS -->
         <b-card-sub-title class="mb-2">
           <span v-for="(author, index) in selectedDataset.authors"><span v-if="author.givenName">{{author.givenName}} {{author.familyName}}</span><span v-else>{{author.name}}</span><span v-if="index != selectedDataset.authors.length - 1">, </span></span>
         </b-card-sub-title>
         <!-- DATASET VERSION ETC -->
         <b-card-text>
           <strong>Version:</strong> {{selectedDataset.dataset_version.substring(0,7)}}&nbsp;
-          <strong>Last updated:</strong> {{displayData.last_updated}}&nbsp;
+          <strong>Metadata extracted:</strong> {{displayData.metadata_extracted}}&nbsp;
           <strong>DOI:</strong> <span v-if="selectedDataset.doi"><a :href="selectedDataset.doi" target="_blank"> {{selectedDataset.doi.replace("https://doi.org/", "")}}</a></span>
-          <span v-else><em>unknown</em></span>&nbsp;
+          <span v-else><em>not available</em></span>&nbsp;
           <strong>License:</strong> <span v-if="selectedDataset.license && selectedDataset.license.name"><a :href="selectedDataset.license.url" target="_blank"> {{selectedDataset.license.name}}</a></span>
-          <span v-else><em>unknown</em></span>
+          <span v-else><em>not available</em></span>
         </b-card-text>
         <!-- DATASET BUTTONS -->
         <div style="text-align: left;">
           <span v-show="displayData.url"><b-button variant="outline-dark" size="sm" v-b-modal.modal-1>
             <img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAMgAAADICAYAAACtWK6eAAAWz0lEQVR4nOzdC3Qb5Zk38GdkjzSKJSPZjq0Z24nt+JIvrl0SSoHCgY/SC7RdStKGBtqFLqXX0KaUa+G0SXq6BOiN0wTasglt093SJoEALRAWaB1KCC0JBWPLcZQoxLF1sWONrItnZEV694imNPEtkjwz72j0/M7JOfHM6H0fO/7n0StpZkrhFGQrbAaAL4ABHDsOj1z+Q/iS2wcprea0WCwlbW1tW1iWvX6a3WkAOJH5MQNAEgASACCf/CMBQIQQEonH45FkMhkGgOOEkOMAMBoOh0cAwE8I8cXj8ZFkMkm0+p6KXSntAlSRhh1ah8NqtZa0t7c/Rgj55AyHmADAfPLvFgCwTT6AYRiw2aZshoqKilO/jBJCekpKSt4YHBx8AwD2RSKRN+LxeFqhbwWdwnABodE5MuFYtGjRllnCoSQ7wzAXpNPpCwRBeGeDIAiZjnRYkqQDsiy7JUl6U5KkbkmSDiYSCQzOHDCnflHwT7HSsKP9LlildTgWL168w2QyXaXVnDmIAMAun8+3U5bl50RRFGkXVGgM00Fodg6dhiOjHACuFgTh6pPrn+54PP7K2NjYHkmSdofDYT/tAvXOGB0EO0c+Mk+9XhFF8RfDw8PbYrHYBO2C9KjgOwh2jryZAOAip9OZ+fPzRCLx4vj4+NOiKD4jiuIg7eL0orADQuHVKovFkukc200m03Kt5tRAmcViuTLzx+l0Zn6WT/v9/nt8Pt9faRdGm4l2AfnKdA6tn1ZlwtHa2rrFYOGYrAQAruR5/pVly5b9vbGx8dsOh6OBdlG0FOYahMKaIxOOJUuWGK1zZI1l2d8dO3bsjqGhoQHatWip4DoIjc6RWXO0tLQYvXPMKplMrnK5XIc7Ozt38Dx/Bcuyhf30PEuFFZA0bKe15rBYLNN9fKTYlLIs+ylBEJ7p7Ox8lef599EuSG0FE5CTneMaXHPoxjmCILzW0dHxDM/zl5vN5oL5XcpFYXxTlDpHZs1hNpuxc8zCbDZfIQjCs52dnc/X1NQspF2P0nQfEOwchYEQ8sG6urr+tra2jU6ns452PUrRd0AodI7MgnzJkiU7sHPkxWKz2W5qamrynn322V+lXYwSdBsQWp1j0aJFmwv8HXI9YEtKSh4655xzXq6urr6YdjFzoc+AUOwcFovl81rNWQQurK+v//PSpUs3cRxnoV1MPnQXEOwchmMymUyrOzs79/I8f5nVaqVdT070FRBKr1Z1dHRg51BZKpVaKgjCCw0NDRto15IL3QTk2Cj8SuvOkdHS0rKZEIKdQyPz5s27c+nSpV1Op7ODdi3Z0E1AIjKUax2OjHQ6Pa71nMXOZDJd0tjYuKelpeUK2rWciW4C0l4LK3o2wON1FXCWlvN6PJ5bJEl68OTVRpBGGIaxl5eX/7G1tXUDx3Es7XpmopuAwD9CsnzXbfCIlnMmk0nZ7XbfJEnSz7ScF73DZLfb72xvb9/NcZym/zFmS1cBAewkxeqClpaWP/E8//9oFzKZ7gIC2EmKktlsXiYIwt95nr+Idi2n0mVAADtJsbIIgrCT5/lP0y7kn3QbEMBOUqyqBEHY3t7eroszW3UdEMBOUrQsFsvGjo6Om8xmM0OzDt0HBLCTFCWGYaxms3ljS0vLGpp1FERAADtJ0eI47t729vbVpaV0ToEvmIAA5U4yPj7+kJbzondZOI7b1NDQQGVNUlABgX91kse07iSHDh26FTsJPWedddYDPM9fqfW8BRcQOBkS7CRFxyYIwk6Xy6XpCVgFGRCguCY52Ukewk5ChUkQhK0ul6tZswm1mkgN76xJbqXSSVZjJ6GDYZiFtbW1XRzHObWYr6ADktFeByt67oHH6pzYSYpIbXNz8xar1ar672/BBwROhoTSmgQ7CSUWi2V5fX39PWrPY4iAAP1Ogq9uUWC32+9oaWlR9XNbhgkI0O0k+I47JeXl5Q/ZbDbV1iOGCghQ7CT4jjs189va2p5lWbZMjcENFxCg3ElwTULFec3Nzd9SY+DCvIFOlnoH4fvvuQu+o+WcLMty9fX112X+enJT5j8hlhBiYRjGDABWQojDbrdXlJaW1jAMIwBAfWbdqWWdRkMIiQQCgYt9Pt+bSo5r6JugtNdCk9ZzZjqJ1+t9OJfH2Gw2xmazLWEY5nxBEC4FgA8BQI16VRoPwzDlPM8/FQqFFsuyLCk1rqEDUihisRiJxWK9mabn9/u3ZLY5nc4WjuPOLS8v/4DNZssEpnVyx0dTLKivr7/T4/GsVWpADIhOiaLoyaz9/X7/bzNfC4LQ6XK5VgPAtQzD2GjXp1fl5eW3NTU1Pez1eoeUGM+Qi3Qj8vl83a+//vqX+/v7G8bGxm5IJBLP4ytm07I6HI4dLMsqsqbDgBSYeDw+eujQoV/29PR8xOfzdRBCumjXpDeZtVxtbe3nlBgLA1LA/H5/b09Pz2U+n++yiYmJP9CuR08qKipu5zhuzpeSx4AUuImJibTf7//TW2+9dWUymbwUAI7RrkkPGIZpXbBgwXfnOg4GxEC6u7u7+vr6zhZFcR0hJES7Htrsdvst1dXV7XMZAwNiMOPj4yGv17v+yJEj5wFAH+16KGPnz58/p6uiYEAMShTFQ263+73xeHwtACRp10MLx3HXOJ3OvN8wxoAYmCRJyQMHDnwvmUx+gBAyQrseSmxNTU0P5vtgDEgR6O7u3uf1ei8hhPyNdi2UXF5dXf3+fB6IASkS4XC4r6+v73yWZZ+mXQsNVVVVX87ncRiQIiJJEtm/f/81kiT9mnYtWrNarZ92Op05fwAUA1Jkkslk1O12f16SpM20a9FYeVNT07dzfRAGpEh5PJ41kiQ9SrsOjX2prKyMz+UBGJAilUwmx91u97VFtiax1tTUrMzlARiQItff3/9FQoibdh1aqaqqwoCg7Imi6Pd4PBcDwHHatWghlUpd6HK5WrI9HgOCIBqNjgaDwa/QrkMjTEVFxd3ZHowBQe8YHBx8LBqNPkC7Di1YrdbPOhyOrC4LhQFB7zp69OhtExMTe2nXoYFSm812RTYHYkDQuxKJxInjx4/fRrsOLZx11lkfz+Y4DAg6jd/v3yNJ0k9o16E2juMus1qtJWc6DgOCphgcHLyVEHKEdh0q451O5yVnOggDgqaIRCLp4eHh+2jXoTaXy3XjmY7BgKBpjY6OPkIIeZt2HWpiGGYFx3GzXh4IA4KmJUlSMhKJXA8AJ2jXoiJLeXn5rOeJYEDQjA4dOvRSOp1+gXYdaiorK7twtv0YEDSrYDBo6BsD2Wy282bbjwFBsxodHf0jABymXYdazGbz+2bbjwFBs0okEulQKHQ77TpUVCcIwoxXPcGAoDM6cuTI44QQw3YRQsjHZtqHAUFZicVi22nXoBae5z840z4MCMrKyMjIE7RrUAvDMJdyHDftPgwIykosFttn4KdZDo7jGqbbgQFBWUkmk6l4PJ7TvRcLCcMwrdNtx4CgrA0PD2816nV+nU5n83TbMSAoa6IoBgCgm3YdaiCETHueOgYE5SQaje6hXYMabDZb43TbMSAoJwzDGPIC2GazuX667RgQlJNgMLiPdg0qWTDdRgwIyoksywcBIEK7DhVUCYJgn7wRA4JyIssyAYCXaNehBkLIlM9kYUBQzqLR6Mu0a1AJBgTNXTQa/SvtGtRQVlY25ZUsDAjKGSHk77RrUEN5eXnd5G0YEJSzQCAwZtCLXbsmb8CAoHwN0S5AaQzDYECQMgghw7RrUBohpHryNgwIyoskSSHaNSiNYZgpV3zHgKC8JBIJkXYNKiifvAEDgvJCCDFcBwEAu8ViYU7dgAFB+YrSLkAFjNVqZU/dgAFBeWEYxpAnTjEMU3rq1xgQlBdCyATtGtRACDntniEYEJQvQwYEADAgSBEp2gWoJH3qFxgQlBeGYVjaNaiBYZjTgo8BQXkhhJhp16AGQggGBCnCkB3EZDKddsMgDAjKC8Mws966rEDJoVAIA4IUMeVzSwYw5Vx7DAjKl4N2ASrAgCBlWCwWIwZkyklgGBCUF6vVWkG7BqURQgKTt2FAUL4E2gUozWQyYUCQMhiGqaVdg9JOnDjhn7wNA4JyxvN89XQnFxW6YDB4ZPI2DAjKRwftAlTinbwBA4JyZrfbP0C7BjUQQjAgaO7sdvtFtGtQwXg4HMZFOpobq9XKAIDhOggh5NjJC3OfBgOCcmKxWFoAwEa7DhUMTLcRA4JyYrVa30e7BjWEw2EMCJo7juPeT7sGlXim24gBQTmpqKg4l3YNapBl+dB02zEgKGsOh6OCELKUdh1qkCQJOwiaG5fLtYphGCvtOlRwQpKkA9PtwICgrFitVigrK7uRdh1qIIS8KsvytJcxwoCgrHAc1wwAhnx6FYvFXpxpHwYEZcXhcCynXYNaotHo/860DwOCslJRUbGCdg1qIIRExsbG9s60HwOCzqi2trYdAAz58i7DMK+Pj49P+YjJP2FA0Bm5XK7vT75mrVGIovjabPsxIGhWNTU1HQBwJe061JJKpfbMth8DgmZVWVn5H0b+PYlEIi/Ptt+w3ziaO4fDUWG1Wq+lXYeKXhJFcXS2AzAgaEYNDQ33Z55l0a5DLT6f75EzHYMBQdOqrq5eVlJS8nnadagoOj4+/tiZDsKAoGlVVVXdYtRXruAf73/sGRsbi53pOAwImqKhoeHDVqt1Je061BQKhZ7N5jgMCDoNx3GOysrK3xv1/h//NDY29sdsjsOAoNM0NDR8BwCctOtQ2W5RFKdc4mc6GBD0rtbW1gvLysrW0K5DbT6f795sj8WAoHc4HI5Fdrv9CSMvzE/yiKL4XLYHY0DQOxYvXrwRAKpo16G2UCi0Y7rrX82kVN1ykN6xLFvS0tLyo2QyeQXtWrQQj8d/l8vxGJAi19rauprjOMOvO+Af733sGh4e7s7lMfgUq4jxPL+K47h7aNehkRPBYPDOXB+EHaRI8Ty/QhCER2nXoRVCSNfQ0NCbuT4OA1JkrFYrOByOawVBeJB2LVoaHh7+eT6Pw4AUmYULF36trKysqMIBAEeOHz/+RD4PxIAUCZZl57W2tq7jOO6btGvRWDocDn9FluVUPg/GgBQBm81maW5ufrKkpORDtGuh4MXDhw/PeFmfM8GAGJwgCB/jeX4TADTSroWGYDD4wFwejwExKI7jLJ2dnfelUqlvAABDux4aCCG7BwcHn5nLGBgQg2FZtqSqqurfBEFYm0qlzqZdD0XhI0eOzPmMSAyIgfA8L/A8/2uGYYpxrXEaSZI2i6L49lzHwYAUOIvFAvPmzTu3vr7+KyzLfg4AzLRr0oGRo0eP/kSJgTAgBUwQhHNcLte92DFOF4lEbozH4z4lxsKAFBiWZZn6+vqbHA7HdQzDGPKGmnMxMTHxpMfjeUqp8fDDigUmmUwSANjNMEwr7Vp0KD02NpbzBxJngwEpQF6vt3toaOgTAOCnXYuOkFQq9dWBgYFpb6WWL6M/xapduxw+oeWE7iD8dfsrMKL2PIFA4C+xWKyzra1tLwA0qz2f3plMpmf279//sNLjnvYGEtkKmwHgC0pPUmQOrNsJ/75+J+zTYjKn09nU2Nj43wzDXKDFfDoVPnz48PnhcLhf6YHxKZbyFq9bDq+uvUqbziWKorevr+9CSZKe1GI+HSLRaPQaNcIBGBDVlKxbDo/23ANr6irUv0qIJEnE4/F8TpKkTQCQ16dWC1Uqldp08ODBXWqNjwFRCwO29jp4YNet8AMtpksmkzG32/11WZbv1mI+PSCE9B04cOB2NefAgKisvQ5u7tkAO1ZeANVazNff33+fz+e7LvO8XIv5KHrb6/V+VJZlWc1JMCAaaK+FT237Mjx7yWKwqT3XiRMnwO/3/2ZoaOgqAJj25vhG4PP5vhQOh4+pPQ8GRCsmWNZ1F3TffDmcr8V0gUBgt9/vPzedTr+lxXwaSiYSiS/6/f7ntZgMA6Ktxh9fC8//+U64WIvJfD5fd19f34cBoE+L+bQgSdKPenp6Nms1HwZEe7b/vwRe2LYabtJiMlmWg729vedOTEwU/CV+JEna6vF41mk5JwaEDnblebCR/AJ+soRX/2w/WZbjBw8e/CzHcRvVnkstkiQ95Xa7r08mkwkt58WA0GSFb+66HX67pFb9xXsikSB79uz5hiiKazJrebXnU5LJZHoxEAjcQGVuGpOif6mvhFW9G2DfyrPBpcV8Xq/3p7FYLLMuOeP9+fQgnU6/1N/f/5FQKDTr7ZrVggHRh7ZtN8MLa1fAe7WYrL+/v2tgYOByABjQYr58mUymP7/99tufiUQiaWo10JoYTcJA+7qrYN/aq+CjWkw3MjKyp7+/vwMAPFrMlyuWZZ/r6em5TBTFAM06MCD6UrpuBWzv+R58ra5C/X+b0tJSJwDUqD1PriRJ+t3+/fuvkSQp6xvdqAUDoj/29gZ4cNetoPptCRYtWvQzAChXe55cSJK0ye12X5NMJkXatQAGRL/a6+COng3w6MplUKnG+NXV1ZcCgG7uKkUIGZdl+Q6Px3Mz7VpOhQHRsfZaWLVtDTx9SRvMU3rsqqoqPf0ipvx+/2d6e3vvTyaTunoJGgOidwyc13U3vLny/dCp1JALFy68yGq16qV7vOHz+c71+/1Z3dhfa0Y/J90ompcotJTmOK6kqqrqlzr5t3+ut7d3pSzLUdqFzEQPPyR0Br2DcOf6P0BON5+cSVVV1bU6uMiDFAqFvuv3+3+Uyy2ZacCA6N/e99wF9yk1WE1NzbeUGitPnsHBwY8Hg0Fdvv8yGQZE39I/fgm+rdRgjY2NNwAAlSu+E0IkWZb/a2Bg4PuxWEz1yyIpBQOiZynYdMtm2K3EUNXV1Y6KioqfKjFWHkZ9Pt/yQCDwF0rz5w0DolcE3mq/G+5QajiHw/E1AChTarwsJWKx2E+PHj36n7Isj2k8tyIwIDq17gn4jtsHilyQwGazsXa7/etKjJUtQsi+oaGhq4PB4BEt51UaBkSHeofg91t2wx+UGq++vv5eAG0+Tg8AB48fP/5Dn8/3m2QyqeoVR7SAAdGfwdW/gusHQ6DIR7ydTmfLvHnztHjlSo5Go/cPDAzcI8uypmf9qQkDojPb/wbf3d0Piv2CVVdXq/2RkjFZlreGw+GNQ0NDBfHSbS4wIPry8rrH4VdKDdbU1MTbbDa1TlVNMQyzzev13hIKhQx7GwYMiF4QCK7cBKvcPlDknWWWZZnKysot6XTaosR4pxiVJOnRkZGRh0dGRox2za0pMCA6sf01uH/HazCk1HiVlZWXptNpxT6QSAiJxWKxTaOjoz8YHR0NKTWu3mFA9IDAGz9+CX6u5JDz589XZO3BMMwroij+TyAQ2BGPx4eVGLOQYEDok9c9Bp98tRvGlRqQ5/kLzGbznO5PYjKZth07dmx9IBBwK1VXIcKAULb3EPxw/VPKXV2EZVmrIAj5XJozE9DdwWDwqXg8/qQoioZdeOcCA0JX4MbNcK+SAzY1NV0NAEtyeEhfJBJ5eHR0dGsoFCqatUW2MCD0SOsehxVuH8SVGpDjOJPdbl9DyKwvhAUlSdozPj7eNTY21hWPx3smJiZ0fU4GTRgQSnqH4Jfrn4C9So65YMGCGwghS6fZNShJ0k5RFH8fDof3SpJE7UJshQYDQsfw+p2wQckBy8rKqu12e+bpWoAQ8pYoim8kEon94+Pj+8Ph8CEl5yomGBAKutxw3fa/waCSY7Isy/r9/mU+n0/XlxMtNBgQbUnHRuGRS++F55QeOBwOD4XDRr8tofYwIMqTAEAGAiIwEAQC3i439Hb1w96ufvjL7r7iuk1zofu/AAAA//8EUXdCEVVrlQAAAABJRU5ErkJggg=="
             alt="datalad_d" height="15em" class="mb-1"/>
             Download with DataLad</b-button>&nbsp;</span>
           <span v-show="displayData.is_github"><b-button variant="outline-dark" size="sm" @click="gotoURL(displayData.url)"><i class="fab fa-github"></i> View on GitHub</b-button>&nbsp;</span>
           <span v-show="displayData.is_gin"><b-button variant="outline-dark" size="sm" @click="gotoURL(displayData.url)"><img src="artwork/ginfavicon.png" style="height: 1em;"></img> View on GIN</b-button>&nbsp;</span>
           <span v-show="selectedDataset.doi"><b-button variant="outline-dark" size="sm" v-b-modal.modal-2 @click="getCitationText(selectedDataset.doi)"><i class="fas fa-quote-right"></i> Cite</b-button>&nbsp;</span>
-          <span v-if="displayData.show_export"><b-button variant="outline-dark" size="sm" :href="displayData.file_path" :download="displayData.download_filename"><i class="fas fa-share"></i> Export metadata</b-button>&nbsp;</span>
+          <b-button variant="outline-dark" size="sm" :href="displayData.file_path" :download="displayData.download_filename"><i class="fas fa-share"></i> Export metadata</b-button>&nbsp;
           <span v-show="displayData.is_github"><b-button variant="outline-dark" size="sm" @click="openWithBinder(displayData.url)"><img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAFkAAABZCAMAAABi1XidAAAB8lBMVEX///9XmsrmZYH1olJXmsr1olJXmsrmZYH1olJXmsr1olJXmsrmZYH1olL1olJXmsr1olJXmsrmZYH1olL1olJXmsrmZYH1olJXmsr1olL1olJXmsrmZYH1olL1olJXmsrmZYH1olL1olL0nFf1olJXmsrmZYH1olJXmsq8dZb1olJXmsrmZYH1olJXmspXmspXmsr1olL1olJXmsrmZYH1olJXmsr1olL1olJXmsrmZYH1olL1olLeaIVXmsrmZYH1olL1olL1olJXmsrmZYH1olLna31Xmsr1olJXmsr1olJXmsrmZYH1olLqoVr1olJXmsr1olJXmsrmZYH1olL1olKkfaPobXvviGabgadXmsqThKuofKHmZ4Dobnr1olJXmsr1olJXmspXmsr1olJXmsrfZ4TuhWn1olL1olJXmsqBi7X1olJXmspZmslbmMhbmsdemsVfl8ZgmsNim8Jpk8F0m7R4m7F5nLB6jbh7jbiDirOEibOGnKaMhq+PnaCVg6qWg6qegKaff6WhnpKofKGtnomxeZy3noG6dZi+n3vCcpPDcpPGn3bLb4/Mb47UbIrVa4rYoGjdaIbeaIXhoWHmZYHobXvpcHjqdHXreHLroVrsfG/uhGnuh2bwj2Hxk17yl1vzmljzm1j0nlX1olL3AJXWAAAAbXRSTlMAEBAQHx8gICAuLjAwMDw9PUBAQEpQUFBXV1hgYGBkcHBwcXl8gICAgoiIkJCQlJicnJ2goKCmqK+wsLC4usDAwMjP0NDQ1NbW3Nzg4ODi5+3v8PDw8/T09PX29vb39/f5+fr7+/z8/Pz9/v7+zczCxgAABC5JREFUeAHN1ul3k0UUBvCb1CTVpmpaitAGSLSpSuKCLWpbTKNJFGlcSMAFF63iUmRccNG6gLbuxkXU66JAUef/9LSpmXnyLr3T5AO/rzl5zj137p136BISy44fKJXuGN/d19PUfYeO67Znqtf2KH33Id1psXoFdW30sPZ1sMvs2D060AHqws4FHeJojLZqnw53cmfvg+XR8mC0OEjuxrXEkX5ydeVJLVIlV0e10PXk5k7dYeHu7Cj1j+49uKg7uLU61tGLw1lq27ugQYlclHC4bgv7VQ+TAyj5Zc/UjsPvs1sd5cWryWObtvWT2EPa4rtnWW3JkpjggEpbOsPr7F7EyNewtpBIslA7p43HCsnwooXTEc3UmPmCNn5lrqTJxy6nRmcavGZVt/3Da2pD5NHvsOHJCrdc1G2r3DITpU7yic7w/7Rxnjc0kt5GC4djiv2Sz3Fb2iEZg41/ddsFDoyuYrIkmFehz0HR2thPgQqMyQYb2OtB0WxsZ3BeG3+wpRb1vzl2UYBog8FfGhttFKjtAclnZYrRo9ryG9uG/FZQU4AEg8ZE9LjGMzTmqKXPLnlWVnIlQQTvxJf8ip7VgjZjyVPrjw1te5otM7RmP7xm+sK2Gv9I8Gi++BRbEkR9EBw8zRUcKxwp73xkaLiqQb+kGduJTNHG72zcW9LoJgqQxpP3/Tj//c3yB0tqzaml05/+orHLksVO+95kX7/7qgJvnjlrfr2Ggsyx0eoy9uPzN5SPd86aXggOsEKW2Prz7du3VID3/tzs/sSRs2w7ovVHKtjrX2pd7ZMlTxAYfBAL9jiDwfLkq55Tm7ifhMlTGPyCAs7RFRhn47JnlcB9RM5T97ASuZXIcVNuUDIndpDbdsfrqsOppeXl5Y+XVKdjFCTh+zGaVuj0d9zy05PPK3QzBamxdwtTCrzyg/2Rvf2EstUjordGwa/kx9mSJLr8mLLtCW8HHGJc2R5hS219IiF6PnTusOqcMl57gm0Z8kanKMAQg0qSyuZfn7zItsbGyO9QlnxY0eCuD1XL2ys/MsrQhltE7Ug0uFOzufJFE2PxBo/YAx8XPPdDwWN0MrDRYIZF0mSMKCNHgaIVFoBbNoLJ7tEQDKxGF0kcLQimojCZopv0OkNOyWCCg9XMVAi7ARJzQdM2QUh0gmBozjc3Skg6dSBRqDGYSUOu66Zg+I2fNZs/M3/f/Grl/XnyF1Gw3VKCez0PN5IUfFLqvgUN4C0qNqYs5YhPL+aVZYDE4IpUk57oSFnJm4FyCqqOE0jhY2SMyLFoo56zyo6becOS5UVDdj7Vih0zp+tcMhwRpBeLyqtIjlJKAIZSbI8SGSF3k0pA3mR5tHuwPFoa7N7reoq2bqCsAk1HqCu5uvI1n6JuRXI+S1Mco54YmYTwcn6Aeic+kssXi8XpXC4V3t7/ADuTNKaQJdScAAAAAElFTkSuQmCC"
             alt="binder_logo" height="16em" class="mb-1">Explore with Binder</b-button></span>
-          <span style="float: right;">
-            <span v-show="selectedDataset.access_request_contact"><b-button variant="outline-dark" size="sm" :href="displayData.access_request_mailto"><i class="far fa-envelope"></i> Request access</b-button>&nbsp;</span>
-            <span v-show="selectedDataset.access_request_url"><b-button variant="outline-dark" size="sm" @click="gotoURL(selectedDataset.access_request_url)"><i class="fas fa-share"></i> Request access</b-button></span>
-          </span>
-          
           <b-modal id="modal-1" size="lg" 
           header-bg-variant="light"
           footer-bg-variant="light"
           body-bg-variant="light"
           body-text-variant="dark"
           ok-only>
             <template #modal-header="{ close }">
@@ -106,15 +101,14 @@
                   </b-tooltip>
                 </b-col>
               </b-row>
             </div>
             <span v-show="invalid_doi"><em>Invalid DOI</em></span>
           </b-modal>
         </div>
-        <!-- -->
         <hr>
         <!-- DATASET DESCRIPTION, KEYWORDS, PROPERTIES -->
         <b-row no-gutters>
           <b-col md="9" style="text-align: justify;">
             <b-card-text>
               <strong>Description:</strong>
               <span v-if="displayData.description && Array.isArray(displayData.description) && displayData.description.length>0 ">
@@ -125,70 +119,64 @@
             </b-card-text>
           </b-col>
           <b-col md="3">
             <b-card-text>
               <strong>Keywords:</strong> <br>
               <b-button pill disabled size="sm" variant="outline-dark" v-for="keyword in selectedDataset.keywords">{{keyword}}</b-button>
             </b-card-text>
-
-            <b-card-text>
-              <strong>Properties:</strong> <br>
-              <span v-if="selectedDataset.subdatasets_available_count"><b-button disabled size="sm" variant="outline-dark">Subdatasets: {{selectedDataset.subdatasets_available_count}}</b-button>&nbsp;</span>
-              <span v-if="selectedDataset.top_display && selectedDataset.top_display.length">
-                <span v-for="display_property in selectedDataset.top_display" v-if="display_property.value"><b-button disabled size="sm" variant="outline-dark">{{display_property.name}}: {{display_property.value}}</b-button>&nbsp;</span>
-              </span>
-            </b-card-text>
+            <span v-if="selectedDataset.top_display && selectedDataset.top_display.length">
+              <b-card-text>
+                <strong>Properties:</strong> <br>
+                <span v-for="display_property in selectedDataset.top_display"><b-button disabled size="sm" variant="outline-dark">{{display_property.name}}: {{display_property.value}}</b-button>&nbsp;</span>
+              </b-card-text>
+            </span>
           </b-col>
         </b-row>
       </b-card-body>
       <!-- BOTTOM SECTION WITH TABS-->
       <b-card-body>
-        <b-tabs card content-class="mt-3" fill active-nav-item-class="font-weight-bold" v-model="tabIndex" @activate-tab="newTabActivated" ref="alltabs">
+        <b-tabs card content-class="mt-3" fill active-nav-item-class="font-weight-bold" v-model="tabIndex">
           <!-- SUBDATASETS -->
-          <b-tab key="subdatasets" ref="tabelement">
+          <b-tab>
             <template v-slot:title>
-              <i class="fas fa-list-ol"></i> Subdatasets <span v-if="subdatasets_ready">({{selectedDataset.subdatasets_available_count}})</span>
+              <i class="fas fa-list-ol"></i> Subdatasets
             </template>
-            <span v-if="!subdatasets_ready">
-              <div class="d-flex justify-content-center mb-3">
-                <b-spinner label="Loading..."></b-spinner>
-              </div>
-            </span>
-            <span v-else>
-              <span v-if="!subdatasets || !subdatasets.length"><em>There are no subdatasets listed for the current dataset</em></span>
+            <span v-if="subdatasets_ready">
+              <span v-if="!sortedSubdatasets || !sortedSubdatasets.length"><em>There are no subdatasets listed for the current dataset</em></span>
               <span v-else>
                 <b-form>
                   <b-row>
                     <b-col md="7">
                       <b-input-group>
                       <b-button-group>
                         <b-button pill variant="outline-dark" @click="sortByName">
                           <span v-if="sort_name"><i class="fas fa-sort-amount-down-alt"></i></span>
                           <span v-else><i class="fas fa-sort-amount-up-alt"></i></span>
                           Name
                         </b-button>&nbsp;
                         <b-button pill variant="outline-dark" @click="sortByModified">
                           <span v-if="sort_modified"><i class="fas fa-sort-amount-down-alt"></i></span>
                           <span v-else><i class="fas fa-sort-amount-up-alt"></i></span>
-                          Modified
+                          Modifed
                         </b-button>
                       </b-button-group>&nbsp;&nbsp;
-                      <b-form-input id="input-1" type="search" placeholder="Filter by dataset or author name" required v-model="search_text" ref="text_search_input"></b-form-input>
+                      <b-form-input id="input-1" type="search" placeholder="Search by dataset or author name" required v-model="search_text" ref="text_search_input"></b-form-input>
                     </b-input-group>
+                    
                     </b-col>
                     <b-col md="5">
                       <b-input-group>
                         <b-form-tags v-model="search_tags" :tag-validator="validator" no-outer-focus class="border-0 p-0">
                           <template v-slot="{ tags, inputAttrs, inputHandlers, tagVariant, addTag, removeTag}">
                             <b-input-group class="mb-1">
                               <b-form-input
                                 v-bind="inputAttrs"
                                 v-model="tag_text"
                                 v-on="inputHandlers"
-                                placeholder="Filter by keyword (select or press enter to add)"
+                                placeholder="Search by keyword (select or press enter to add)"
                                 class="form-control"
                                 ref="tag_search_input"
                                 @input="inputTagText()"
                                 v-on:keyup.enter="clearSearchTagText()"
                               ></b-form-input>
                             </b-input-group>
                             <div class="d-inline-block" style="font-size: 1.5rem;">
@@ -213,24 +201,24 @@
                 <b-card v-for="ds in sortedSubdatasets" border-variant="dark" header-bg-variant="transparent" no-body class="mb-2 pt-1">
                   <template v-slot:header>
                     <b-row no-gutters>
                       <b-col align-h="center" align-v="center" md="1">
                         <span class="xxlfont"><i class="fas fa-database"></i></span>
                       </b-col>
                       <b-col class="text-muted" md="7">
-                        <h5><a @click="selectDataset($event, ds)" class="newlink">{{ds.dirs_from_path.at(-1)}}</a></h5>
+                        <h5><a @click="selectDataset(ds)" class="newlink">{{ds.dirs_from_path.at(-1)}}</a></h5>
                         <span v-for="(author, index) in ds.authors">
                           <small>
                             <span v-if="author.givenName">{{author.givenName}} {{author.familyName}}</span><span v-else>{{author.name}}</span><span v-if="index != ds.authors.length - 1">, </span>
                           </small>
                         </span>
                         <b-card-text>
                           <small>
                             <strong>Version:</strong> {{ds.dataset_version.substring(0,7)}}&nbsp;
-                            <strong>Modified:</strong> {{getDateFromUTCseconds(ds.source_time)}}&nbsp;
+                            <strong>Modified:</strong> {{getDateFromUTCseconds(ds.extraction_time)}}&nbsp;
                           </small>
                         </b-card-text>
                       </b-col>
                       <b-col md="4">
                         <b-card-text>
                           <span v-for="keyword in ds.keywords"><b-button pill size="sm" class="p-1" variant="outline-dark" @click="addSearchTag(keyword)">{{keyword}}</b-button>&nbsp;</span>
                         </b-card-text>
@@ -238,51 +226,51 @@
                     </b-row>
                   </template>
                 </b-card>
               </span>
             </span>
           </b-tab>
           <!-- FILE TREE -->
-          <b-tab @click="getFiles" key="content" ref="tabelement">
+          <b-tab @click="getFiles">
             <template v-slot:title>
-              <i class="far fa-folder"></i> Content
+              <i class="far fa-folder"></i> Files
             </template>
-            <span v-if="files_ready">
-              <span v-if="!selectedDataset.tree || !selectedDataset.tree.length"><em>There is no content available for the current dataset</em></span>
-              <span v-else>
-                <b-card no-body class="p-2">
+            <span v-if="!selectedDataset.tree || !selectedDataset.tree.length"><em>There are no files listed for the current dataset</em></span>
+            <span v-else>
+              <b-card no-body class="p-2">
+                <span v-if="files_ready">
                   <ul>
                     <tree-item class="item" v-for="item in selectedDataset.tree" :item="item"></tree-item>
                   </ul>
-                </b-card>
-              </span>
-              <b-modal id="modal-3" size="md"
-              header-bg-variant="light"
-              footer-bg-variant="light"
-              body-bg-variant="light"
-              body-text-variant="dark"
-              ok-only
-              >
-                <template #modal-header="{ close }">
-                  <div class="d-block text-center">
-                    <h3>Dataset not found</h3>
-                    <p class="my-4">The selected dataset is currently not available in the catalog.</p>
+                </span>
+                <span v-else>
+                  <div class="d-flex justify-content-center mb-3">
+                    <b-spinner label="Loading..."></b-spinner>
                   </div>
-                </template>
-              </b-modal>
-            </span>
-            <span v-else>
-              <div class="d-flex justify-content-center mb-3">
-                <b-spinner label="Loading..."></b-spinner>
-              </div>
+                </span>
+              </b-card>
             </span>
+            <b-modal id="modal-3" size="md"
+            header-bg-variant="light"
+            footer-bg-variant="light"
+            body-bg-variant="light"
+            body-text-variant="dark"
+            ok-only
+            >
+              <template #modal-header="{ close }">
+                <div class="d-block text-center">
+                  <h3>Dataset not found</h3>
+                  <p class="my-4">The selected dataset is currently not available in the catalog.</p>
+                </div>
+              </template>
+            </b-modal>
           </b-tab>
           <!-- PUBLICATIONS -->
           <span v-if="selectedDataset.publications && selectedDataset.publications.length">
-            <b-tab key="publications" ref="tabelement">
+            <b-tab>
               <template v-slot:title>
                 <i class="fas fa-book"></i> Publications
               </template>
               <span v-if="!selectedDataset.publications || !selectedDataset.publications.length"><em>There are no publications listed for the current dataset</em></span>
               <span v-else v-for="pub in selectedDataset.publications">
                 <b-card border-variant="dark" header-bg-variant="transparent" no-body class="mb-2">
                   <template v-slot:header>
@@ -307,17 +295,17 @@
                   </template>
                 </b-card>
               </span>
             </b-tab>
           </span>
           <!-- FUNDING -->
           <span v-if="selectedDataset.funding && selectedDataset.funding.length">
-            <b-tab key="funding" ref="tabelement">
+            <b-tab>
               <template v-slot:title>
-                <i class="fas fa-building-columns"></i> Funding
+                <i class="fas fa-dollar-sign"></i> Funding
               </template>
               <span v-if="!selectedDataset.funding || !selectedDataset.funding.length"><em>There are no funding sources listed for the current dataset</em></span>
               <span v-else v-for="fund in selectedDataset.funding">
                 <b-card border-variant="dark" header-bg-variant="transparent" no-body class="mb-2">
                   <template v-slot:header>
                     <b-row no-gutters>
                       <b-col align-h="center" align-v="center" md="1">
@@ -332,15 +320,15 @@
                   </template>
                 </b-card>
               </span>
             </b-tab>
           </span>
           <!-- PROVENANCE -->
           <span v-if="selectedDataset.provenance && selectedDataset.provenance.length">
-            <b-tab key="provenance" ref="tabelement">
+            <b-tab>
               <template v-slot:title>
                 <i class="fas fa-laptop-code"></i> Provenance
               </template>
               <span v-if="!selectedDataset.provenance || !selectedDataset.provenance.length"><em>There are no provenance records listed for the current dataset</em></span>
               <span v-else v-for="record in selectedDataset.provenance">
                 <b-container>
                   <b-row>
@@ -348,15 +336,15 @@
                       <b-card header-bg-variant="transparent" >
                         <template v-slot:header>
                           <b-row no-gutters>
                             <b-col align-h="center" align-v="center" md="3">
                               <span class="lfont"><i class="fas fa-database"></i></span>
                             </b-col>
                             <b-col align-h="center" align-v="center" md="9">
-                              <span><a @click="selectDataset($event, null, selectedDataset.dataset_id, record.previous_version)" class="newlink"><span class="lfont">Dataset:  <em>before</em></span></a></span>
+                              <span><a @click="selectDataset(null, selectedDataset.dataset_id, record.previous_version)" class="newlink"><span class="lfont">Dataset:  <em>before</em></span></a></span>
                             </b-col>
                           </b-row>
                         </template>
                         <b-card-text class="text-muted">
                           <small>
                             <strong>ID: </strong>{{selectedDataset.dataset_id.slice(0,7)}}...<br>
                             <strong>Version: </strong>{{record.previous_version.slice(0,7)}}...<br>
@@ -417,15 +405,15 @@
                       <b-card header-bg-variant="transparent" >
                         <template v-slot:header>
                           <b-row no-gutters>
                             <b-col align-h="center" align-v="center" md="3">
                               <span class="lfont"><i class="fas fa-database"></i></span>
                             </b-col>
                             <b-col align-h="center" align-v="center" md="9">
-                              <span><a @click="selectDataset($event, null, selectedDataset.dataset_id, record.dataset_version)" class="newlink"><span class="lfont">Dataset:  <em>after</em></span></a></span>
+                              <span><a @click="selectDataset(null, selectedDataset.dataset_id, record.dataset_version)" class="newlink"><span class="lfont">Dataset:  <em>after</em></span></a></span>
                             </b-col>
                           </b-row>
                         </template>
                         <b-card-text class="text-muted">
                               <small>
                                 <strong>ID: </strong>{{selectedDataset.dataset_id.slice(0,7)}}...<br>
                                 <strong>Version: </strong>{{record.dataset_version.slice(0,7)}}...<br>
@@ -444,15 +432,15 @@
                 <hr class="mb-5 pb-1">
               </span>
             </b-tab>
           </span>
           <!-- EXTRA TABS -->
           <span v-if="selectedDataset.additional_display && selectedDataset.additional_display.length">
             <span v-for="new_tab in selectedDataset.additional_display">
-              <b-tab :key="new_tab.name" ref="tabelement">
+              <b-tab>
                 <template v-slot:title>
                   <span v-if="new_tab.icon"><i :class="new_tab.icon"></i></span><span v-else><i class="fas fa-bars"></i></span> {{new_tab.name}}
                 </template>
                 <span v-if="!new_tab.content"><em>No available content for this display option</em></span>
                 <span v-else>
                   <table class="table table-striped">
                     <thead>
```

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/catalog.py` & `datalad_catalog-0.2.2/datalad_catalog/catalog.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 )
 from datalad.distribution.dataset import datasetmethod
 from datalad.interface.base import (
     Interface,
     build_doc,
 )
 from datalad.interface.results import get_status_dict
-from datalad.interface.base import eval_results
+from datalad.interface.utils import eval_results
 from datalad.log import log_progress
 from datalad.support.constraints import EnsureChoice
 from datalad.support.exceptions import InsufficientArgumentsError
 from datalad.support.param import Parameter
 from jsonschema import (
     Draft202012Validator,
     RefResolver,
@@ -30,18 +30,14 @@
 
 from datalad_catalog.meta_item import MetaItem
 from datalad_catalog.utils import read_json_file
 from datalad_catalog.webcatalog import (
     Node,
     WebCatalog,
 )
-from datalad_catalog.translate import (
-    Translate,
-    get_translators,
-)
 
 # Create named logger
 lgr = logging.getLogger("datalad.catalog.catalog")
 
 
 # Decoration auto-generates standard help
 @build_doc
@@ -159,109 +155,107 @@
                 "subdataset_path='path/to/subdataset')"
             ),
             code_cmd=(
                 "datalad catalog workflow-update -c /tmp/my-cat "
                 "-d 'path/to/superdataset' -s 'path/to/subdataset'"
             ),
         ),
-        dict(
-            text=(
-                "Translate a metadata item from a particular source structure "
-                "into the catalog schema. A dedicated translator should be "
-                "provided and exposed as an entry point (e.g. via a DataLad "
-                "extension) as part of the 'datalad.metadata.translators' group."
-            ),
-            code_py=("catalog('translate', metadata='path/to/metadata.jsonl')"),
-            code_cmd=("datalad catalog translate -m path/to/metadata.jsonl"),
-        ),
     ]
 
     # parameters of the command, must be exhaustive
     _params_ = dict(
         # name of the parameter, must match argument name
         catalog_action=Parameter(
             args=("catalog_action",),
             # documentation
             doc="""This is the subcommand to be executed by datalad-catalog.
             Options include: create, add, remove, serve, set-super, validate,
-            workflow-new, and workflow-update.""",
+            workflow-new, and workflow-update.
+            Example: ''""",
             # type checkers, constraint definition is automatically
             # added to the docstring
             constraints=EnsureChoice(
                 "create",
                 "add",
                 "remove",
                 "serve",
                 "set-super",
                 "validate",
                 "workflow-new",
                 "workflow-update",
-                "translate",
             ),
         ),
         catalog_dir=Parameter(
             # cmdline argument definitions, incl aliases
             args=("-c", "--catalog_dir"),
             # documentation
-            doc="""Directory where the catalog is located or will be created.""",
+            doc="""Directory where the catalog is located or will be created.
+            Example: ''""",
         ),
         metadata=Parameter(
             # cmdline argument definitions, incl aliases
             args=("-m", "--metadata"),
             # documentation
             doc="""Path to input metadata. Multiple input types are possible:
             - A '.json' file containing an array of JSON objects related to a
              single datalad dataset.
-            - A stream of JSON objects/lines""",
+            - A stream of JSON objects/lines
+            Example: ''""",
         ),
         dataset_id=Parameter(
             # cmdline argument definitions, incl aliases
             args=("-i", "--dataset_id"),
             # documentation
-            doc="""""",
+            doc="""
+            Example: ''""",
         ),
         dataset_version=Parameter(
             # cmdline argument definitions, incl aliases
             args=("-v", "--dataset_version"),
             # documentation
-            doc="""""",
+            doc="""
+            Example: ''""",
         ),
         force=Parameter(
             # cmdline argument definitions, incl aliases
             args=("-f", "--force"),
             # documentation
             doc="""If content for the user interface already exists in the catalog
             directory, force this content to be overwritten. Content
             overwritten with this flag include the 'artwork' and 'assets'
             directories and the 'index.html' and 'config.json' files. Content in
-            the 'metadata' directory remain untouched.""",
+            the 'metadata' directory remain untouched.
+            Example: ''""",
             action="store_true",
             default=False,
         ),
         config_file=Parameter(
             # cmdline argument definitions, incl aliases
             args=("-y", "--config-file"),
             # documentation
             doc="""Path to config file in YAML or JSON format. Default config is read
-            from datalad_catalog/config/config.json""",
+            from datalad_catalog/config/config.json
+            Example: ''""",
         ),
         dataset_path=Parameter(
             # cmdline argument definitions, incl aliases
             args=("-d", "--dataset-path"),
             # documentation
             doc="""Path to dataset on which to run an extraction, translation
-            and catalog generation workflow.""",
+            and catalog generation workflow.
+            Example: ''""",
         ),
         subdataset_path=Parameter(
             # cmdline argument definitions, incl aliases
             args=("-s", "--subdataset-path"),
             # documentation
             doc="""Path to dataset on which to run an extraction, translation
             and catalog generation workflow. Used together with '-d',
-            '--dataset-path' when running 'workflow-update'.""",
+            '--dataset-path' when running 'workflow-update'.
+            Example: ''""",
         ),
     )
 
     @staticmethod
     # decorator binds the command to the Dataset class as a method
     @datasetmethod(name="catalog")
     # generic handling of command results (logging, rendering, filtering, ...)
@@ -306,33 +300,31 @@
             "validate",
             "serve",
             "add",
             "remove",
             "set-super",
             "workflow-new",
             "workflow-update",
-            "translate",
         ]
         if catalog_action not in CALL_ACTION:
             raise ValueError(
                 "Unknown subcommand %s, choose from %s"
                 % (catalog_action, ", ".join(c for c in CALL_ACTION))
             )
 
+        # TODO: check if schema is valid (move to tests)
+        # Draft202012Validator.check_schema(schema)
+
         # set common result kwargs:
         action = "catalog_%s" % catalog_action
         res_kwargs = dict(action=action)
         # If action is validate, only metadata required
         if catalog_action == "validate":
             yield from _validate_metadata(metadata)
             return
-        # If action is translate, only metadata required
-        if catalog_action == "translate":
-            yield from _translate_metadata(metadata)
-            return
 
         # Error out if `catalog_dir` argument was not supplied
         if catalog_dir is None:
             yield dict(
                 **res_kwargs,
                 status="impossible",
                 message=(
@@ -343,37 +335,33 @@
                 path=None,
             )
             return
         # now that we have a path, update result kwargs with it
         res_kwargs["path"] = catalog_dir
 
         # Instantiate WebCatalog class
-        ctlg = WebCatalog(
-            catalog_dir,
-            dataset_id,
-            dataset_version,
-            config_file,
-            catalog_action,
-        )
+        ctlg = WebCatalog(catalog_dir, dataset_id, dataset_version, config_file)
+        # catalog_path = Path(catalog_dir)
+        # catalog_exists = catalog_path.exists() and catalog_path.is_dir()
 
-        # Handle case where a non-catalog directory already exists at path
+        # Hanlde case where a non-catalog directory already exists at path
         # argument. Should prevent overwriting
         if ctlg.path_exists() and not ctlg.is_created():
             yield dict(
                 **res_kwargs,
                 status="error",
                 message=(
                     "A non-catalog directory already exists at %s. "
                     "Please supply a different path.",
                     catalog_dir,
                 ),
             )
             return
 
-        # Catalog should exist for all actions except create and workflow-[run|update]
+        # Catalog should exist for all actions except create and run-workflow
         # (for create action: unless force flag supplied)
         if not ctlg.is_created():
             if (
                 catalog_action != "create"
                 and catalog_action != "workflow-new"
                 and catalog_action != "workflow-update"
             ):
@@ -479,15 +467,15 @@
     else:
         if force:
             catalog.create(force)
             msg = (
                 "Catalog assets successfully overwritten at: %s",
                 catalog.location,
             )
-    # Yield created/overwritten status message
+    # Yield created/overwitten status message
     yield get_status_dict(**res_kwargs, status="ok", message=msg)
     # If metadata was also supplied, add this to the catalog
     if metadata is not None:
         yield from _add_to_catalog(catalog, metadata, res_kwargs)
 
 
 def _add_to_catalog(
@@ -519,23 +507,23 @@
             message=(
                 "No metadata supplied: Datalad catalog has to be supplied with "
                 "metadata in the form of a path to a file containing a JSON "
                 "array, or JSON lines stream, using the argument: "
                 "-m, --metadata."
             ),
         )
-    # PROCESS DESCRIPTION FOR "add" ACTION:
+    # We need to do the following:
     # 1. Establish input type (file-with-json-lines, command line stdout / stream)
     #    - for now: assume file-with-json-lines (e.g. data exported by `datalad meta-dump`
     #      and all exported objects written to file)
-    # 2. Read lines into python dictionaries. For each line:
-    #    - Validate the dictionary against the catalog schema
-    #    - Instantiate the MetaItem class, which handles translation of a json line into
-    #      the Node instances that populate the catalog
-    #    - For the MetaItem instance, write all related Node instances to file
+    # 2. Read line into python dictionary
+    # 3. Validate the dictionary against the catalog schema
+    # 4. Instantiate the MetaItem class, which handles translation of a json line into
+    #    the catalog metadata (Node instances)
+    # 5. Per MetaItem instance, write all related Node instances to file
     with open(metadata) as file:
         i = 0
         for line in file:
             i += 1
             meta_dict = json.loads(line.rstrip())
             # Check if item/line is a dict
             if not isinstance(meta_dict, dict):
@@ -704,16 +692,17 @@
             "metadata in the form of a path to a file containing a JSON array, "
             "or JSON lines stream, using the argument: -m, --metadata."
         )
         raise InsufficientArgumentsError(err_msg)
 
     # Setup schema parameters
     package_path = Path(__file__).resolve().parent
+    config_dir = package_path / "config"
     schema_dir = package_path / "schema"
-    schemas = ["catalog", "dataset", "file", "authors", "metadata_sources"]
+    schemas = ["catalog", "dataset", "file", "authors", "extractors"]
     schema_store = {}
     for s in schemas:
         schema_path = schema_dir / str("jsonschema_" + s + ".json")
         schema = read_json_file(schema_path)
         schema_store[schema["$id"]] = schema
 
     # Access the schema against which incoming metadata items will be validated
@@ -817,78 +806,7 @@
             catalog=catalog,
         )
 
 
 def _get_line_count(file: str) -> int:
     """A helper function to get a file line count"""
     return sum(1 for _ in open(file))
-
-
-def _translate_metadata(metadata: str):
-    """Translate a metadata item from a particular source structure
-    into the catalog schema.
-
-    A dedicated translator should be provided and exposed as an entry
-    point (e.g. via a DataLad extension) as part of the
-    'datalad.metadata.translators' group."
-
-    Parameters
-    ----------
-    metadata : path-like object
-        metadata to be translated
-
-    Yields
-    ------
-    status_dict : dict
-        DataLad result record
-    """
-    # First check metadata was supplied via -m flag
-    if metadata is None:
-        err_msg = (
-            "No metadata supplied: datalad catalog has to be supplied with "
-            "metadata in the form of a path to a file containing a JSON array, "
-            "or JSON lines stream, using the argument: -m, --metadata."
-        )
-        raise InsufficientArgumentsError(err_msg)
-    # Get available translators
-    translators = get_translators()
-    # Open metadata file and translate line by line
-    num_lines = _get_line_count(metadata)
-    with open(metadata) as file:
-        i = 0
-        prog_id = "catalogtranslate"
-        log_progress(
-            lgr.info,
-            prog_id,
-            "Translating metadata",
-            unit=" Lines",
-            label="Translating",
-            total=num_lines,
-        )
-        for line in file:
-            i += 1
-            log_progress(
-                lgr.info,
-                prog_id,
-                "Translating metadata",
-                update=i,
-                noninteractive_level=logging.DEBUG,
-            )
-            meta_dict = json.loads(line.rstrip())
-            # Check if item/line is a dict
-            if not isinstance(meta_dict, dict):
-                err_msg = (
-                    "Metadata item not of type dict: metadata items should be "
-                    "passed to datalad catalog as JSON objects adhering to the "
-                    "catalog schema."
-                )
-                lgr.warning(err_msg)
-            # Translate dict
-            translated_meta = Translate(meta_dict, translators).run_translator()
-            yield get_status_dict(
-                action="catalog_translate",
-                path=Path(metadata),
-                status="ok",
-                message=("Metadata successfully translated"),
-                translated_metadata=translated_meta,
-            )
-        log_progress(lgr.info, prog_id, "Translation completed")
```

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/config/config.json` & `datalad_catalog-0.2.2/datalad_catalog/schema/_metaladcore2catalog_dataset.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Differences: {'replace': "OrderedDict([('variables', OrderedDict([('metadata', '.'), ('extracted', "*

 * *            '\'.extracted_metadata\'), (\'graph\', \'.extracted_metadata["@graph"]?\')])), '*

 * *            "('properties', [OrderedDict([('name', 'type'), ('program', '.type'), ('input', "*

 * *            "'metadata')]), OrderedDict([('name', 'dataset_id'), ('program', '.dataset_id'), "*

 * *            "('input', 'metadata')]), OrderedDict([('name', 'dataset_version'), ('program', "*

 * *            "'.dataset_version'), ('input', 'met […]*

```diff
@@ -1,83 +1,89 @@
 {
-    "catalog_name": "DataCat",
-    "dataset_options": {
-        "include_metadata_export": true
-    },
-    "link_color": "#fba304",
-    "link_hover_color": "#af7714",
-    "logo_path": "",
-    "property_sources": {
-        "dataset": {
-            "additional_display": {
-                "rule": "merge",
-                "source": "any"
-            },
-            "authors": {
-                "rule": "merge",
-                "source": "any"
-            },
-            "children": {
-                "rule": "merge",
-                "source": "any"
-            },
-            "dataset_id": {
-                "rule": "single",
-                "source": "metalad_core"
-            },
-            "dataset_version": {
-                "rule": "single",
-                "source": "metalad_core"
-            },
-            "description": {
-                "rule": "priority",
-                "source": [
-                    "catalog_readme",
-                    "metalad_studyminimeta",
-                    "datacite_gin",
-                    "bids_dataset"
-                ]
-            },
-            "doi": {},
-            "funding": {
-                "rule": "merge",
-                "source": "any"
-            },
-            "keywords": {
-                "rule": "merge",
-                "source": "any"
-            },
-            "license": {},
-            "name": {
-                "rule": "single",
-                "source": "metalad_studyminimeta"
-            },
-            "publications": {
-                "rule": "merge",
-                "source": "any"
-            },
-            "short_name": {},
-            "subdatasets": {
-                "rule": "merge",
-                "source": "any"
-            },
-            "top_display": {
-                "rule": "merge",
-                "source": "any"
-            },
-            "type": {
-                "rule": "single",
-                "source": "metalad_core"
-            },
-            "url": {
-                "rule": "merge",
-                "source": "any"
-            }
+    "properties": [
+        {
+            "input": "metadata",
+            "name": "type",
+            "program": ".type"
+        },
+        {
+            "input": "metadata",
+            "name": "dataset_id",
+            "program": ".dataset_id"
+        },
+        {
+            "input": "metadata",
+            "name": "dataset_version",
+            "program": ".dataset_version"
+        },
+        {
+            "input": "",
+            "name": "name",
+            "program": null
+        },
+        {
+            "input": "",
+            "name": "short_name",
+            "program": null
+        },
+        {
+            "input": "",
+            "name": "description",
+            "program": null
+        },
+        {
+            "input": "",
+            "name": "doi",
+            "program": null
+        },
+        {
+            "input": "graph",
+            "name": "url",
+            "program": ".[]? | select(.[\"@type\"] == \"Dataset\") | [.distribution[]? | select(has(\"url\")) | .url]"
+        },
+        {
+            "input": {},
+            "name": "license",
+            "program": null
+        },
+        {
+            "input": "graph",
+            "name": "authors",
+            "program": "[.[]? | select(.[\"@type\"]==\"agent\")] | map(del(.[\"@id\"], .[\"@type\"]))"
+        },
+        {
+            "input": [],
+            "name": "keywords",
+            "program": null
+        },
+        {
+            "input": [],
+            "name": "funding",
+            "program": null
+        },
+        {
+            "input": [],
+            "name": "publications",
+            "program": null
+        },
+        {
+            "input": "graph",
+            "name": "subdatasets",
+            "program": ".[]? | select(.[\"@type\"] == \"Dataset\") | [.hasPart[]? | {\"dataset_id\": (.[\"identifier\"] // \"\" | sub(\"^datalad:\"; \"\")), \"dataset_version\": (.[\"@id\"] | sub(\"^datalad:\"; \"\")), \"dataset_path\": .[\"name\"], \"dirs_from_path\": []}]"
+        },
+        {
+            "input": [],
+            "name": "children",
+            "program": null
+        },
+        {
+            "input": "metadata",
+            "name": "extractors_used",
+            "program": "[{\"extractor_name\": .extractor_name, \"extractor_version\": .extractor_version, \"extraction_parameter\": .extraction_parameter, \"extraction_time\": .extraction_time, \"agent_name\": .agent_name, \"agent_email\": .agent_email,}]"
         }
-    },
-    "social_links": {
-        "about": null,
-        "documentation": "https://docs.datalad.org/projects/catalog/en/latest/",
-        "github": "https://github.com/datalad/datalad-catalog",
-        "twitter": "https://twitter.com/datalad"
+    ],
+    "variables": {
+        "extracted": ".extracted_metadata",
+        "graph": ".extracted_metadata[\"@graph\"]?",
+        "metadata": "."
     }
 }
```

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/constants.py` & `datalad_catalog-0.2.2/datalad_catalog/constants.py`

 * *Files 24% similar despite different names*

```diff
@@ -28,34 +28,26 @@
 EXTRACTOR_NAME = "extractor_name"
 EXTRACTOR_STUDYMINIMETA = "metalad_studyminimeta"
 EXTRACTOR_VERSION = "extractor_version"
 EXTRACTORS = "extractors"
 EXTRACTORS_USED = "extractors_used"
 HASPART = "hasPart"
 IDENTIFIER = "identifier"
-KEY_SOURCE_MAP = "key_source_map"
 LOGO_PATH = "logo_path"
-METADATA_SOURCES = "metadata_sources"
 NAME = "name"
 ORIGIN = "origin"
 PATH = "path"
 PERSONLIST = "#personList"
-PROPERTY_SOURCES = "property_sources"
+PROPERTY_SOURCE = "property_source"
 PUBLICATION = "publication"
 PUBLICATIONS = "publications"
 PUBLICATIONLIST = "#publicationList"
 SAMEAS = "sameAs"
 SOURCE = "source"
-SOURCES = "sources"
-SOURCE_NAME = "source_name"
-SOURCE_VERSION = "source_version"
-SOURCE_PARAMETER = "source_parameter"
-SOURCE_TIME = "source_time"
 STRIPDATALAD = "datalad:"
 STUDY = "study"
 SUBDATASETS = "subdatasets"
 TYPE = "type"
 TYPE_DATASET = "dataset"
 TYPE_DIRECTORY = "directory"
 TYPE_FILE = "file"
 URL = "url"
-VERSION = "version"
```

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/extractors/datacite_gin.py` & `datalad_catalog-0.2.2/datalad_catalog/extractors/datacite_gin.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,17 +13,16 @@
 from uuid import UUID
 
 from datalad_metalad.extractors.base import (
     DatasetMetadataExtractor,
     DataOutputCategory,
     ExtractorResult,
 )
-from datalad_metalad.extractors.legacy.definitions import vocabulary_id
 from datalad.log import log_progress
-from datalad.utils import ensure_unicode
+from datalad.utils import assure_unicode
 
 
 lgr = logging.getLogger("datalad.metadata.extractors.datacite_gin")
 
 # From metalad legacy; TODO: remove/replace when it becomes useful
 # identifiers that defines an ontology as a whole
 vocabulary_id = "http://purl.org/dc/dcam/VocabularyEncodingScheme"
@@ -115,9 +114,9 @@
         # For now, keep all other fields as they are. Might format/translate in
         # the future. See:
         # https://github.com/datalad/datalad-metalad/issues/202#issuecomment-1024192167
         return metadata
 
     def _get_description(self, description_in):
         """"""
-        desc = ensure_unicode(description_in)
+        desc = assure_unicode(description_in)
         return desc.strip()
```

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/meta_item.py` & `datalad_catalog-0.2.2/datalad_catalog/meta_item.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,25 +20,24 @@
     A single metadata item input to datalad catalog in its raw state and translated
     into a node, set of nodes, and/or child of a node.
 
     This class takes care of the delineation of a metadata item into nodes based on
     the item type (dataset / file) and the path of the item.
     """
 
-    # PROCESS DESCRIPTION:
-    # 1. Receive a validated item
-    # 2. Check whether file or dataset:
-    # IF dataset:
-    #   - create/get dataset node
-    #   - loop through metaitem keys, copy values
-    #   - loop through subdatasets, create children and directory nodes
-    # IF file:
-    #   - create/get parent dataset node
-    #   - loop through keys, copy values
-    #   - create children and directory nodes
+    # get validated item
+    # check whether file or dataset
+    # dataset:
+    # - create/get dataset node
+    # - loop through metaitem keys, copy values
+    # - loop through subdatasets, create children and directory nodes
+    # file:
+    # - create/get parent dataset node
+    # - loop through keys, copy values
+    # - create children and directory nodes
 
     def __init__(self, catalog: WebCatalog, meta_item: dict) -> None:
         # Get dataset id and version
         d_id = meta_item[cnst.DATASET_ID]
         d_version = meta_item[cnst.DATASET_VERSION]
         self._node_instances = {}
         # For both type dataset and type file, we need the dataset Node instance
```

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/schema/jsonschema_authors.json` & `datalad_catalog-0.2.2/datalad_catalog/schema/jsonschema_authors.json`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/schema/jsonschema_catalog.json` & `datalad_catalog-0.2.2/datalad_catalog/schema/jsonschema_catalog.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8571428571428571%*

 * *Differences: {'delete': "['version']"}*

```diff
@@ -25,10 +25,9 @@
             "then": {
                 "$ref": "https://datalad.org/catalog.file.schema.json"
             }
         }
     ],
     "description": "The main catalog schema",
     "title": "catalog",
-    "type": "object",
-    "version": "1.0.0"
+    "type": "object"
 }
```

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/schema/jsonschema_dataset.json` & `datalad_catalog-0.2.2/datalad_catalog/schema/jsonschema_dataset.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9853869047619047%*

 * *Differences: {"'properties'": "{'additional_display': {'description': 'Additonal items to display in tabs on "*

 * *                 "dataset page'}, 'top_display': {'description': 'Additonal items to display at "*

 * *                 "the top of the dataset page (along with keywords, description, etc)'}, "*

 * *                 "'extractors_used': OrderedDict([('$ref', "*

 * *                 "'https://datalad.org/catalog.extractors.schema.json')]), delete: "*

 * *                 "['access_request_contact', 'access_request_url', 'metadata_so […]*

```diff
@@ -1,78 +1,14 @@
 {
     "$id": "https://datalad.org/catalog.dataset.schema.json",
     "$schema": "https://json-schema.org/draft/2020-12/schema",
     "description": "A dataset in a DataLad Catalog",
     "properties": {
-        "access_request_contact": {
-            "description": "The contact details of the person/office from which to request access to the dataset content",
-            "properties": {
-                "email": {
-                    "description": "Email address of the author, such as johndoe@example.com",
-                    "format": "email",
-                    "title": "Email",
-                    "type": "string"
-                },
-                "familyName": {
-                    "description": "The author's last/family name, such as 'Doe'",
-                    "title": "Family name",
-                    "type": "string"
-                },
-                "givenName": {
-                    "description": "The author's given name, such as 'John'",
-                    "title": "Given name",
-                    "type": "string"
-                },
-                "honorificSuffix": {
-                    "description": "Title of the author, such as 'Dr.'",
-                    "title": "Honorific suffix",
-                    "type": "string"
-                },
-                "identifiers": {
-                    "description": "Identifiers for the person",
-                    "items": {
-                        "properties": {
-                            "identifier": {
-                                "description": "The actual identifier, such as the ORCID ID '0000-1212-5566'",
-                                "title": "Identifier",
-                                "type": "string"
-                            },
-                            "type": {
-                                "description": "Type of identifier, such as 'ORCID'",
-                                "title": "Type",
-                                "type": "string"
-                            }
-                        },
-                        "type": "object"
-                    },
-                    "title": "Identifiers",
-                    "type": "array"
-                },
-                "name": {
-                    "description": "A concatenation of the honorificSuffix, givenName and familyName properties, such as 'Dr. John Doe'",
-                    "title": "Name",
-                    "type": "string"
-                }
-            },
-            "required": [
-                "givenName",
-                "familyName",
-                "email"
-            ],
-            "title": "Access Request Contact",
-            "type": "object"
-        },
-        "access_request_url": {
-            "description": "The url of the online location from which to request access to the dataset content",
-            "format": "uri",
-            "title": "Access Request URL",
-            "type": "string"
-        },
         "additional_display": {
-            "description": "Additional items to display in tabs on dataset page",
+            "description": "Additonal items to display in tabs on dataset page",
             "items": {
                 "properties": {
                     "content": {
                         "description": "The content that will appear in the tab when opened, specified as key-value pairs",
                         "title": "Content",
                         "type": "object"
                     },
@@ -119,14 +55,17 @@
             ]
         },
         "doi": {
             "description": "The dataset's digital object identifier",
             "title": "DOI",
             "type": "string"
         },
+        "extractors_used": {
+            "$ref": "https://datalad.org/catalog.extractors.schema.json"
+        },
         "funding": {
             "description": "Sources of funding for the dataset",
             "items": {
                 "properties": {
                     "description": {
                         "description": "Free form description of grant or funding",
                         "title": "Description",
@@ -184,17 +123,14 @@
                     "description": "A URL where a description of the license can be viewed",
                     "title": "URL",
                     "type": "string"
                 }
             },
             "type": "object"
         },
-        "metadata_sources": {
-            "$ref": "https://datalad.org/catalog.metadata_sources.schema.json"
-        },
         "name": {
             "description": "The long name of the dataset",
             "title": "Name",
             "type": "string"
         },
         "publications": {
             "description": "Publications related to the dataset",
@@ -276,15 +212,15 @@
                 "type": "object"
             },
             "title": "Subdatasets",
             "type": "array",
             "uniqueItems": true
         },
         "top_display": {
-            "description": "Additional items to display at the top of the dataset page (along with keywords, description, etc)",
+            "description": "Additonal items to display at the top of the dataset page (along with keywords, description, etc)",
             "items": {
                 "properties": {
                     "name": {
                         "description": "Name of the item that will appear as part of the top display",
                         "title": "Name",
                         "type": "string"
                     },
```

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/schema/jsonschema_file.json` & `datalad_catalog-0.2.2/datalad_catalog/schema/jsonschema_file.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9837301587301587%*

 * *Differences: {"'properties'": "{'additional_display': {'description': 'Additonal items to display on the file "*

 * *                 "level'}, 'extractors_used': OrderedDict([('$ref', "*

 * *                 "'https://datalad.org/catalog.extractors.schema.json')]), delete: "*

 * *                 "['metadata_sources']}"}*

```diff
@@ -1,14 +1,14 @@
 {
     "$id": "https://datalad.org/catalog.file.schema.json",
     "$schema": "https://json-schema.org/draft/2020-12/schema",
     "description": "A file in a DataLad Catalog",
     "properties": {
         "additional_display": {
-            "description": "Additional items to display on the file level",
+            "description": "Additonal items to display on the file level",
             "items": {
                 "properties": {
                     "content": {
                         "description": "The content that will appear when selecting the file, specified as key-value pairs",
                         "title": "Content",
                         "type": "object"
                     },
@@ -39,16 +39,16 @@
             "type": "string"
         },
         "dataset_version": {
             "description": "The parent dataset VERSION",
             "title": "Dataset version",
             "type": "string"
         },
-        "metadata_sources": {
-            "$ref": "https://datalad.org/catalog.metadata_sources.schema.json"
+        "extractors_used": {
+            "$ref": "https://datalad.org/catalog.extractors.schema.json"
         },
         "path": {
             "description": "The path of the file relative to its parent dataset",
             "title": "Path",
             "type": "string"
         },
         "type": {
```

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/tests/data/catalog_metadata_dataset.json` & `datalad_catalog-0.2.2/datalad_catalog/tests/data/catalog_metadata_dataset.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8947368421052632%*

 * *Differences: {"'extractors_used'": "[OrderedDict([('extractor_name', 'bids_dataset'), ('extractor_version', "*

 * *                      "'0.0.1'), ('extraction_parameter', OrderedDict()), ('extraction_time', "*

 * *                      "1643901350.65269), ('agent_name', 'Stephan Heunis'), ('agent_email', "*

 * *                      "'s.heunis@fz-juelich.de')])]",*

 * * 'delete': "['metadata_sources']"}*

```diff
@@ -165,14 +165,24 @@
         }
     ],
     "children": [],
     "dataset_id": "5eaff716-54eb-11e8-803d-a0369f7c647e",
     "dataset_version": "72f835ada046bd0479009ea0ff933b30a95b0076",
     "description": "hello description",
     "doi": "",
+    "extractors_used": [
+        {
+            "agent_email": "s.heunis@fz-juelich.de",
+            "agent_name": "Stephan Heunis",
+            "extraction_parameter": {},
+            "extraction_time": 1643901350.65269,
+            "extractor_name": "bids_dataset",
+            "extractor_version": "0.0.1"
+        }
+    ],
     "funding": [
         {
             "description": "We acknowledge the support of the Combinatorial NeuroImaging Core Facility at the Leibniz Institute for Neurobiology in Magdeburg, and the German federal state of Saxony-Anhalt, Project: Center for Behavioral Brain Sciences. This research was, in part, also supported by the German Federal Ministry of Education and Research (BMBF) as part of a US-German collaboration in computational neuroscience (CRCNS), co-funded by the BMBF and the US National Science Foundation (BMBF 01GQ1112; NSF 1129855). Work on the data-sharing technology employed for this research was supported by US-German CRCNS project, co-funded by the BMBF and the US National Science Foundation (BMBF 01GQ1411; NSF 1429999).",
             "grant": "",
             "name": ""
         }
     ],
@@ -204,27 +214,14 @@
         "vision_problems_past",
         "suffix"
     ],
     "license": {
         "name": "PDDL",
         "url": ""
     },
-    "metadata_sources": {
-        "key_source_map": {},
-        "sources": [
-            {
-                "agent_email": "s.heunis@fz-juelich.de",
-                "agent_name": "Stephan Heunis",
-                "source_name": "bids_dataset",
-                "source_parameter": {},
-                "source_time": 1643901350.65269,
-                "source_version": "0.0.1"
-            }
-        ]
-    },
     "name": "studyforrest_phase2",
     "publications": [],
     "short_name": "",
     "subdatasets": [],
     "top_display": [
         {
             "name": "Subjects",
```

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/tests/data/catalog_metadata_valid.json` & `datalad_catalog-0.2.2/datalad_catalog/tests/data/catalog_metadata_valid.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8%*

 * *Differences: {"'extractors_used'": "[OrderedDict([('extractor_name', 'metalad_core'), ('extractor_version', "*

 * *                      "'1'), ('extraction_parameter', OrderedDict()), ('extraction_time', "*

 * *                      "1649839999.652626), ('agent_name', 'Stephan Heunis'), ('agent_email', "*

 * *                      "'s.heunis@fz-juelich.de')])]",*

 * * 'delete': "['access_request_contact', 'access_request_url', 'metadata_sources']"}*

```diff
@@ -1,14 +1,8 @@
 {
-    "access_request_contact": {
-        "email": "adina@example.com",
-        "familyName": "Wagner",
-        "givenName": "Adina"
-    },
-    "access_request_url": "https://github.com/datalad/datalad-catalog",
     "authors": [
         {
             "email": "adina.wagner@t-online.de",
             "name": "Adina Wagner"
         },
         {
             "email": "michael.hanke@gmail.com",
@@ -67,30 +61,27 @@
             "content": "",
             "name": "README.md",
             "path": "README.md",
             "type": "file"
         }
     ],
     "doi": "",
+    "extractors_used": [
+        {
+            "agent_email": "s.heunis@fz-juelich.de",
+            "agent_name": "Stephan Heunis",
+            "extraction_parameter": {},
+            "extraction_time": 1649839999.652626,
+            "extractor_name": "metalad_core",
+            "extractor_version": "1"
+        }
+    ],
     "funding": [],
     "keywords": [],
     "license": {},
-    "metadata_sources": {
-        "key_source_map": {},
-        "sources": [
-            {
-                "agent_email": "s.heunis@fz-juelich.de",
-                "agent_name": "Stephan Heunis",
-                "source_name": "metalad_core",
-                "source_parameter": {},
-                "source_time": 1649839999.652626,
-                "source_version": "1"
-            }
-        ]
-    },
     "name": "StudyForrest",
     "publications": [],
     "short_name": "",
     "subdatasets": [
         {
             "dataset_id": "d5dd3da0-a631-4c0c-a4a9-de55dfc4620f",
             "dataset_path": "artifact/3T_movie_eyetracking",
```

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/tests/data/metadata_bids_dataset.json` & `datalad_catalog-0.2.2/datalad_catalog/tests/data/metadata_bids_dataset.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9979166666666666%*

 * *Differences: {"'extracted_metadata'": "{'description': ['An Extension of studyforrest.org "*

 * *                         'Dataset\\n****************************************\\n\\n|license| '*

 * *                         '|access| |doi|\\n\\nSimultaneous fMRI/eyetracking while movie watching, '*

 * *                         'plus visual '*

 * *                         'localizers\\n==========================================================================\\n\\nThis '*

 * *                         'is an extension of the studyforrest project, al […]*

```diff
@@ -29,15 +29,15 @@
         "HowToAcknowledge": "Please follow good scientific practice by citing the most appropriate publication(s) describing the aspects of this datasets that were used in a study.",
         "License": "PDDL",
         "Name": "studyforrest_phase2",
         "ReferencesAndLinks": [
             "http://studyforrest.org"
         ],
         "description": [
-            "An Extension of studyforrest.org Dataset\n****************************************\n\n|license| |access| |doi|\n\nSimultaneous fMRI/eyetracking while movie watching, plus visual localizers\n==========================================================================\n\nThis is an extension of the studyforrest project, all participants previously\nvolunteered for the audio-only Forrest Gump study. The dataset is structured in\nBIDS format, details of the files and metadata can be found at:\n\n     Ayan Sengupta, Falko R. Kaule, J. Swaroop Guntupalli, Michael B. Hoffmann,\n     Christian H\u00e4usler, J\u00f6rg Stadler, Michael Hanke. `An extension of the\n     studyforrest dataset for vision research\n     <http://biorxiv.org/content/early/2016/03/31/046573>`_. (submitted for\n     publication)\n\n     Michael Hanke, Nico Adelh\u00f6fer, Daniel Kottke, Vittorio Iacovella,\n     Ayan Sengupta, Falko R. Kaule, Roland Nigbur, Alexander Q. Waite,\n     Florian J. Baumgartner & J\u00f6rg Stadler. `Simultaneous fMRI and eye gaze\n     recordings during prolonged natural stimulation \u2013 a studyforrest extension\n     <http://biorxiv.org/content/early/2016/03/31/046581>`_. (submitted for\n     publication)\n\nFor more information about the project visit: http://studyforrest.org\n\n\nHow to obtain the dataset\n-------------------------\n\nThe dataset is available for download from `OpenFMRI (accession number\nds000113d) <https://www.openfmri.org/dataset/ds000113d>`_.\n\nAlternatively, the `studyforrest phase 2 repository on GitHub\n<https://github.com/psychoinformatics-de/studyforrest-data-phase2>`_ provides\naccess as a DataLad dataset.\n\nDataLad datasets and how to use them\n------------------------------------\n\nThis repository is a `DataLad <https://www.datalad.org/>`__ dataset. It provides\nfine-grained data access down to the level of individual files, and allows for\ntracking future updates up to the level of single files. In order to use\nthis repository for data retrieval, `DataLad <https://www.datalad.org>`_ is\nrequired. It is a free and open source command line tool, available for all\nmajor operating systems, and builds up on Git and `git-annex\n<https://git-annex.branchable.com>`__ to allow sharing, synchronizing, and\nversion controlling collections of large files. You can find information on\nhow to install DataLad at `handbook.datalad.org/en/latest/intro/installation.html\n<http://handbook.datalad.org/en/latest/intro/installation.html>`_.\n\nGet the dataset\n^^^^^^^^^^^^^^^\n\nA DataLad dataset can be ``cloned`` by running::\n\n   datalad clone <url>\n\nOnce a dataset is cloned, it is a light-weight directory on your local machine.\nAt this point, it contains only small metadata and information on the\nidentity of the files in the dataset, but not actual *content* of the\n(sometimes large) data files.\n\nRetrieve dataset content\n^^^^^^^^^^^^^^^^^^^^^^^^\n\nAfter cloning a dataset, you can retrieve file contents by running::\n\n   datalad get <path/to/directory/or/file>\n\nThis command will trigger a download of the files, directories, or\nsubdatasets you have specified.\n\nDataLad datasets can contain other datasets, so called *subdatasets*. If you\nclone the top-level dataset, subdatasets do not yet contain metadata and\ninformation on the identity of files, but appear to be empty directories. In\norder to retrieve file availability metadata in subdatasets, run::\n\n   datalad get -n <path/to/subdataset>\n\nAfterwards, you can browse the retrieved metadata to find out about\nsubdataset contents, and retrieve individual files with ``datalad get``. If you\nuse ``datalad get <path/to/subdataset>``, all contents of the subdataset will\nbe downloaded at once.\n\nStay up-to-date\n^^^^^^^^^^^^^^^\n\nDataLad datasets can be updated. The command ``datalad update`` will *fetch*\nupdates and store them on a different branch (by default\n``remotes/origin/master``). Running::\n\n   datalad update --merge\n\nwill *pull* available updates and integrate them in one go.\n\nMore information\n^^^^^^^^^^^^^^^^\n\nMore information on DataLad and how to use it can be found in the DataLad Handbook at\n`handbook.datalad.org <http://handbook.datalad.org/en/latest/index.html>`_. The\nchapter \"DataLad datasets\" can help you to familiarize yourself with the\nconcept of a dataset.\n\n\n.. _Git: http://www.git-scm.com\n\n.. _git-annex: http://git-annex.branchable.com/\n\n.. |license|\n   image:: https://img.shields.io/badge/license-PDDL-blue.svg\n    :target: http://opendatacommons.org/licenses/pddl/summary\n    :alt: PDDL-licensed\n\n.. |access|\n   image:: https://img.shields.io/badge/data_access-unrestricted-green.svg\n    :alt: No registration or authentication required\n\n.. |doi|\n   image:: https://zenodo.org/badge/14167/psychoinformatics-de/studyforrest-data-phase2.svg\n    :target: https://zenodo.org/badge/latestdoi/14167/psychoinformatics-de/studyforrest-data-phase2\n    :alt: DOI"
+            "An Extension of studyforrest.org Dataset\n****************************************\n\n|license| |access| |doi|\n\nSimultaneous fMRI/eyetracking while movie watching, plus visual localizers\n==========================================================================\n\nThis is an extension of the studyforrest project, all participants previously\nvolunteered for the audio-only Forrest Gump study. The datset is structured in\nBIDS format, details of the files and metadata can be found at:\n\n     Ayan Sengupta, Falko R. Kaule, J. Swaroop Guntupalli, Michael B. Hoffmann,\n     Christian H\u00e4usler, J\u00f6rg Stadler, Michael Hanke. `An extension of the\n     studyforrest dataset for vision research\n     <http://biorxiv.org/content/early/2016/03/31/046573>`_. (submitted for\n     publication)\n\n     Michael Hanke, Nico Adelh\u00f6fer, Daniel Kottke, Vittorio Iacovella,\n     Ayan Sengupta, Falko R. Kaule, Roland Nigbur, Alexander Q. Waite,\n     Florian J. Baumgartner & J\u00f6rg Stadler. `Simultaneous fMRI and eye gaze\n     recordings during prolonged natural stimulation \u2013 a studyforrest extension\n     <http://biorxiv.org/content/early/2016/03/31/046581>`_. (submitted for\n     publication)\n\nFor more information about the project visit: http://studyforrest.org\n\n\nHow to obtain the dataset\n-------------------------\n\nThe dataset is available for download from `OpenFMRI (accession number\nds000113d) <https://www.openfmri.org/dataset/ds000113d>`_.\n\nAlternatively, the `studyforrest phase 2 repository on GitHub\n<https://github.com/psychoinformatics-de/studyforrest-data-phase2>`_ provides\naccess as a DataLad dataset.\n\nDataLad datasets and how to use them\n------------------------------------\n\nThis repository is a `DataLad <https://www.datalad.org/>`__ dataset. It provides\nfine-grained data access down to the level of individual files, and allows for\ntracking future updates up to the level of single files. In order to use\nthis repository for data retrieval, `DataLad <https://www.datalad.org>`_ is\nrequired. It is a free and open source command line tool, available for all\nmajor operating systems, and builds up on Git and `git-annex\n<https://git-annex.branchable.com>`__ to allow sharing, synchronizing, and\nversion controlling collections of large files. You can find information on\nhow to install DataLad at `handbook.datalad.org/en/latest/intro/installation.html\n<http://handbook.datalad.org/en/latest/intro/installation.html>`_.\n\nGet the dataset\n^^^^^^^^^^^^^^^\n\nA DataLad dataset can be ``cloned`` by running::\n\n   datalad clone <url>\n\nOnce a dataset is cloned, it is a light-weight directory on your local machine.\nAt this point, it contains only small metadata and information on the\nidentity of the files in the dataset, but not actual *content* of the\n(sometimes large) data files.\n\nRetrieve dataset content\n^^^^^^^^^^^^^^^^^^^^^^^^\n\nAfter cloning a dataset, you can retrieve file contents by running::\n\n   datalad get <path/to/directory/or/file>\n\nThis command will trigger a download of the files, directories, or\nsubdatasets you have specified.\n\nDataLad datasets can contain other datasets, so called *subdatasets*. If you\nclone the top-level dataset, subdatasets do not yet contain metadata and\ninformation on the identity of files, but appear to be empty directories. In\norder to retrieve file availability metadata in subdatasets, run::\n\n   datalad get -n <path/to/subdataset>\n\nAfterwards, you can browse the retrieved metadata to find out about\nsubdataset contents, and retrieve individual files with ``datalad get``. If you\nuse ``datalad get <path/to/subdataset>``, all contents of the subdataset will\nbe downloaded at once.\n\nStay up-to-date\n^^^^^^^^^^^^^^^\n\nDataLad datasets can be updated. The command ``datalad update`` will *fetch*\nupdates and store them on a different branch (by default\n``remotes/origin/master``). Running::\n\n   datalad update --merge\n\nwill *pull* available updates and integrate them in one go.\n\nMore information\n^^^^^^^^^^^^^^^^\n\nMore information on DataLad and how to use it can be found in the DataLad Handbook at\n`handbook.datalad.org <http://handbook.datalad.org/en/latest/index.html>`_. The\nchapter \"DataLad datasets\" can help you to familiarize yourself with the\nconcept of a dataset.\n\n\n.. _Git: http://www.git-scm.com\n\n.. _git-annex: http://git-annex.branchable.com/\n\n.. |license|\n   image:: https://img.shields.io/badge/license-PDDL-blue.svg\n    :target: http://opendatacommons.org/licenses/pddl/summary\n    :alt: PDDL-licensed\n\n.. |access|\n   image:: https://img.shields.io/badge/data_access-unrestricted-green.svg\n    :alt: No registration or authentication required\n\n.. |doi|\n   image:: https://zenodo.org/badge/14167/psychoinformatics-de/studyforrest-data-phase2.svg\n    :target: https://zenodo.org/badge/latestdoi/14167/psychoinformatics-de/studyforrest-data-phase2\n    :alt: DOI"
         ],
         "entities": {
             "datatype": [
                 "beh",
                 "func"
             ],
             "extension": [
```

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/tests/data/metadata_bids_dataset.jsonl` & `datalad_catalog-0.2.2/datalad_catalog/tests/data/metadata_bids_dataset.jsonl`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/tests/data/metadata_bids_dataset2.json` & `datalad_catalog-0.2.2/datalad_catalog/tests/data/metadata_bids_dataset2.json`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/tests/data/metadata_bids_dataset2.jsonl` & `datalad_catalog-0.2.2/datalad_catalog/tests/data/metadata_bids_dataset2.jsonl`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9979166666666666%*

 * *Differences: {"'extracted_metadata'": "{'description': ['An Extension of studyforrest.org "*

 * *                         'Dataset\\n****************************************\\n\\n|license| '*

 * *                         '|access| |doi|\\n\\nSimultaneous fMRI/eyetracking while movie watching, '*

 * *                         'plus visual '*

 * *                         'localizers\\n==========================================================================\\n\\nThis '*

 * *                         'is an extension of the studyforrest project, al […]*

```diff
@@ -29,15 +29,15 @@
         "HowToAcknowledge": "Please follow good scientific practice by citing the most appropriate publication(s) describing the aspects of this datasets that were used in a study.",
         "License": "PDDL",
         "Name": "studyforrest_phase2",
         "ReferencesAndLinks": [
             "http://studyforrest.org"
         ],
         "description": [
-            "An Extension of studyforrest.org Dataset\n****************************************\n\n|license| |access| |doi|\n\nSimultaneous fMRI/eyetracking while movie watching, plus visual localizers\n==========================================================================\n\nThis is an extension of the studyforrest project, all participants previously\nvolunteered for the audio-only Forrest Gump study. The dataset is structured in\nBIDS format, details of the files and metadata can be found at:\n\n     Ayan Sengupta, Falko R. Kaule, J. Swaroop Guntupalli, Michael B. Hoffmann,\n     Christian H\u00e4usler, J\u00f6rg Stadler, Michael Hanke. `An extension of the\n     studyforrest dataset for vision research\n     <http://biorxiv.org/content/early/2016/03/31/046573>`_. (submitted for\n     publication)\n\n     Michael Hanke, Nico Adelh\u00f6fer, Daniel Kottke, Vittorio Iacovella,\n     Ayan Sengupta, Falko R. Kaule, Roland Nigbur, Alexander Q. Waite,\n     Florian J. Baumgartner & J\u00f6rg Stadler. `Simultaneous fMRI and eye gaze\n     recordings during prolonged natural stimulation \u2013 a studyforrest extension\n     <http://biorxiv.org/content/early/2016/03/31/046581>`_. (submitted for\n     publication)\n\nFor more information about the project visit: http://studyforrest.org\n\n\nHow to obtain the dataset\n-------------------------\n\nThe dataset is available for download from `OpenFMRI (accession number\nds000113d) <https://www.openfmri.org/dataset/ds000113d>`_.\n\nAlternatively, the `studyforrest phase 2 repository on GitHub\n<https://github.com/psychoinformatics-de/studyforrest-data-phase2>`_ provides\naccess as a DataLad dataset.\n\nDataLad datasets and how to use them\n------------------------------------\n\nThis repository is a `DataLad <https://www.datalad.org/>`__ dataset. It provides\nfine-grained data access down to the level of individual files, and allows for\ntracking future updates up to the level of single files. In order to use\nthis repository for data retrieval, `DataLad <https://www.datalad.org>`_ is\nrequired. It is a free and open source command line tool, available for all\nmajor operating systems, and builds up on Git and `git-annex\n<https://git-annex.branchable.com>`__ to allow sharing, synchronizing, and\nversion controlling collections of large files. You can find information on\nhow to install DataLad at `handbook.datalad.org/en/latest/intro/installation.html\n<http://handbook.datalad.org/en/latest/intro/installation.html>`_.\n\nGet the dataset\n^^^^^^^^^^^^^^^\n\nA DataLad dataset can be ``cloned`` by running::\n\n   datalad clone <url>\n\nOnce a dataset is cloned, it is a light-weight directory on your local machine.\nAt this point, it contains only small metadata and information on the\nidentity of the files in the dataset, but not actual *content* of the\n(sometimes large) data files.\n\nRetrieve dataset content\n^^^^^^^^^^^^^^^^^^^^^^^^\n\nAfter cloning a dataset, you can retrieve file contents by running::\n\n   datalad get <path/to/directory/or/file>\n\nThis command will trigger a download of the files, directories, or\nsubdatasets you have specified.\n\nDataLad datasets can contain other datasets, so called *subdatasets*. If you\nclone the top-level dataset, subdatasets do not yet contain metadata and\ninformation on the identity of files, but appear to be empty directories. In\norder to retrieve file availability metadata in subdatasets, run::\n\n   datalad get -n <path/to/subdataset>\n\nAfterwards, you can browse the retrieved metadata to find out about\nsubdataset contents, and retrieve individual files with ``datalad get``. If you\nuse ``datalad get <path/to/subdataset>``, all contents of the subdataset will\nbe downloaded at once.\n\nStay up-to-date\n^^^^^^^^^^^^^^^\n\nDataLad datasets can be updated. The command ``datalad update`` will *fetch*\nupdates and store them on a different branch (by default\n``remotes/origin/master``). Running::\n\n   datalad update --merge\n\nwill *pull* available updates and integrate them in one go.\n\nMore information\n^^^^^^^^^^^^^^^^\n\nMore information on DataLad and how to use it can be found in the DataLad Handbook at\n`handbook.datalad.org <http://handbook.datalad.org/en/latest/index.html>`_. The\nchapter \"DataLad datasets\" can help you to familiarize yourself with the\nconcept of a dataset.\n\n\n.. _Git: http://www.git-scm.com\n\n.. _git-annex: http://git-annex.branchable.com/\n\n.. |license|\n   image:: https://img.shields.io/badge/license-PDDL-blue.svg\n    :target: http://opendatacommons.org/licenses/pddl/summary\n    :alt: PDDL-licensed\n\n.. |access|\n   image:: https://img.shields.io/badge/data_access-unrestricted-green.svg\n    :alt: No registration or authentication required\n\n.. |doi|\n   image:: https://zenodo.org/badge/14167/psychoinformatics-de/studyforrest-data-phase2.svg\n    :target: https://zenodo.org/badge/latestdoi/14167/psychoinformatics-de/studyforrest-data-phase2\n    :alt: DOI"
+            "An Extension of studyforrest.org Dataset\n****************************************\n\n|license| |access| |doi|\n\nSimultaneous fMRI/eyetracking while movie watching, plus visual localizers\n==========================================================================\n\nThis is an extension of the studyforrest project, all participants previously\nvolunteered for the audio-only Forrest Gump study. The datset is structured in\nBIDS format, details of the files and metadata can be found at:\n\n     Ayan Sengupta, Falko R. Kaule, J. Swaroop Guntupalli, Michael B. Hoffmann,\n     Christian H\u00e4usler, J\u00f6rg Stadler, Michael Hanke. `An extension of the\n     studyforrest dataset for vision research\n     <http://biorxiv.org/content/early/2016/03/31/046573>`_. (submitted for\n     publication)\n\n     Michael Hanke, Nico Adelh\u00f6fer, Daniel Kottke, Vittorio Iacovella,\n     Ayan Sengupta, Falko R. Kaule, Roland Nigbur, Alexander Q. Waite,\n     Florian J. Baumgartner & J\u00f6rg Stadler. `Simultaneous fMRI and eye gaze\n     recordings during prolonged natural stimulation \u2013 a studyforrest extension\n     <http://biorxiv.org/content/early/2016/03/31/046581>`_. (submitted for\n     publication)\n\nFor more information about the project visit: http://studyforrest.org\n\n\nHow to obtain the dataset\n-------------------------\n\nThe dataset is available for download from `OpenFMRI (accession number\nds000113d) <https://www.openfmri.org/dataset/ds000113d>`_.\n\nAlternatively, the `studyforrest phase 2 repository on GitHub\n<https://github.com/psychoinformatics-de/studyforrest-data-phase2>`_ provides\naccess as a DataLad dataset.\n\nDataLad datasets and how to use them\n------------------------------------\n\nThis repository is a `DataLad <https://www.datalad.org/>`__ dataset. It provides\nfine-grained data access down to the level of individual files, and allows for\ntracking future updates up to the level of single files. In order to use\nthis repository for data retrieval, `DataLad <https://www.datalad.org>`_ is\nrequired. It is a free and open source command line tool, available for all\nmajor operating systems, and builds up on Git and `git-annex\n<https://git-annex.branchable.com>`__ to allow sharing, synchronizing, and\nversion controlling collections of large files. You can find information on\nhow to install DataLad at `handbook.datalad.org/en/latest/intro/installation.html\n<http://handbook.datalad.org/en/latest/intro/installation.html>`_.\n\nGet the dataset\n^^^^^^^^^^^^^^^\n\nA DataLad dataset can be ``cloned`` by running::\n\n   datalad clone <url>\n\nOnce a dataset is cloned, it is a light-weight directory on your local machine.\nAt this point, it contains only small metadata and information on the\nidentity of the files in the dataset, but not actual *content* of the\n(sometimes large) data files.\n\nRetrieve dataset content\n^^^^^^^^^^^^^^^^^^^^^^^^\n\nAfter cloning a dataset, you can retrieve file contents by running::\n\n   datalad get <path/to/directory/or/file>\n\nThis command will trigger a download of the files, directories, or\nsubdatasets you have specified.\n\nDataLad datasets can contain other datasets, so called *subdatasets*. If you\nclone the top-level dataset, subdatasets do not yet contain metadata and\ninformation on the identity of files, but appear to be empty directories. In\norder to retrieve file availability metadata in subdatasets, run::\n\n   datalad get -n <path/to/subdataset>\n\nAfterwards, you can browse the retrieved metadata to find out about\nsubdataset contents, and retrieve individual files with ``datalad get``. If you\nuse ``datalad get <path/to/subdataset>``, all contents of the subdataset will\nbe downloaded at once.\n\nStay up-to-date\n^^^^^^^^^^^^^^^\n\nDataLad datasets can be updated. The command ``datalad update`` will *fetch*\nupdates and store them on a different branch (by default\n``remotes/origin/master``). Running::\n\n   datalad update --merge\n\nwill *pull* available updates and integrate them in one go.\n\nMore information\n^^^^^^^^^^^^^^^^\n\nMore information on DataLad and how to use it can be found in the DataLad Handbook at\n`handbook.datalad.org <http://handbook.datalad.org/en/latest/index.html>`_. The\nchapter \"DataLad datasets\" can help you to familiarize yourself with the\nconcept of a dataset.\n\n\n.. _Git: http://www.git-scm.com\n\n.. _git-annex: http://git-annex.branchable.com/\n\n.. |license|\n   image:: https://img.shields.io/badge/license-PDDL-blue.svg\n    :target: http://opendatacommons.org/licenses/pddl/summary\n    :alt: PDDL-licensed\n\n.. |access|\n   image:: https://img.shields.io/badge/data_access-unrestricted-green.svg\n    :alt: No registration or authentication required\n\n.. |doi|\n   image:: https://zenodo.org/badge/14167/psychoinformatics-de/studyforrest-data-phase2.svg\n    :target: https://zenodo.org/badge/latestdoi/14167/psychoinformatics-de/studyforrest-data-phase2\n    :alt: DOI"
         ],
         "entities": {
             "datatype": [
                 "func",
                 "beh"
             ],
             "extension": [
```

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/tests/data/metadata_core.json` & `datalad_catalog-0.2.2/datalad_catalog/tests/data/metadata_core.json`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/tests/data/metadata_core.jsonl` & `datalad_catalog-0.2.2/datalad_catalog/tests/data/metadata_core.jsonl`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/tests/data/metadata_core_dataset.json` & `datalad_catalog-0.2.2/datalad_catalog/tests/data/metadata_core_dataset.json`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/tests/data/metadata_datacite_gin.json` & `datalad_catalog-0.2.2/datalad_catalog/tests/data/metadata_datacite_gin.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9974999999999999%*

 * *Differences: {"'extracted_metadata'": "{'description': 'Extension of the dataset published in Hanke et al. "*

 * *                         '(2014; doi:10.1038/sdata.2014.3) with additional acquisitions for 15 of '*

 * *                         'the original 20 participants. These additions include: retinotopic '*

 * *                         'mapping, a localizer paradigm for higher visual areas (FFA, EBA, PPA), '*

 * *                         'and another 2h movie recording with 3T full-brain BOLD fMRI with '*

 * *                         'sim […]*

```diff
@@ -48,15 +48,15 @@
                 "lastname": "Kottke"
             },
             {
                 "firstname": "J\u00f6rg",
                 "lastname": "Stadler"
             }
         ],
-        "description": "Extension of the dataset published in Hanke et al. (2014; doi:10.1038/sdata.2014.3) with additional acquisitions for 15 of the original 20 participants. These additions include: retinotopic mapping, a localizer paradigm for higher visual areas (FFA, EBA, PPA), and another 2h movie recording with 3T full-brain BOLD fMRI with simultaneous 1000 Hz eyetracking. This is an extension of the studyforrest project, all participants previously volunteered for the audio-only Forrest Gump study. The dataset is structured in BIDS format, details of the files and metadata can be found at:   Ayan Sengupta, Falko R. Kaule, J. Swaroop Guntupalli, Michael B. Hoffmann,   Christian H\u00e4usler, J\u00f6rg Stadler, Michael Hanke. `An extension of the   studyforrest dataset for vision research   <http://biorxiv.org/content/early/2016/03/31/046573>`_. (submitted for   publication)   Michael Hanke, Nico Adelh\u00f6fer, Daniel Kottke, Vittorio Iacovella,   Ayan Sengupta, Falko R. Kaule, Roland Nigbur, Alexander Q. Waite,   Florian J. Baumgartner & J\u00f6rg Stadler. `Simultaneous fMRI and eye gaze   recordings during prolonged natural stimulation \u2013 a studyforrest extension   <http://biorxiv.org/content/early/2016/03/31/046581>`_. (submitted for   publication) For more information about the project visit: http://studyforrest.org We acknowledge the support of the Combinatorial NeuroImaging Core Facility at the Leibniz Institute for Neurobiology in Magdeburg, and the German federal state of Saxony-Anhalt, Project: Center for Behavioral Brain Sciences. This research was, in part, also supported by the German Federal Ministry of Education and Research (BMBF) as part of a US-German collaboration in computational neuroscience (CRCNS), co-funded by the BMBF and the US National Science Foundation (BMBF 01GQ1112; NSF 1129855). Work on the data-sharing technology employed for this research was supported by US-German CRCNS project, co-funded by the BMBF and the US National Science Foundation (BMBF 01GQ1411; NSF 1429999).",
+        "description": "Extension of the dataset published in Hanke et al. (2014; doi:10.1038/sdata.2014.3) with additional acquisitions for 15 of the original 20 participants. These additions include: retinotopic mapping, a localizer paradigm for higher visual areas (FFA, EBA, PPA), and another 2h movie recording with 3T full-brain BOLD fMRI with simultaneous 1000 Hz eyetracking. This is an extension of the studyforrest project, all participants previously volunteered for the audio-only Forrest Gump study. The datset is structured in BIDS format, details of the files and metadata can be found at:   Ayan Sengupta, Falko R. Kaule, J. Swaroop Guntupalli, Michael B. Hoffmann,   Christian H\u00e4usler, J\u00f6rg Stadler, Michael Hanke. `An extension of the   studyforrest dataset for vision research   <http://biorxiv.org/content/early/2016/03/31/046573>`_. (submitted for   publication)   Michael Hanke, Nico Adelh\u00f6fer, Daniel Kottke, Vittorio Iacovella,   Ayan Sengupta, Falko R. Kaule, Roland Nigbur, Alexander Q. Waite,   Florian J. Baumgartner & J\u00f6rg Stadler. `Simultaneous fMRI and eye gaze   recordings during prolonged natural stimulation \u2013 a studyforrest extension   <http://biorxiv.org/content/early/2016/03/31/046581>`_. (submitted for   publication) For more information about the project visit: http://studyforrest.org We acknowledge the support of the Combinatorial NeuroImaging Core Facility at the Leibniz Institute for Neurobiology in Magdeburg, and the German federal state of Saxony-Anhalt, Project: Center for Behavioral Brain Sciences. This research was, in part, also supported by the German Federal Ministry of Education and Research (BMBF) as part of a US-German collaboration in computational neuroscience (CRCNS), co-funded by the BMBF and the US National Science Foundation (BMBF 01GQ1112; NSF 1129855). Work on the data-sharing technology employed for this research was supported by US-German CRCNS project, co-funded by the BMBF and the US National Science Foundation (BMBF 01GQ1411; NSF 1429999).",
         "funding": [
             "BMBF, 01GQ1112",
             "NSF, 1129855",
             "BMBF, 01GQ1411",
             "NSF, 1429999"
         ],
         "keywords": [
```

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/tests/data/metadata_datacite_gin.jsonl` & `datalad_catalog-0.2.2/datalad_catalog/tests/data/metadata_datacite_gin.jsonl`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9974999999999999%*

 * *Differences: {"'extracted_metadata'": '{\'description\': \'"Extension of the dataset published in Hanke et '*

 * *                         'al.\\n (2014; doi:10.1038/sdata.2014.3) with additional acquisitions for '*

 * *                         '15 of\\n the original 20 participants. These additions include: '*

 * *                         'retinotopic mapping,\\n a localizer paradigm for higher visual areas '*

 * *                         '(FFA, EBA, PPA), and another\\n 2h movie recording with 3T full-brain '*

 * *                         'BO […]*

```diff
@@ -48,15 +48,15 @@
                 "lastname": "Kottke"
             },
             {
                 "firstname": "J\u00f6rg",
                 "lastname": "Stadler"
             }
         ],
-        "description": "\"Extension of the dataset published in Hanke et al.\n (2014; doi:10.1038/sdata.2014.3) with additional acquisitions for 15 of\n the original 20 participants. These additions include: retinotopic mapping,\n a localizer paradigm for higher visual areas (FFA, EBA, PPA), and another\n 2h movie recording with 3T full-brain BOLD fMRI with simultaneous 1000 Hz\n eyetracking.\n\n This is an extension of the studyforrest project, all participants previously\n volunteered for the audio-only Forrest Gump study. The dataset is structured in\n BIDS format, details of the files and metadata can be found at:\n\n   Ayan Sengupta, Falko R. Kaule, J. Swaroop Guntupalli, Michael B. Hoffmann,\n   Christian H\u00e4usler, J\u00f6rg Stadler, Michael Hanke. `An extension of the\n   studyforrest dataset for vision research\n   <http://biorxiv.org/content/early/2016/03/31/046573>`_. (submitted for\n   publication)\n\n   Michael Hanke, Nico Adelh\u00f6fer, Daniel Kottke, Vittorio Iacovella,\n   Ayan Sengupta, Falko R. Kaule, Roland Nigbur, Alexander Q. Waite,\n   Florian J. Baumgartner & J\u00f6rg Stadler. `Simultaneous fMRI and eye gaze\n   recordings during prolonged natural stimulation \u2013 a studyforrest extension\n   <http://biorxiv.org/content/early/2016/03/31/046581>`_. (submitted for\n   publication)\n\n For more information about the project visit: http://studyforrest.org\n\n We acknowledge the support of the Combinatorial NeuroImaging Core\n Facility at the Leibniz Institute for Neurobiology in Magdeburg, and\n the German federal state of Saxony-Anhalt, Project: Center for\n Behavioral Brain Sciences. This research was, in part, also supported\n by the German Federal Ministry of Education and Research (BMBF) as\n part of a US-German collaboration in computational neuroscience (CRCNS),\n co-funded by the BMBF and the US National Science Foundation\n (BMBF 01GQ1112; NSF 1129855). Work on the data-sharing technology\n employed for this research was supported by US-German CRCNS project,\n co-funded by the BMBF and the US National Science Foundation\n (BMBF 01GQ1411; NSF 1429999).\"",
+        "description": "\"Extension of the dataset published in Hanke et al.\n (2014; doi:10.1038/sdata.2014.3) with additional acquisitions for 15 of\n the original 20 participants. These additions include: retinotopic mapping,\n a localizer paradigm for higher visual areas (FFA, EBA, PPA), and another\n 2h movie recording with 3T full-brain BOLD fMRI with simultaneous 1000 Hz\n eyetracking.\n\n This is an extension of the studyforrest project, all participants previously\n volunteered for the audio-only Forrest Gump study. The datset is structured in\n BIDS format, details of the files and metadata can be found at:\n\n   Ayan Sengupta, Falko R. Kaule, J. Swaroop Guntupalli, Michael B. Hoffmann,\n   Christian H\u00e4usler, J\u00f6rg Stadler, Michael Hanke. `An extension of the\n   studyforrest dataset for vision research\n   <http://biorxiv.org/content/early/2016/03/31/046573>`_. (submitted for\n   publication)\n\n   Michael Hanke, Nico Adelh\u00f6fer, Daniel Kottke, Vittorio Iacovella,\n   Ayan Sengupta, Falko R. Kaule, Roland Nigbur, Alexander Q. Waite,\n   Florian J. Baumgartner & J\u00f6rg Stadler. `Simultaneous fMRI and eye gaze\n   recordings during prolonged natural stimulation \u2013 a studyforrest extension\n   <http://biorxiv.org/content/early/2016/03/31/046581>`_. (submitted for\n   publication)\n\n For more information about the project visit: http://studyforrest.org\n\n We acknowledge the support of the Combinatorial NeuroImaging Core\n Facility at the Leibniz Institute for Neurobiology in Magdeburg, and\n the German federal state of Saxony-Anhalt, Project: Center for\n Behavioral Brain Sciences. This research was, in part, also supported\n by the German Federal Ministry of Education and Research (BMBF) as\n part of a US-German collaboration in computational neuroscience (CRCNS),\n co-funded by the BMBF and the US National Science Foundation\n (BMBF 01GQ1112; NSF 1129855). Work on the data-sharing technology\n employed for this research was supported by US-German CRCNS project,\n co-funded by the BMBF and the US National Science Foundation\n (BMBF 01GQ1411; NSF 1429999).\"",
         "funding": [
             "BMBF, 01GQ1112",
             "NSF, 1129855",
             "BMBF, 01GQ1411",
             "NSF, 1429999"
         ],
         "keywords": [
```

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/tests/data/metadata_studyminimeta.json` & `datalad_catalog-0.2.2/datalad_catalog/tests/data/metadata_studyminimeta.json`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/tests/data/metadata_studyminimeta.jsonl` & `datalad_catalog-0.2.2/datalad_catalog/tests/data/metadata_studyminimeta.jsonl`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/tests/data/workflow_generated_meta_sub.json` & `datalad_catalog-0.2.2/datalad_catalog/tests/data/workflow_generated_meta_sub.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6923076923076923%*

 * *Differences: {"'dataset_id'": "'ce345be8-eba6-476a-a52c-94ed2ca535fe'",*

 * * "'dataset_version'": "'d90b0dd1bc8f270ab16107dbeff77d54a50f298c'",*

 * * "'description'": '[OrderedDict([(\'content\', \'"Extension of the dataset published in Hanke et '*

 * *                  'al.\\n (2014; doi:10.1038/sdata.2014.3) with additional acquisitions for 15 '*

 * *                  'of\\n the original 20 participants. These additions include: retinotopic '*

 * *                  'mapping,\\n a localizer paradigm for higher visual areas (FFA, EBA, PPA), an […]*

```diff
@@ -55,17 +55,40 @@
                     "type": "ORCID"
                 }
             ],
             "name": ""
         }
     ],
     "children": [],
-    "dataset_id": "48e08e83-4c13-406a-8532-584b4d78ce06",
-    "dataset_version": "4f78ff4a3c5622e0a1475631e882cad3433f98ac",
-    "description": "\"Extension of the dataset published in Hanke et al.\n (2014; doi:10.1038/sdata.2014.3) with additional acquisitions for 15 of\n the original 20 participants. These additions include: retinotopic mapping,\n a localizer paradigm for higher visual areas (FFA, EBA, PPA), and another\n 2h movie recording with 3T full-brain BOLD fMRI with simultaneous 1000 Hz\n eyetracking.\n\n This is an extension of the studyforrest project, all participants previously\n volunteered for the audio-only Forrest Gump study. The dataset is structured in\n BIDS format, details of the files and metadata can be found at:\n\n   Ayan Sengupta, Falko R. Kaule, J. Swaroop Guntupalli, Michael B. Hoffmann,\n   Christian H\u00e4usler, J\u00f6rg Stadler, Michael Hanke. `An extension of the\n   studyforrest dataset for vision research\n   <http://biorxiv.org/content/early/2016/03/31/046573>`_. (submitted for\n   publication)\n\n   Michael Hanke, Nico Adelh\u00f6fer, Daniel Kottke, Vittorio Iacovella,\n   Ayan Sengupta, Falko R. Kaule, Roland Nigbur, Alexander Q. Waite,\n   Florian J. Baumgartner & J\u00f6rg Stadler. `Simultaneous fMRI and eye gaze\n   recordings during prolonged natural stimulation \u2013 a studyforrest extension\n   <http://biorxiv.org/content/early/2016/03/31/046581>`_. (submitted for\n   publication)\n\n For more information about the project visit: http://studyforrest.org\n\n We acknowledge the support of the Combinatorial NeuroImaging Core\n Facility at the Leibniz Institute for Neurobiology in Magdeburg, and\n the German federal state of Saxony-Anhalt, Project: Center for\n Behavioral Brain Sciences. This research was, in part, also supported\n by the German Federal Ministry of Education and Research (BMBF) as\n part of a US-German collaboration in computational neuroscience (CRCNS),\n co-funded by the BMBF and the US National Science Foundation\n (BMBF 01GQ1112; NSF 1129855). Work on the data-sharing technology\n employed for this research was supported by US-German CRCNS project,\n co-funded by the BMBF and the US National Science Foundation\n (BMBF 01GQ1411; NSF 1429999).\"",
+    "dataset_id": "ce345be8-eba6-476a-a52c-94ed2ca535fe",
+    "dataset_version": "d90b0dd1bc8f270ab16107dbeff77d54a50f298c",
+    "description": [
+        {
+            "content": "\"Extension of the dataset published in Hanke et al.\n (2014; doi:10.1038/sdata.2014.3) with additional acquisitions for 15 of\n the original 20 participants. These additions include: retinotopic mapping,\n a localizer paradigm for higher visual areas (FFA, EBA, PPA), and another\n 2h movie recording with 3T full-brain BOLD fMRI with simultaneous 1000 Hz\n eyetracking.\n\n This is an extension of the studyforrest project, all participants previously\n volunteered for the audio-only Forrest Gump study. The datset is structured in\n BIDS format, details of the files and metadata can be found at:\n\n   Ayan Sengupta, Falko R. Kaule, J. Swaroop Guntupalli, Michael B. Hoffmann,\n   Christian H\u00e4usler, J\u00f6rg Stadler, Michael Hanke. `An extension of the\n   studyforrest dataset for vision research\n   <http://biorxiv.org/content/early/2016/03/31/046573>`_. (submitted for\n   publication)\n\n   Michael Hanke, Nico Adelh\u00f6fer, Daniel Kottke, Vittorio Iacovella,\n   Ayan Sengupta, Falko R. Kaule, Roland Nigbur, Alexander Q. Waite,\n   Florian J. Baumgartner & J\u00f6rg Stadler. `Simultaneous fMRI and eye gaze\n   recordings during prolonged natural stimulation \u2013 a studyforrest extension\n   <http://biorxiv.org/content/early/2016/03/31/046581>`_. (submitted for\n   publication)\n\n For more information about the project visit: http://studyforrest.org\n\n We acknowledge the support of the Combinatorial NeuroImaging Core\n Facility at the Leibniz Institute for Neurobiology in Magdeburg, and\n the German federal state of Saxony-Anhalt, Project: Center for\n Behavioral Brain Sciences. This research was, in part, also supported\n by the German Federal Ministry of Education and Research (BMBF) as\n part of a US-German collaboration in computational neuroscience (CRCNS),\n co-funded by the BMBF and the US National Science Foundation\n (BMBF 01GQ1112; NSF 1129855). Work on the data-sharing technology\n employed for this research was supported by US-German CRCNS project,\n co-funded by the BMBF and the US National Science Foundation\n (BMBF 01GQ1411; NSF 1429999).\"",
+            "source": "datacite_gin"
+        }
+    ],
+    "extractors_used": [
+        {
+            "agent_email": "s.heunis@fz-juelich.de",
+            "agent_name": "Stephan Heunis",
+            "extraction_parameter": {},
+            "extraction_time": 1659000883.00646,
+            "extractor_name": "metalad_core",
+            "extractor_version": "1"
+        },
+        {
+            "agent_email": "s.heunis@fz-juelich.de",
+            "agent_name": "Stephan Heunis",
+            "extraction_parameter": {},
+            "extraction_time": 1659000883.1729012,
+            "extractor_name": "datacite_gin",
+            "extractor_version": "0.0.1"
+        }
+    ],
     "funding": [
         {
             "description": "",
             "identifier": "",
             "name": "BMBF, 01GQ1112"
         },
         {
@@ -89,56 +112,15 @@
         "Studyforrest",
         "BIDS"
     ],
     "license": {
         "name": "Open Data Commons Public Domain Dedication and License (PDDL)",
         "url": "https://opendatacommons.org/licenses/pddl/"
     },
-    "metadata_sources": {
-        "key_source_map": {
-            "authors": [
-                "metalad_core",
-                "datacite_gin"
-            ],
-            "dataset_id": [
-                "metalad_core"
-            ],
-            "dataset_version": [
-                "metalad_core"
-            ],
-            "description": [
-                "datacite_gin"
-            ],
-            "keywords": [
-                "datacite_gin"
-            ],
-            "type": [
-                "metalad_core"
-            ]
-        },
-        "sources": [
-            {
-                "agent_email": "s.heunis@fz-juelich.de",
-                "agent_name": "Stephan Heunis",
-                "source_name": "metalad_core",
-                "source_parameter": {},
-                "source_time": 1675717944.9006562,
-                "source_version": "1"
-            },
-            {
-                "agent_email": "s.heunis@fz-juelich.de",
-                "agent_name": "Stephan Heunis",
-                "source_name": "datacite_gin",
-                "source_parameter": {},
-                "source_time": 1675717945.078315,
-                "source_version": "0.0.1"
-            }
-        ]
-    },
-    "name": null,
+    "name": "Simultaneous fMRI/eyetracking while movie watching, plus visual localizers",
     "publications": [
         {
             "authors": [],
             "datePublished": "",
             "doi": "doi:10.1038/sdata.2016.93",
             "publicationOutlet": "",
             "title": "Sengupta, A., Kaule, F. R., Guntupalli, J. S., Hoffmann, M. B., H\u00e4usler, C., Stadler, J., Hanke, M. (2016). A studyforrest extension, retinotopic mapping and localization of higher visual areas. Scientific Data, 3, 160093.",
```

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/tests/data/workflow_generated_meta_super.json` & `datalad_catalog-0.2.2/datalad_catalog/tests/data/workflow_generated_meta_super.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7211538461538461%*

 * *Differences: {"'dataset_id'": "'201d7059-1491-4a4f-909f-5cd918d5d2ec'",*

 * * "'dataset_version'": "'4bea05fe4cb1ad3dfcef9a07437e5a0f3b2b445e'",*

 * * "'description'": "[OrderedDict([('content', 'The StudyForrest project centers around the use of "*

 * *                  'the movie Forrest Gump, which provides complex sensory input that is both '*

 * *                  'reproducible and is also richly laden with real-life-like content and contexts. '*

 * *                  'Since its initial release, the StudyForrest dataset has grown and been  […]*

```diff
@@ -17,75 +17,45 @@
     "children": [
         {
             "name": "some_dir",
             "path": "some_dir",
             "type": "directory"
         }
     ],
-    "dataset_id": "e27af456-a66c-452e-b3cb-62bb5a564307",
-    "dataset_version": "569fd768420742a5de20922526f9d9a5231975e9",
-    "description": "The StudyForrest project centers around the use of the movie Forrest Gump, which provides complex sensory input that is both reproducible and is also richly laden with real-life-like content and contexts. Since its initial release, the StudyForrest dataset has grown and been extended substantially, and now encompasses many hours of fMRI scans, structural brain scans, eye-tracking data, and extensive annotations of the movie.",
+    "dataset_id": "201d7059-1491-4a4f-909f-5cd918d5d2ec",
+    "dataset_version": "4bea05fe4cb1ad3dfcef9a07437e5a0f3b2b445e",
+    "description": [
+        {
+            "content": "The StudyForrest project centers around the use of the movie Forrest Gump, which provides complex sensory input that is both reproducible and is also richly laden with real-life-like content and contexts. Since its initial release, the StudyForrest dataset has grown and been extended substantially, and now encompasses many hours of fMRI scans, structural brain scans, eye-tracking data, and extensive annotations of the movie.",
+            "source": "metalad_studyminimeta"
+        }
+    ],
+    "extractors_used": [
+        {
+            "agent_email": "s.heunis@fz-juelich.de",
+            "agent_name": "Stephan Heunis",
+            "extraction_parameter": {},
+            "extraction_time": 1659000881.718712,
+            "extractor_name": "metalad_core",
+            "extractor_version": "1"
+        },
+        {
+            "agent_email": "s.heunis@fz-juelich.de",
+            "agent_name": "Stephan Heunis",
+            "extraction_parameter": {},
+            "extraction_time": 1659000881.765142,
+            "extractor_name": "metalad_studyminimeta",
+            "extractor_version": "0.1"
+        }
+    ],
     "keywords": [
         "human",
         "fMRI",
         "task"
     ],
-    "metadata_sources": {
-        "key_source_map": {
-            "authors": [
-                "metalad_studyminimeta",
-                "metalad_core"
-            ],
-            "dataset_id": [
-                "metalad_core"
-            ],
-            "dataset_version": [
-                "metalad_core"
-            ],
-            "description": [
-                "metalad_studyminimeta"
-            ],
-            "keywords": [
-                "metalad_studyminimeta"
-            ],
-            "name": [
-                "metalad_studyminimeta"
-            ],
-            "publications": [
-                "metalad_studyminimeta"
-            ],
-            "subdatasets": [
-                "metalad_core"
-            ],
-            "type": [
-                "metalad_core"
-            ],
-            "url": [
-                "metalad_studyminimeta"
-            ]
-        },
-        "sources": [
-            {
-                "agent_email": "s.heunis@fz-juelich.de",
-                "agent_name": "Stephan Heunis",
-                "source_name": "metalad_core",
-                "source_parameter": {},
-                "source_time": 1675717944.0956402,
-                "source_version": "1"
-            },
-            {
-                "agent_email": "s.heunis@fz-juelich.de",
-                "agent_name": "Stephan Heunis",
-                "source_name": "metalad_studyminimeta",
-                "source_parameter": {},
-                "source_time": 1675717944.16534,
-                "source_version": "0.1"
-            }
-        ]
-    },
     "name": "StudyForrest",
     "publications": [
         {
             "authors": [
                 {
                     "@id": "https://schema.datalad.org/person#a@fz-juelich.de",
                     "@type": "Person",
@@ -183,17 +153,17 @@
             "publicationOutlet": "F1000Research",
             "title": "Spatial band-pass filtering aids decoding musical genres from auditory cortex 7T fMRI",
             "type": "ScholarlyArticle"
         }
     ],
     "subdatasets": [
         {
-            "dataset_id": "48e08e83-4c13-406a-8532-584b4d78ce06",
+            "dataset_id": "ce345be8-eba6-476a-a52c-94ed2ca535fe",
             "dataset_path": "some_dir/subdataset",
-            "dataset_version": "4f78ff4a3c5622e0a1475631e882cad3433f98ac",
+            "dataset_version": "d90b0dd1bc8f270ab16107dbeff77d54a50f298c",
             "dirs_from_path": [
                 "some_dir",
                 "subdataset"
             ]
         }
     ],
     "type": "dataset",
```

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/tests/test_action_create.py` & `datalad_catalog-0.2.2/datalad_catalog/tests/test_action_create.py`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/tests/test_action_setsuper.py` & `datalad_catalog-0.2.2/datalad_catalog/tests/test_action_setsuper.py`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/tests/test_catalog.py` & `datalad_catalog-0.2.2/datalad_catalog/tests/test_catalog.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 )
 from unittest.mock import (
     call,
     patch,
 )
 
 from datalad.support.exceptions import InsufficientArgumentsError
-from datalad.tests.utils import (
+from datalad.tests.utils_pytest import (
     assert_equal,
     assert_in,
     assert_raises,
     with_tempfile,
 )
 from jsonschema.exceptions import ValidationError
 
@@ -119,31 +119,28 @@
         "datalad_catalog.catalog._create_catalog"
     ) as f2, patch("datalad_catalog.catalog._serve_catalog") as f3, patch(
         "datalad_catalog.catalog._add_to_catalog"
     ) as f4, patch(
         "datalad_catalog.catalog._remove_from_catalog"
     ) as f5, patch(
         "datalad_catalog.catalog._set_super_of_catalog"
-    ) as f6, patch(
-        "datalad_catalog.catalog._translate_metadata"
-    ) as f7:
+    ) as f6:
         for mock, name in zip(
-            (f1, f2, f3, f4, f5, f6, f7), (f"f{i}" for i in range(1, 8))
+            (f1, f2, f3, f4, f5, f6), (f"f{i}" for i in range(1, 7))
         ):
             mock.return_value = iter([{**result_template, "action": name}])
 
         results = []
         for action, create_dir in (
             ("create", False),
             ("validate", False),
             ("add", True),
             ("remove", True),
             ("set-super", True),
             ("serve", True),
-            ("translate", True),
         ):
             test_catalog_path = Path(temp_dir) / "test_catalog"
 
             if create_dir:
                 try:
                     test_catalog_path.mkdir()
                     (test_catalog_path / "assets").mkdir()
@@ -167,9 +164,9 @@
                             "catalog_dir": str(test_catalog_path),
                             "result_renderer": "disabled",
                         }
                     )
                 )[0]["action"]
             )
 
-        for i in range(1, 8):
+        for i in range(1, 7):
             assert_in(f"f{i}", results)
```

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/tests/test_catalog_arguments.py` & `datalad_catalog-0.2.2/datalad_catalog/tests/test_catalog_arguments.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 from datalad.support.exceptions import InsufficientArgumentsError
-from datalad.tests.utils import (
+from datalad.tests.utils_pytest import (
     assert_in_results,
     assert_raises,
 )
 from datalad_catalog.catalog import Catalog
 
 
 def test_catalog_no_argument():
```

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/tests/test_meta_item.py` & `datalad_catalog-0.2.2/datalad_catalog/tests/test_translate.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,36 +8,39 @@
 from datalad_catalog import constants as cnst
 from datalad_catalog.meta_item import MetaItem
 from datalad_catalog.utils import read_json_file
 from datalad_catalog.webcatalog import (
     Node,
     WebCatalog,
 )
+from datalad.tests.utils_pytest import (
+    assert_in_results,
+    assert_raises,
+    assert_result_count,
+)
 
 tests_path = Path(__file__).resolve().parent
 data_path = tests_path / "data"
 
 
 @pytest.fixture
 def demo_catalog(tmp_path):
     catalog_path = tmp_path / "test_catalog"
-
-    return WebCatalog(location=catalog_path, catalog_action="create")
+    return WebCatalog(location=catalog_path)
 
 
 @pytest.fixture
 def demo_metadata_item():
     metadata_path = data_path / "catalog_metadata_dataset.json"
     return read_json_file(metadata_path)
 
 
 def test_translate_dataset(demo_catalog: WebCatalog, demo_metadata_item: dict):
     """"""
-    assert demo_catalog.catalog_config
-    demo_catalog.catalog_config = {"property_sources": {"dataset": {}}}
+    demo_catalog.config = {"property_source": {"dataset": {}}}
     metatest = MetaItem(demo_catalog, demo_metadata_item)
     assert len(metatest._node_instances) == 1
     new_node = [
         metatest._node_instances[n]
         for n in metatest._node_instances
         if metatest._node_instances[n].dataset_id
         == demo_metadata_item[cnst.DATASET_ID]
@@ -48,9 +51,8 @@
     fn = new_node[0].get_location()
     new_node[0].write_attributes_to_file()
     translated_metadata = read_json_file(fn)
     for key in translated_metadata:
         if not bool(translated_metadata[key]):
             continue
         assert key in demo_metadata_item
-        if key != "metadata_sources":
-            assert demo_metadata_item[key] == translated_metadata[key]
+        assert demo_metadata_item[key] == translated_metadata[key]
```

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/tests/test_schema.py` & `datalad_catalog-0.2.2/datalad_catalog/tests/test_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from datalad_catalog.catalog import Catalog
 from datalad_catalog.utils import read_json_file
 from datalad_catalog.webcatalog import WebCatalog
 
 # Setup schema parameters
 package_path = Path(__file__).resolve().parent.parent
 schema_dir = package_path / "schema"
-schemas = ["dataset", "file", "authors", "metadata_sources"]
+schemas = ["dataset", "file", "authors", "extractors"]
 schema_store = {}
 for s in schemas:
     schema_path = schema_dir / str("jsonschema_" + s + ".json")
     schema = read_json_file(schema_path)
     schema_store[schema["$id"]] = schema
 dataset_schema = schema_store["https://datalad.org/catalog.dataset.schema.json"]
```

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/tests/test_webcatalog.py` & `datalad_catalog-0.2.2/datalad_catalog/tests/test_webcatalog.py`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/tests/test_workflow.py` & `datalad_catalog-0.2.2/datalad_catalog/tests/test_workflow.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,16 +32,14 @@
     "datacite_gin": tests_path / "data" / "metadata_datacite_gin.json",
     "metalad_studyminimeta": tests_path
     / "data"
     / "metadata_studyminimeta.json",
     "bids_dataset": tests_path / "data" / "metadata_bids_dataset2.json",
 }
 
-test_config_file = tests_path / "data" / "test_config_file_workflow.json"
-
 studyminimeta_content = """\
 #<!-- METADATA START --> # DO NOT DELETE THIS LINE
 # All example text is surrounded with <ex> and </ex>. Please replace the example
 # text including the <ex> and </ex> with your data. Delete all non-applicable
 # lines and sections.
 
 # Attention: indentation is important and must be preserved!
@@ -181,15 +179,15 @@
    (2014; doi:10.1038/sdata.2014.3) with additional acquisitions for 15 of
    the original 20 participants. These additions include: retinotopic mapping,
    a localizer paradigm for higher visual areas (FFA, EBA, PPA), and another
    2h movie recording with 3T full-brain BOLD fMRI with simultaneous 1000 Hz
    eyetracking.
 
    This is an extension of the studyforrest project, all participants previously
-   volunteered for the audio-only Forrest Gump study. The dataset is structured in
+   volunteered for the audio-only Forrest Gump study. The datset is structured in
    BIDS format, details of the files and metadata can be found at:
 
      Ayan Sengupta, Falko R. Kaule, J. Swaroop Guntupalli, Michael B. Hoffmann,
      Christian Häusler, Jörg Stadler, Michael Hanke. `An extension of the
      studyforrest dataset for vision research
      <http://biorxiv.org/content/early/2016/03/31/046573>`_. (submitted for
      publication)
@@ -314,17 +312,15 @@
     super_ds.save(to_git=True, **ckwa)
     assert_repo_status(super_ds.path)
     # Test if metadata files exist
     assert (Path(sub_ds.path) / "datacite.yml").exists()
     assert (Path(super_ds.path) / ".studyminimeta.yaml").exists()
     # Create catalog
     cat_path = Path(cat_path)
-    cat = WebCatalog(
-        location=cat_path, catalog_action="create", config_file=test_config_file
-    )
+    cat = WebCatalog(location=cat_path)
     cat.create(force=True)
     assert cat_path.exists()
     assert cat_path.is_dir()
     for p in catalog_paths:
         pth = cat_path / p
         assert pth.exists()
     # Run workflow
@@ -368,36 +364,29 @@
     )
     assert superds_node_path.exists()
     generated_meta = read_json_file(superds_node_path)
     correct_meta_path = (
         tests_path / "data" / "workflow_generated_meta_super.json"
     )
     correct_meta = read_json_file(correct_meta_path)
-    assert_equal(
-        list(generated_meta.keys()).sort(), list(correct_meta.keys()).sort()
-    )
+    assert_equal(generated_meta.keys(), correct_meta.keys())
     keys_to_test = [
         "authors",
         "children",
         "description",
         "keywords",
         "name",
         "publications",
         "type",
         "url",
     ]
     assert_dict_values_equal(generated_meta, correct_meta, keys_to_test)
-    # keys_to_test = [
-    #     "authors",
-    #     "publications",
-    # ]
-    # assert_dict_values_in_list_equal(generated_meta, correct_meta, keys_to_test)
     assert_super_variable_values_equal(
         generated_meta,
-        ["subdatasets", "metadata_sources", "dataset_id", "dataset_version"],
+        ["subdatasets", "extractors_used", "dataset_id", "dataset_version"],
         dataset_details,
     )
     # - Node metadata directories and content: superdataset subdir
     super_subdir_node_path = get_node_path(
         meta_path,
         dataset_details["super_ds"][0],
         dataset_details["super_ds"][1],
@@ -423,37 +412,30 @@
     subds_node_path = get_node_path(
         meta_path, dataset_details["sub_ds"][0], dataset_details["sub_ds"][1]
     )
     assert subds_node_path.exists()
     generated_meta = read_json_file(subds_node_path)
     correct_meta_path = tests_path / "data" / "workflow_generated_meta_sub.json"
     correct_meta = read_json_file(correct_meta_path)
-    assert_equal(
-        list(generated_meta.keys()).sort(), list(correct_meta.keys()).sort()
-    )
+    assert_equal(generated_meta.keys(), correct_meta.keys())
     keys_to_test = [
         "authors",
         "children",
         "description",
         "funding",
         "keywords",
-        "publications",
         "license",
         "name",
+        "publications",
         "type",
     ]
     assert_dict_values_equal(generated_meta, correct_meta, keys_to_test)
-    # keys_to_test = [
-    #     "authors",
-    #     "publications",
-    # ]
-    # assert_dict_values_in_list_equal(generated_meta, correct_meta, keys_to_test)
     assert_sub_variable_values_equal(
         generated_meta,
-        ["metadata_sources", "dataset_id", "dataset_version"],
+        ["extractors_used", "dataset_id", "dataset_version"],
         dataset_details,
     )
 
 
 def get_node_path(root_path, dataset_id, dataset_version, node_path=None):
     _split_dir_length = Node._split_dir_length
     md5_hash = md5sum_from_id_version_path(
@@ -481,46 +463,18 @@
 
 def assert_dict_values_equal(
     dict_to_test: dict,
     dict_correct: dict,
     keys_to_test: list,
 ):
     """"""
-
     for key in keys_to_test:
         assert_equal(dict_to_test[key], dict_correct[key])
 
 
-def assert_dict_values_in_list_equal(
-    dict_to_test: dict,
-    dict_correct: dict,
-    keys_to_test: list,
-):
-    """"""
-
-    for key in keys_to_test:
-        print("---")
-        print(key)
-        print("---")
-        assert_equal(len(dict_to_test[key]), len(dict_correct[key]))
-        for val in dict_to_test[key]:
-            first_key = list(val.keys())[0]
-            print(f"dict_correct[key]: {dict_correct[key]}")
-            print(f"dict_to_test[key]: {dict_to_test[key]}")
-            print(f"val: {val}")
-            print(f"first_key: {first_key}")
-            print(f"val[first_key]: {val[first_key]}")
-            # print(f"x[first_key]: {x[first_key]}")
-
-            found_obj = [
-                x for x in dict_correct[key] if val[first_key] == x[first_key]
-            ]
-            assert_equal(len(found_obj), 1)
-
-
 def assert_super_variable_values_equal(
     dict_to_test: dict,
     keys_to_test: list,
     dataset_details: dict,
 ):
     """"""
     for key in keys_to_test:
@@ -537,21 +491,20 @@
             "dataset_path": "some_dir/subdataset",
             "dataset_version": f"{dataset_details['sub_ds'][1]}",
             "dirs_from_path": ["some_dir", "subdataset"],
         }
     ]
     assert_equal(dict_to_test["subdatasets"], correct_subds)
     # extractors_used
-    assert_equal(len(dict_to_test["metadata_sources"]["sources"]), 2)
+    assert_equal(len(dict_to_test["extractors_used"]), 2)
     assert_equal(
-        dict_to_test["metadata_sources"]["sources"][0]["source_name"],
-        "metalad_core",
+        dict_to_test["extractors_used"][0]["extractor_name"], "metalad_core"
     )
     assert_equal(
-        dict_to_test["metadata_sources"]["sources"][1]["source_name"],
+        dict_to_test["extractors_used"][1]["extractor_name"],
         "metalad_studyminimeta",
     )
 
 
 def assert_dir_variable_values_equal(
     dict_to_test: dict,
     keys_to_test: list,
@@ -586,16 +539,14 @@
     """"""
     for key in keys_to_test:
         assert key in dict_to_test
     # id and version
     assert_equal(dict_to_test["dataset_id"], dataset_details["sub_ds"][0])
     assert_equal(dict_to_test["dataset_version"], dataset_details["sub_ds"][1])
     # extractors_used
-    assert_equal(len(dict_to_test["metadata_sources"]["sources"]), 2)
+    assert_equal(len(dict_to_test["extractors_used"]), 2)
     assert_equal(
-        dict_to_test["metadata_sources"]["sources"][0]["source_name"],
-        "metalad_core",
+        dict_to_test["extractors_used"][0]["extractor_name"], "metalad_core"
     )
     assert_equal(
-        dict_to_test["metadata_sources"]["sources"][1]["source_name"],
-        "datacite_gin",
+        dict_to_test["extractors_used"][1]["extractor_name"], "datacite_gin"
     )
```

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog/workflows.py` & `datalad_catalog-0.2.2/datalad_catalog/workflows.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,28 +7,20 @@
 from datalad.api import (
     meta_extract,
     meta_conduct,
 )
 from datalad.distribution.dataset import Dataset
 from datalad.local.wtf import _describe_metadata_elements
 from datalad.support.exceptions import IncompleteResultsError
-from datalad_catalog.translate import (
-    Translate,
-    get_translators,
-)
 from datalad_catalog.utils import read_json_file
 from datalad_catalog.webcatalog import WebCatalog
 from datalad_catalog.catalog import (
     _add_to_catalog,
 )
 
-# metadata_file = Path('datalad_catalog/tests/data/metadata_datacite_gin.json')
-# metadata_record = utils.read_json_file(metadata_file)
-# translate.Translate(metadata_record).run_translator()
-
 lgr = logging.getLogger("datalad.catalog.workflows")
 
 # DETAILS FOR EXTRACTORS AND TRANSLATORS
 extractor_names_dataset = [
     "metalad_core",
     "metalad_studyminimeta",
     "bids_dataset",
@@ -189,22 +181,22 @@
     # - Not implemented yet
     # 3. Run translation
     translated_file = Path(ds.path) / "translated_meta.json"
     with open(extracted_file) as file:
         for line in file:
             meta_dict = json.loads(line.rstrip())
             try:
-                # extr_name = meta_dict["extractor_name"]
-                # extr_type = meta_dict["type"]
-                # mapping_path = schema_dir / get_translation_map(
-                #     extr_name, extr_type
-                # )
+                extr_name = meta_dict["extractor_name"]
+                extr_type = meta_dict["type"]
+                mapping_path = schema_dir / get_translation_map(
+                    extr_name, extr_type
+                )
                 write_jsonline_to_file(
                     translated_file,
-                    Translate(meta_dict, get_translators()).run_translator(),
+                    translate_to_catalog(meta_dict, mapping_path),
                 )
             except Exception as e:
                 lgr.error("Failed to translate line due to error: %s", str(e))
                 continue
     # 4. Add translated metadata to catalog
     return _add_to_catalog(catalog, translated_file, dict())
```

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog.egg-info/PKG-INFO` & `datalad_catalog-0.2.2/datalad_catalog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datalad-catalog
-Version: 0.2.1b0
+Version: 0.2.2
 Summary: DataLad Catalog
 Home-page: https://github.com/datalad/datalad-catalog
 Author: DataLad Developers
 Author-email: team@datalad.org
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: BSD License
@@ -22,17 +22,15 @@
 [![GitHub release](https://img.shields.io/github/release/datalad/datalad-catalog.svg)](https://GitHub.com/datalad/datalad-catalog/releases/)
 [![PyPI version fury.io](https://badge.fury.io/py/datalad-catalog.svg)](https://pypi.python.org/pypi/datalad-catalog/)
 [![docs](https://github.com/datalad/datalad-catalog/actions/workflows/docbuild.yml/badge.svg)](https://github.com/datalad/datalad-catalog/actions/workflows/docbuild.yml)
 [![Build status](https://ci.appveyor.com/api/projects/status/github/datalad/datalad-catalog?branch=main&svg=true)](https://ci.appveyor.com/project/mih/datalad-catalog/branch/main)
 [![codecov.io](https://codecov.io/github/datalad/datalad-catalog/coverage.svg?branch=main)](https://codecov.io/github/datalad/datalad-catalog?branch=main)
 [![crippled-filesystems](https://github.com/datalad/datalad-catalog/actions/workflows/test_crippledfs.yml/badge.svg)](https://github.com/datalad/datalad-catalog/actions/workflows/test_crippledfs.yml)
 [![pages-build-deployment](https://github.com/datalad/datalad-catalog/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/datalad/datalad-catalog/actions/workflows/pages/pages-build-deployment)
-[![push_catalog_to_gh_pages](https://github.com/datalad/datalad-catalog/actions/workflows/deploy_demo.yml/badge.svg)](https://github.com/datalad/datalad-catalog/actions/workflows/deploy_demo.yml)
-[![DOI](https://zenodo.org/badge/371040885.svg)](https://zenodo.org/badge/latestdoi/371040885)
-<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
+[![push_catalog_to_gh_pages](https://github.com/datalad/datalad-catalog/actions/workflows/deploy_demo.yml/badge.svg)](https://github.com/datalad/datalad-catalog/actions/workflows/deploy_demo.yml)<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
 [![All Contributors](https://img.shields.io/badge/all_contributors-11-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 
 <picture>
   <source media="(prefers-color-scheme: light)" srcset="docs/source/_static/datacat0_hero.svg">
   <source media="(prefers-color-scheme: dark)" srcset="docs/source/_static/datacat0_hero_lightbg.svg">
```

### Comparing `datalad_catalog-0.2.1b0/datalad_catalog.egg-info/SOURCES.txt` & `datalad_catalog-0.2.2/datalad_catalog.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 _datalad_buildsupport/setup.py
 datalad_catalog/__init__.py
 datalad_catalog/_version.py
 datalad_catalog/catalog.py
 datalad_catalog/conftest.py
 datalad_catalog/constants.py
 datalad_catalog/meta_item.py
-datalad_catalog/translate.py
 datalad_catalog/utils.py
 datalad_catalog/webcatalog.py
 datalad_catalog/workflows.py
 datalad_catalog.egg-info/PKG-INFO
 datalad_catalog.egg-info/SOURCES.txt
 datalad_catalog.egg-info/dependency_links.txt
 datalad_catalog.egg-info/entry_points.txt
@@ -51,16 +50,16 @@
 datalad_catalog/catalog/assets/fa-brands-400.woff2
 datalad_catalog/catalog/assets/fa-regular-400.woff2
 datalad_catalog/catalog/assets/fa-solid-900.woff2
 datalad_catalog/catalog/assets/fontawesome.min.css
 datalad_catalog/catalog/assets/jsonschema_authors.json
 datalad_catalog/catalog/assets/jsonschema_catalog.json
 datalad_catalog/catalog/assets/jsonschema_dataset.json
+datalad_catalog/catalog/assets/jsonschema_extractors.json
 datalad_catalog/catalog/assets/jsonschema_file.json
-datalad_catalog/catalog/assets/jsonschema_metadata_sources.json
 datalad_catalog/catalog/assets/marked.4.0.17.min.js
 datalad_catalog/catalog/assets/md5-2.3.0.js
 datalad_catalog/catalog/assets/meta_entry.js
 datalad_catalog/catalog/assets/style.css
 datalad_catalog/catalog/assets/vue-router.3.5.3.min.js
 datalad_catalog/catalog/assets/vue.2.6.14.min.js
 datalad_catalog/catalog/assets/favicon/favicon-16x16.png
@@ -70,84 +69,70 @@
 datalad_catalog/catalog/templates/dataset-template.html
 datalad_catalog/catalog/templates/item-template.html
 datalad_catalog/catalog/templates/main-template.html
 datalad_catalog/config/config.json
 datalad_catalog/config/config.yml
 datalad_catalog/extractors/__init__.py
 datalad_catalog/extractors/datacite_gin.py
+datalad_catalog/schema/_bidsdataset2catalog.json
+datalad_catalog/schema/_datacitegin2catalog.json
+datalad_catalog/schema/_metaladcore2catalog_dataset.json
+datalad_catalog/schema/_metaladcore2catalog_file.json
+datalad_catalog/schema/_studyminimeta2catalog.json
 datalad_catalog/schema/jsonschema_authors.json
 datalad_catalog/schema/jsonschema_catalog.json
 datalad_catalog/schema/jsonschema_dataset.json
+datalad_catalog/schema/jsonschema_extractors.json
 datalad_catalog/schema/jsonschema_file.json
-datalad_catalog/schema/jsonschema_metadata_sources.json
 datalad_catalog/tests/__init__.py
 datalad_catalog/tests/register.py
 datalad_catalog/tests/test_action_add.py
 datalad_catalog/tests/test_action_create.py
 datalad_catalog/tests/test_action_setsuper.py
-datalad_catalog/tests/test_add_update_attributes.py
 datalad_catalog/tests/test_catalog.py
 datalad_catalog/tests/test_catalog_arguments.py
 datalad_catalog/tests/test_config.py
-datalad_catalog/tests/test_meta_item.py
+datalad_catalog/tests/test_multisource.py
 datalad_catalog/tests/test_node.py
 datalad_catalog/tests/test_schema.py
 datalad_catalog/tests/test_translate.py
 datalad_catalog/tests/test_utils.py
 datalad_catalog/tests/test_webcatalog.py
 datalad_catalog/tests/test_workflow.py
 datalad_catalog/tests/data/catalog_metadata_dataset.json
-datalad_catalog/tests/data/catalog_metadata_dataset.jsonl
-datalad_catalog/tests/data/catalog_metadata_dataset2.jsonl
-datalad_catalog/tests/data/catalog_metadata_dataset_updated.json
-datalad_catalog/tests/data/catalog_metadata_dataset_updated_min.json
 datalad_catalog/tests/data/catalog_metadata_invalid.json
 datalad_catalog/tests/data/catalog_metadata_valid.json
 datalad_catalog/tests/data/metadata_bids_dataset.json
 datalad_catalog/tests/data/metadata_bids_dataset.jsonl
 datalad_catalog/tests/data/metadata_bids_dataset2.json
 datalad_catalog/tests/data/metadata_bids_dataset2.jsonl
 datalad_catalog/tests/data/metadata_core.json
 datalad_catalog/tests/data/metadata_core.jsonl
 datalad_catalog/tests/data/metadata_core_dataset.json
 datalad_catalog/tests/data/metadata_datacite_gin.json
 datalad_catalog/tests/data/metadata_datacite_gin.jsonl
-datalad_catalog/tests/data/metadata_datacite_gin2.jsonl
 datalad_catalog/tests/data/metadata_studyminimeta.json
 datalad_catalog/tests/data/metadata_studyminimeta.jsonl
-datalad_catalog/tests/data/metadata_translate_nonsense.jsonl
-datalad_catalog/tests/data/metadata_translate_wrongname.jsonl
-datalad_catalog/tests/data/metadata_translate_wrongversion.jsonl
 datalad_catalog/tests/data/test_config_file.json
 datalad_catalog/tests/data/test_config_file.yml
-datalad_catalog/tests/data/test_config_file_catalog.json
-datalad_catalog/tests/data/test_config_file_dataset.json
-datalad_catalog/tests/data/test_config_file_workflow.json
 datalad_catalog/tests/data/workflow_generated_meta_dir.json
 datalad_catalog/tests/data/workflow_generated_meta_sub.json
 datalad_catalog/tests/data/workflow_generated_meta_super.json
-datalad_catalog/translators/__init__.py
-datalad_catalog/translators/bids_dataset_translator.py
-datalad_catalog/translators/datacite_gin_translator.py
-datalad_catalog/translators/metalad_core_translator.py
-datalad_catalog/translators/metalad_studyminimeta_translator.py
 docs/Makefile
-docs/source/catalog_config.rst
 docs/source/catalog_schema.rst
 docs/source/changelog.rst
 docs/source/command_line_reference.rst
 docs/source/conf.py
 docs/source/contributing.rst
 docs/source/index.rst
 docs/source/installation.rst
 docs/source/metadata_formats.rst
 docs/source/overview.rst
 docs/source/pipeline_description.rst
 docs/source/python_module_reference.rst
-docs/source/resources.rst
 docs/source/usage.rst
 docs/source/_static/catalog_screenshot.png
 docs/source/_static/datacat0_hero.svg
 docs/source/_static/datacat0_hero_lightbg.svg
 docs/source/_static/datacat1_the_challenge.svg
 docs/source/_static/datacat2_the_opportunity.svg
 docs/source/_static/datacat3_the_toolset.svg
```

### Comparing `datalad_catalog-0.2.1b0/docs/Makefile` & `datalad_catalog-0.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.1b0/docs/source/_static/catalog_screenshot.png` & `datalad_catalog-0.2.2/docs/source/_static/catalog_screenshot.png`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.1b0/docs/source/_static/datacat0_hero.svg` & `datalad_catalog-0.2.2/docs/source/_static/datacat0_hero.svg`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.1b0/docs/source/_static/datacat0_hero_lightbg.svg` & `datalad_catalog-0.2.2/docs/source/_static/datacat0_hero_lightbg.svg`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.1b0/docs/source/_static/datacat1_the_challenge.svg` & `datalad_catalog-0.2.2/docs/source/_static/datacat1_the_challenge.svg`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.1b0/docs/source/_static/datacat2_the_opportunity.svg` & `datalad_catalog-0.2.2/docs/source/_static/datacat2_the_opportunity.svg`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.1b0/docs/source/_static/datacat3_the_toolset.svg` & `datalad_catalog-0.2.2/docs/source/_static/datacat3_the_toolset.svg`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.1b0/docs/source/_static/datacat3_the_toolset_lightbg.svg` & `datalad_catalog-0.2.2/docs/source/_static/datacat3_the_toolset_lightbg.svg`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.1b0/docs/source/_static/datacat4_the_catalog.svg` & `datalad_catalog-0.2.2/docs/source/_static/datacat4_the_catalog.svg`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.1b0/docs/source/_static/datacat4_the_catalog_lightbg.svg` & `datalad_catalog-0.2.2/docs/source/_static/datacat4_the_catalog_lightbg.svg`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.1b0/docs/source/_static/datacat_logo.svg` & `datalad_catalog-0.2.2/docs/source/_static/datacat_logo.svg`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.1b0/docs/source/_static/datalad_catalog_demo.svg` & `datalad_catalog-0.2.2/docs/source/_static/datalad_catalog_demo.svg`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.1b0/docs/source/_static/datalad_catalog_functionality.svg` & `datalad_catalog-0.2.2/docs/source/_static/datalad_catalog_functionality.svg`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.1b0/docs/source/_static/datalad_catalog_logo_1_dark.svg` & `datalad_catalog-0.2.2/docs/source/_static/datalad_catalog_logo_1_dark.svg`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.1b0/docs/source/_static/datalad_logo.png` & `datalad_catalog-0.2.2/docs/source/_static/datalad_logo.png`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.1b0/docs/source/catalog_schema.rst` & `datalad_catalog-0.2.2/docs/source/catalog_schema.rst`

 * *Files 12% similar despite different names*

```diff
@@ -6,22 +6,23 @@
 
 Source files defining the catalog's schema can be found here:
 
 - `catalog`_
 - `dataset`_
 - `file`_
 - `authors`_
-- `metadata_sources`_
+- `extractors`_
 
 
 A rendering of the schema can be accessed at:
 https://datalad.github.io/datalad-catalog/display_schema.html
 
 
+
 .. _draft 2020-12: https://json-schema.org/specification.html
 .. _JSON Schema: https://json-schema.org/
 .. _schema: https://datalad.github.io/datalad-catalog/display_schema
 .. _catalog: https://raw.githubusercontent.com/datalad/datalad-catalog/main/datalad_catalog/schema/jsonschema_catalog.json
 .. _dataset: https://raw.githubusercontent.com/datalad/datalad-catalog/main/datalad_catalog/schema/jsonschema_dataset.json
 .. _file: https://raw.githubusercontent.com/datalad/datalad-catalog/main/datalad_catalog/schema/jsonschema_file.json
 .. _authors: https://raw.githubusercontent.com/datalad/datalad-catalog/main/datalad_catalog/schema/jsonschema_authors.json
-.. _metadata_sources: https://raw.githubusercontent.com/datalad/datalad-catalog/main/datalad_catalog/schema/jsonschema_metadata_sources.json
+.. _extractors: https://raw.githubusercontent.com/datalad/datalad-catalog/main/datalad_catalog/schema/jsonschema_extractors.json
```

### Comparing `datalad_catalog-0.2.1b0/docs/source/conf.py` & `datalad_catalog-0.2.2/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,15 @@
 # The name of the Pygments (syntax highlighting) style to use.
 pygments_style = 'sphinx'
 
 # If true, `todo` and `todoList` produce output, else they produce nothing.
 todo_include_todos = True
 
 # Example configuration for intersphinx: refer to the Python standard library.
-intersphinx_mapping = {'https://docs.python.org/': None}
+intersphinx_mapping = {'python': ('https://docs.python.org/3', None)}
 
 # -- Options for HTML output ----------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 html_theme = 'sphinx_rtd_theme'
```

### Comparing `datalad_catalog-0.2.1b0/docs/source/index.rst` & `datalad_catalog-0.2.2/docs/source/index.rst`

 * *Files 10% similar despite different names*

```diff
@@ -39,16 +39,14 @@
 
    overview
    installation
    usage
    pipeline_description
    metadata_formats
    catalog_schema
-   catalog_config
-   resources
    contributing
    command_line_reference
    python_module_reference
    changelog
```

### Comparing `datalad_catalog-0.2.1b0/docs/source/installation.rst` & `datalad_catalog-0.2.2/docs/source/installation.rst`

 * *Files 6% similar despite different names*

```diff
@@ -68,19 +68,14 @@
 
 Similarly, the metadata input to ``datalad-catalog`` can come from any source as
 long as it conforms to the catalog schema. While the catalog does not expect
 metadata originating only from ``datalad-metalad``'s extractors, this tool has
 advanced metadata handling capabilities that will integrate seamlessly with
 DataLad datasets and the catalog generation process.
 
-In order to translate metadata extracted using ``datalad-metalad`` into the
-catalog schema, ``datalad-catalog`` provides translation modules that are
-dependent on `jq`_.
-
 .. _datalad: https://github.com/datalad/datalad
 .. _GitHub: https://github.com/datalad/datalad-catalog
 .. _datalad-metalad: https://github.com/datalad/datalad-metalad
 .. _DataLad Handbook: https://handbook.datalad.org/en/latest/intro/installation.html
-.. _jq: https://stedolan.github.io/jq/
 .. _miniconda: https://docs.conda.io/en/latest/miniconda.html
 .. _PyPI: https://pypi.org/project/datalad-catalog/
 .. _venv: https://github.com/pypa/virtualenv
```

### Comparing `datalad_catalog-0.2.1b0/docs/source/overview.rst` & `datalad_catalog-0.2.2/docs/source/overview.rst`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.1b0/docs/source/pipeline_description.rst` & `datalad_catalog-0.2.2/docs/source/pipeline_description.rst`

 * *Files 8% similar despite different names*

```diff
@@ -52,28 +52,28 @@
 
 Step 2 - Add metadata
 ---------------------
 
 In order to extract arbitrary structured metadata from a DataLad dataset,
 this information first has to be added explicitly to the dataset. It can
 be added in your preferred location in the dataset tree. For example, here
-we add a ``.studyminimeta.yaml`` file to the root directory of the dataset:
+we add a ``studyminimeta.yaml`` file to the root directory of the dataset:
 
 .. code-block:: bash
    
     cd mydataset
     mv [path/to/studyminimeta.yaml] .
 
 Once the dataset has been updated with metadata, it has to be saved:
 
 .. code-block:: bash
    
     datalad save -m "add metadata to mydataset"
 
-Various metadata formats can be recognized by DataLad MetaLad's extraction process.
+Various metadata formats are recognized by DataLad MetaLad's extractors.
 See :doc:`metadata_formats` for an overview and `DataLad Metalad`_'s
 documentation for more detail.
 
 
 Step 3 - Extract metadata
 -------------------------
 
@@ -104,53 +104,57 @@
 
 .. code-block:: bash
 
     #!/bin/zsh
     DATASET_PATH="path/to/mydataset"
     PIPELINE_PATH="path/to/extract_dataset_pipeline.json"
     datalad meta-conduct "$PIPELINE_PATH" \
-        traverser.top_level_dir=$DATASET_PATH \
-        traverser.item_type=dataset \
-        traverser.traverse_sub_datasets=True \
-        extractor1.extractor_type=dataset \
-        extractor1.extractor_name=metalad_core \
-        extractor2.extractor_type=dataset \
-        extractor2.extractor_name=metalad_studyminimeta \
-        adder.aggregate=True
+        traverser:"$DATASET_PATH" \
+        traverser:dataset \
+        traverser:True \
+        extractor1:Dataset \
+        extractor1:metalad_core \
+        extractor2:Dataset \
+        extractor2:metalad_studyminimeta \
+        adder:True
 
 where the pipeline in ``path/to/extract_dataset_pipeline.json``
 looks like this:
 
 .. code-block:: json
 
     {
       "provider": {
-        "module": "datalad_metalad.pipeline.provider.datasettraverse",
+        "module": "datalad_metalad.provider.datasettraverse",
         "class": "DatasetTraverser",
         "name": "traverser",
-        "arguments": {}  
+        "arguments": [],
+        "keyword_arguments": {}
       },
       "processors": [
         {
-          "module": "datalad_metalad.pipeline.processor.extract",
+          "module": "datalad_metalad.processor.extract",
           "class": "MetadataExtractor",
           "name": "extractor1",
-          "arguments": {}    
+          "arguments": [],
+          "keyword_arguments": {}
         },
         {
-          "module": "datalad_metalad.pipeline.processor.extract",
+          "module": "datalad_metalad.processor.extract",
           "class": "MetadataExtractor",
           "name": "extractor2",
-          "arguments": {}    
+          "arguments": [],
+          "keyword_arguments": {}
         },
         {
           "name": "adder",
-          "module": "datalad_metalad.pipeline.processor.add",
+          "module": "datalad_metalad.processor.add",
           "class": "MetadataAdder",
-          "arguments": {}    
+          "arguments": [],
+          "keyword_arguments": {}
         }
       ]
     }
 
 Dump and write to disk:
 
 .. code-block:: bash
@@ -171,73 +175,55 @@
     DATASET_PATH="path/to/mydataset"
     PIPELINE_PATH="path/to/extract_file_pipeline.json"
     METADATA_OUT_PATH="path/to/file_metadata.json" # empty text file
     # Add starting array bracket
     echo "[" > "$METADATA_OUT_PATH"
     # Extract file-level metadata, add comma
     datalad -f json meta-conduct "$PIPELINE_PATH" \
-        traverser.top_level_dir=$DATASET_PATH \
-        traverser.item_type=file \
-        traverser.traverse_sub_datasets=True \
-        extractor.extractor_type=file \
-        extractor.extractor_name=metalad_core \
+        traverser:"$DATASET_PATH" \
+        traverser:file \
+        traverser:True \
+        extractor:File \
+        extractor:metalad_core \
         | jq '.["pipeline_element"]["result"]["metadata"][0]["metadata_record"]' \
         | jq -c . | sed 's/$/,/' >> "$METADATA_OUT_PATH"
     # Remove last comma
     sed -i '' '$ s/.$//' "$METADATA_OUT_PATH"
     # Add closing array bracket
     echo "]" >> "$METADATA_OUT_PATH"
 
 where the pipeline in ``path/to/extract_file_pipeline.json``
 looks like this:
 
-.. code-block:: javascript
+.. code-block:: json
 
     {
       "provider": {
-        "module": "datalad_metalad.pipeline.provider.datasettraverse",
+        "module": "datalad_metalad.provider.datasettraverse",
         "class": "DatasetTraverser",
         "name": "traverser",
-        "arguments": {}
+        "arguments": [],
+        "keyword_arguments": {}
       },
       "processors": [
         {
-          "module": "datalad_metalad.pipeline.processor.extract",
+          "module": "datalad_metalad.processor.extract",
           "class": "MetadataExtractor",
           "name": "extractor",
-          "arguments": {}
+          "arguments": [],
+          "keyword_arguments": {}
         }
       ]
     }
 
 At the end of this process, you have two files with structured metadata that
-can eventually be provided to ``datalad-catalog`` in order to generate the catalog
-and its entries.
-
-
-Step 4 - Translate the metadata
--------------------------------
+can be given as arguments to DataLad Catalog in order to generate the catalog.
 
-Before the extracted metadata can be provided to ``datalad-catalog``, it needs to be
-in a format/structure that will validate successfully against the catalog schema.
-Extracted metadata will typically be structured according to whatever schema was
-specified by the extractor, and information in such a schema will have to be translated
-to the catalog schema. For this purpose, ``datalad-catalog`` provides a ``translate``
-mechanism together with dedicated translators for specific metadata extractors.
-See :doc:`metadata_formats` and the :doc:`usage` instructions for more information.
 
-To translate the extracted metadata, we do the following:
-
-.. code-block:: bash
-   
-    datalad catalog translate -m [path/to/dataset_metadata.json] > [path/to/translated_dataset_metadata.json]
-    datalad catalog translate -m [path/to/file_metadata.json] > [path/to/translated_file_metadata.json]
-
-
-Step 5 - Run DataLad Catalog
+Step 4 - Run DataLad Catalog
 ----------------------------
 
 .. note:: Detailed usage instructions for DataLad Catalog can be viewed in
     :doc:`usage` and :doc:`command_line_reference`.
 
 The important subcommands for generating a catalog are:
 
@@ -246,28 +232,33 @@
 - ``add`` adds dataset and/or file level metadata to an existing catalog
 
 To create a catalog from the metadata we generated above, we can run the following:
 
 .. code-block:: bash
 
     #!/bin/zsh
-    TRANSLATED_DATASET_METADATA_OUT_PATH="path/to/translated_dataset_metadata.json"
-    TRANSLATED_FILE_METADATA_OUT_PATH="path/to/translated_file_metadata.json"
+    DATASET_METADATA_OUT_PATH="path/to/dataset_metadata.json"
+    FILE_METADATA_OUT_PATH="path/to/file_metadata.json"
     CATALOG_PATH="path/to/new/catalog"
-    datalad catalog create -c "$CATALOG_PATH" -m "$TRANSLATED_DATASET_METADATA_OUT_PATH"
-    datalad catalog add -c "$CATALOG_PATH" -m "$TRANSLATED_FILE_METADATA_OUT_PATH"
+    datalad catalog create -c "$CATALOG_PATH" -m "$DATASET_METADATA_OUT_PATH"
+    datalad catalog add -c "$CATALOG_PATH" -m "$FILE_METADATA_OUT_PATH"
+
+
+Step 5 - Deploy the catalog
+---------------------------
+
+.. admonition:: TODO
+    
+    - add/update content
 
 
-Step 6 - Next steps
--------------------
+Step 6 - Update the catalog
+---------------------------
 
-Congratulations! You now have a catalog with multiple entries!
+.. admonition:: TODO
+    
+    - add/update content
 
-This catalog can be served locally (``datalad catalog serve``) to view/test it, deployed
-to an open or/restricted cloud server in order to make it available to the public or 
-colleagues/collaborators (e.g. via GitHub Pages in the case of publicly available catalogs),
-and updated with new entries in future (with a ``datalad catalog add``).
 
-Happy cataloging!
 
 .. _DataLad Handbook: https://handbook.datalad.org/en/latest/basics/basics-datasets.html
 .. _DataLad Metalad: https://github.com/datalad/datalad-metalad
```

### Comparing `datalad_catalog-0.2.1b0/setup.cfg` & `datalad_catalog-0.2.2/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -11,46 +11,40 @@
 	License :: OSI Approved :: BSD License
 	Programming Language :: Python :: 3
 
 [options]
 python_requires = >= 3.7
 install_requires = 
 	datalad >= 0.17
-	datalad-metalad >= 0.4.6
+	datalad-metalad >= 0.4.1
 	jsonschema
 	pyyaml
 	jq;platform_system!='Windows'
 packages = find:
 include_package_data = True
 
 [options.package_data]
 * = catalog/*, catalog/artwork/*, catalog/assets/*, catalog/assets/favicon/*, catalog/metadata/*, catalog/templates/*, config/*, schema/*, tests/data/*
 
 [options.extras_require]
 devel = 
-	nose
 	coverage
 	pytest
 
 [options.packages.find]
 exclude = 
 	_datalad_buildsupport
 
 [options.entry_points]
 datalad.extensions = 
 	catalog = datalad_catalog:command_suite
 datalad.metadata.extractors = 
 	datacite_gin = datalad_catalog.extractors.datacite_gin:DataciteGINDatasetExtractor
 datalad.tests = 
 	catalog = datalad_catalog
-datalad.metadata.translators = 
-	datacite_gin_translator = datalad_catalog.translators.datacite_gin_translator:DataciteGINTranslator
-	bids_dataset_translator = datalad_catalog.translators.bids_dataset_translator:BIDSDatasetTranslator
-	metalad_core_translator = datalad_catalog.translators.metalad_core_translator:MetaladCoreTranslator
-	metalad_studyminimeta_translator = datalad_catalog.translators.metalad_studyminimeta_translator:MetaladStudyminimetaTranslator
 
 [versioneer]
 VCS = git
 style = pep440
 versionfile_source = datalad_catalog/_version.py
 versionfile_build = datalad_catalog/_version.py
 tag_prefix =
```

### Comparing `datalad_catalog-0.2.1b0/versioneer.py` & `datalad_catalog-0.2.2/versioneer.py`

 * *Files identical despite different names*

