# Comparing `tmp/kiara_plugin.streamlit-0.4.1.tar.gz` & `tmp/kiara_plugin.streamlit-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiara_plugin.streamlit-0.4.1.tar", last modified: Mon Feb 13 21:05:27 2023, max compression
+gzip compressed data, was "kiara_plugin.streamlit-0.4.2.tar", last modified: Fri Jun 23 10:09:52 2023, max compression
```

## Comparing `kiara_plugin.streamlit-0.4.1.tar` & `kiara_plugin.streamlit-0.4.2.tar`

### file list

```diff
@@ -1,143 +1,151 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 21:05:27.264623 kiara_plugin.streamlit-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/.envrc.disabled
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 21:05:27.240623 kiara_plugin.streamlit-0.4.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 21:05:27.244623 kiara_plugin.streamlit-0.4.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/.github/ISSUE_TEMPLATE/suggest-a-module.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 21:05:27.244623 kiara_plugin.streamlit-0.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/.github/workflows/build-darwin.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7473 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/.github/workflows/build-linux.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/.github/workflows/build-windows.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5860 2023-02-13 21:05:27.264623 kiara_plugin.streamlit-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 21:05:27.244623 kiara_plugin.streamlit-0.4.1/apps/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/apps/components.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/apps/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 21:05:27.244623 kiara_plugin.streamlit-0.4.1/apps/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/apps/pipelines/components_doc_onboarding.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/apps/pipelines/operations_doc_onboarding.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 21:05:27.240623 kiara_plugin.streamlit-0.4.1/ci/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 21:05:27.244623 kiara_plugin.streamlit-0.4.1/ci/conda/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/ci/conda/conda-pkg-patch.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/commitlint.config.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 21:05:27.244623 kiara_plugin.streamlit-0.4.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/docs/SUMMARY.md
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/docs/development.md
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 21:05:27.244623 kiara_plugin.streamlit-0.4.1/docs/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/docs/stylesheets/extra.css
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 21:05:27.240623 kiara_plugin.streamlit-0.4.1/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 21:05:27.244623 kiara_plugin.streamlit-0.4.1/examples/data/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/examples/data/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 21:05:27.244623 kiara_plugin.streamlit-0.4.1/examples/data/journals/
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/examples/data/journals/JournalEdges1902.csv
--rw-r--r--   0 runner    (1001) docker     (123)    33398 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/examples/data/journals/JournalNodes1902.csv
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/examples/data/journals/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 21:05:27.248623 kiara_plugin.streamlit-0.4.1/examples/streamlit/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/examples/streamlit/example.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/examples/streamlit/help.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/examples/streamlit/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 21:05:27.248623 kiara_plugin.streamlit-0.4.1/examples/streamlit/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/examples/streamlit/pipelines/example.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/examples/streamlit/pipelines/topic_modeling.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/examples/streamlit/workflow_dynamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6222 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/examples/streamlit/workflow_static.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/examples/streamlit/workflows.py
--rw-r--r--   0 runner    (1001) docker     (123)     7482 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/examples/streamlit/workshop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 21:05:27.240623 kiara_plugin.streamlit-0.4.1/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 21:05:27.248623 kiara_plugin.streamlit-0.4.1/scripts/documentation/
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/scripts/documentation/gen_api_doc_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/scripts/documentation/gen_info_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/scripts/documentation/gen_module_doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-02-13 21:05:27.264623 kiara_plugin.streamlit-0.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 21:05:27.240623 kiara_plugin.streamlit-0.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 21:05:27.240623 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 21:05:27.252623 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 21:05:27.252623 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/components/
--rw-r--r--   0 runner    (1001) docker     (123)     7655 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 21:05:27.252623 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/components/context/
--rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/components/context/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 21:05:27.252623 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/components/info/
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/components/info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/components/info/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/components/info/components.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 21:05:27.256623 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/components/input/
--rw-r--r--   0 runner    (1001) docker     (123)     9272 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/components/input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/components/input/assemblies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/components/input/container_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7005 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/components/input/scalars.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 21:05:27.256623 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/components/operations/
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/components/operations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 21:05:27.256623 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/components/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/components/pipelines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 21:05:27.256623 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/components/preview/
--rw-r--r--   0 runner    (1001) docker     (123)     7566 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/components/preview/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/components/preview/assemblies.py
--rw-r--r--   0 runner    (1001) docker     (123)     5864 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/components/preview/core_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/components/preview/network_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/components/preview/tabular.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 21:05:27.256623 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/components/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/components/workflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 21:05:27.256623 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/components/workflow/dynamic/
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/components/workflow/dynamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11223 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/components/workflow/dynamic/components.py
--rw-r--r--   0 runner    (1001) docker     (123)    11896 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/components/workflow/dynamic/workflow_page.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 21:05:27.260623 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/components/workflow/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/components/workflow/requirements/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 21:05:27.260623 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/components/workflow/static/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/components/workflow/static/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/components/workflow/static/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/components/workflow/static/workflow_page.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 21:05:27.260623 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 21:05:27.260623 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/interfaces/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/interfaces/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/interfaces/cli/streamlit.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 21:05:27.260623 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 21:05:27.260623 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/pipelines/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 21:05:27.260623 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/renderers/
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/renderers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 21:05:27.260623 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/resources/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 21:05:27.240623 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/resources/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 21:05:27.260623 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/resources/templates/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/resources/templates/pipeline/streamlit_app.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)    10231 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/streamlit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 21:05:27.264623 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/utils/class_loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/utils/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/utils/monkey_patches.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 21:05:27.252623 kiara_plugin.streamlit-0.4.1/src/kiara_plugin.streamlit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5860 2023-02-13 21:05:27.000000 kiara_plugin.streamlit-0.4.1/src/kiara_plugin.streamlit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-02-13 21:05:27.000000 kiara_plugin.streamlit-0.4.1/src/kiara_plugin.streamlit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 21:05:27.000000 kiara_plugin.streamlit-0.4.1/src/kiara_plugin.streamlit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-02-13 21:05:27.000000 kiara_plugin.streamlit-0.4.1/src/kiara_plugin.streamlit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 21:04:28.000000 kiara_plugin.streamlit-0.4.1/src/kiara_plugin.streamlit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-02-13 21:05:27.000000 kiara_plugin.streamlit-0.4.1/src/kiara_plugin.streamlit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-13 21:05:27.000000 kiara_plugin.streamlit-0.4.1/src/kiara_plugin.streamlit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 21:05:27.264623 kiara_plugin.streamlit-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/tests/conftest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      233 2023-02-13 21:04:20.000000 kiara_plugin.streamlit-0.4.1/tests/test_kiara_modules_default.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.744479 kiara_plugin.streamlit-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/.envrc.disabled
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.720479 kiara_plugin.streamlit-0.4.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.728479 kiara_plugin.streamlit-0.4.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/.github/ISSUE_TEMPLATE/suggest-a-module.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.732479 kiara_plugin.streamlit-0.4.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/.github/workflows/build-darwin.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/.github/workflows/build-linux.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/.github/workflows/build-windows.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-06-23 10:09:52.744479 kiara_plugin.streamlit-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.732479 kiara_plugin.streamlit-0.4.2/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/apps/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/apps/operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.732479 kiara_plugin.streamlit-0.4.2/apps/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/apps/pipelines/components_doc_onboarding.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/apps/pipelines/operations_doc_onboarding.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.720479 kiara_plugin.streamlit-0.4.2/ci/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.732479 kiara_plugin.streamlit-0.4.2/ci/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/ci/conda/conda-pkg-patch.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/commitlint.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.732479 kiara_plugin.streamlit-0.4.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/docs/SUMMARY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/docs/development.md
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.732479 kiara_plugin.streamlit-0.4.2/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/docs/stylesheets/extra.css
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.724479 kiara_plugin.streamlit-0.4.2/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.732479 kiara_plugin.streamlit-0.4.2/examples/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/examples/data/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.732479 kiara_plugin.streamlit-0.4.2/examples/data/journals/
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/examples/data/journals/JournalEdges1902.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    33398 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/examples/data/journals/JournalNodes1902.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/examples/data/journals/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.732479 kiara_plugin.streamlit-0.4.2/examples/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/examples/jobs/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.732479 kiara_plugin.streamlit-0.4.2/examples/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/examples/pipelines/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.736479 kiara_plugin.streamlit-0.4.2/examples/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/examples/streamlit/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/examples/streamlit/help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/examples/streamlit/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.736479 kiara_plugin.streamlit-0.4.2/examples/streamlit/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/examples/streamlit/pipelines/example.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/examples/streamlit/pipelines/topic_modeling.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/examples/streamlit/step_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/examples/streamlit/workflow_dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/examples/streamlit/workflow_static.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/examples/streamlit/workflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7482 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/examples/streamlit/workshop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.724479 kiara_plugin.streamlit-0.4.2/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.736479 kiara_plugin.streamlit-0.4.2/scripts/documentation/
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/scripts/documentation/gen_api_doc_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/scripts/documentation/gen_info_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/scripts/documentation/gen_module_doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-06-23 10:09:52.748479 kiara_plugin.streamlit-0.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.724479 kiara_plugin.streamlit-0.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.724479 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.736479 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.736479 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     7654 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.736479 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/context/
+-rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/context/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.740479 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/info/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5489 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/info/components.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.740479 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/input/
+-rw-r--r--   0 runner    (1001) docker     (123)     9266 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8539 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/input/assemblies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/input/container_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7004 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/input/scalars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.740479 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/operations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.740479 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/pipelines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.740479 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/preview/
+-rw-r--r--   0 runner    (1001) docker     (123)     7566 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/preview/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/preview/assemblies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/preview/core_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/preview/network_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/preview/tabular.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.740479 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/workflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.740479 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/workflow/dynamic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/workflow/dynamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11223 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/workflow/dynamic/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11895 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/workflow/dynamic/workflow_page.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.740479 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/workflow/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/workflow/requirements/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.744479 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/workflow/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/workflow/static/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/workflow/static/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/workflow/static/workflow_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.744479 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.744479 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/interfaces/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/interfaces/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/interfaces/cli/streamlit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.744479 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.744479 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/pipelines/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.744479 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/renderers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/renderers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.744479 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/resources/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.724479 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/resources/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.744479 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/resources/templates/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/resources/templates/pipeline/streamlit_app.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)    10206 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/streamlit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.744479 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/utils/class_loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/utils/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/utils/monkey_patches.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.736479 kiara_plugin.streamlit-0.4.2/src/kiara_plugin.streamlit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-06-23 10:09:52.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin.streamlit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-06-23 10:09:52.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin.streamlit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 10:09:52.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin.streamlit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-23 10:09:52.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin.streamlit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 10:08:42.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin.streamlit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-23 10:09:52.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin.streamlit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-23 10:09:52.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin.streamlit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.744479 kiara_plugin.streamlit-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.744479 kiara_plugin.streamlit-0.4.2/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/tests/resources/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/tests/test_job_descs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      233 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/tests/test_kiara_modules_default.py
```

### Comparing `kiara_plugin.streamlit-0.4.1/.cruft.json` & `kiara_plugin.streamlit-0.4.2/.cruft.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'commit'": "'f30a92644095dd13556ab071b97d20008badaed3'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "checkout": null,
-    "commit": "b9f3af819a31735ed09c6b9cc605c12486bcfcd9",
+    "commit": "f30a92644095dd13556ab071b97d20008badaed3",
     "context": {
         "cookiecutter": {
             "_template": "https://github.com/DHARPA-Project/kiara_plugin.develop.git",
             "anaconda_user": "dharpa",
             "email": "markus@frkl.io",
             "full_name": "Markus Binsteiner",
             "github_user": "DHARPA-Project",
```

### Comparing `kiara_plugin.streamlit-0.4.1/.github/ISSUE_TEMPLATE/bug_report.md` & `kiara_plugin.streamlit-0.4.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.1/.github/ISSUE_TEMPLATE/suggest-a-module.md` & `kiara_plugin.streamlit-0.4.2/.github/ISSUE_TEMPLATE/suggest-a-module.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.1/.github/workflows/build-darwin.yaml` & `kiara_plugin.streamlit-0.4.2/.github/workflows/build-darwin.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.1/.github/workflows/build-linux.yaml` & `kiara_plugin.streamlit-0.4.2/.github/workflows/build-linux.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -22,90 +22,95 @@
     steps:
       - name: "Set up Python ${{ matrix.python_version }}"
         uses: actions/setup-python@v4
         with:
           python-version: "${{ matrix.python_version }}"
       - uses: actions/checkout@v3
       - name: install kiara_plugin.streamlit
-        run: pip install -U --extra-index-url https://pypi.fury.io/dharpa/ .[all,dev_testing]
+        run: pip install -U .[all,dev_testing]
       - name: display installed kiara and module package versions
         run: pip list | grep kiara
       - name: Test with pytest
         run: make test
 
-# Uncomment this if you have coveralls.io setup with this repo
 #  coverage:
 #    name: create and publish test coverage
 #    runs-on: ubuntu-latest
 #    steps:
 #      - name: "Set up Python 3.9"
 #        uses: actions/setup-python@v4
 #        with:
 #          python-version: "3.9"
 #      - uses: actions/checkout@v3
 #      - name: install kiara
-#        run: pip install -U --extra-index-url https://pypi.fury.io/dharpa/ .[all,dev_testing]
+#        run: pip install -U .[all,dev_testing]
 #      - name: display installed kiara and module package versions
 #        run: pip list | grep kiara
 #      - name: Run coverage
 #        run: coverage run -m pytest tests
-#      - name: Upload coverage data to coveralls.io
-#        run: coveralls --service=github
-#        env:
-#          GITHUB_TOKEN:  ${{ secrets.GITHUB_TOKEN }}""
+#      - name: coverallsUpload coverage data to coveralls.io
+#        uses: coverallsapp/github-action@v2
 
   mypy-linux:
     name: mypy check on linux
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python_version: ["3.8", "3.9", "3.10", "3.11"]
     steps:
       - name: "Set up Python ${{ matrix.python_version }}"
         uses: actions/setup-python@v4
         with:
           python-version: "${{ matrix.python_version }}"
       - uses: actions/checkout@v3
       - name: install kiara_plugin.streamlit
-        run: pip install -U --extra-index-url https://pypi.fury.io/dharpa/ .[all,dev_testing]
+        run: pip install -U .[all,dev_testing]
       - name: Test with mypy
         run: make mypy
 
-  flake8-linux:
-    name: flake8 on linux
+  linting-linux:
     runs-on: ubuntu-latest
     steps:
-      - name: Set up Python 3.9
+      - uses: actions/checkout@v3
+      - name: Install Python
         uses: actions/setup-python@v4
         with:
-          python-version: "3.9"
-      - uses: actions/checkout@v3
-      - name: install kiara_plugin.streamlit
-        run: pip install -U --extra-index-url https://pypi.fury.io/dharpa/ .[all,dev_testing]
-      - name: Test with flake8
-        run: make flake
+          python-version: "3.11"
+      - name: pip cache
+        id: pip-cache
+        uses: actions/cache@v3
+        with:
+          path: ~/.cache/pip
+          key: ${{ runner.os }}-pip-${{ hashFiles('**/setup.*') }}
+      - name: Install dependencies
+        run: |
+          python -m pip install --upgrade pip
+          pip install ruff
+      # Include `--format=github` to enable automatic inline annotations.
+      - name: Run Ruff
+        run: ruff --format=github src/
 
   build-docs:
     name: build documentation
     if: ${{ github.ref == 'refs/heads/develop' }} || ${{ github.ref == 'refs/heads/main' }} || startsWith(github.ref, 'refs/tags/')
     runs-on: ubuntu-latest
     needs:
       - test-linux
       - mypy-linux
-      - flake8-linux
+      - linting-linux
     steps:
-      - name: Set up Python 3.9
+      - name: Set up Python 3.11
         uses: actions/setup-python@v4
         with:
-          python-version: "3.9"
+          python-version: "3.11"
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
       - name: install kiara_plugin.streamlit package
-        run: pip install -U --extra-index-url https://pypi.fury.io/dharpa/ .[all,dev_documentation]
+        run: pip install -U .[all,dev_documentation]
       - run: git config --global user.email "Markus Binsteiner"
       - run: git config --global user.name "markus@frkl.io"
       - name: create latest documentation
         if: ${{ ( github.ref == 'refs/heads/develop') }}
         run: FAIL_DOC_BUILD_ON_ERROR=true mike deploy --push latest && mike set-default --push latest
       - name: extract tag name
         run: echo "RELEASE_VERSION=${GITHUB_REF#refs/*/}" >> $GITHUB_ENV
@@ -116,29 +121,29 @@
   release_package:
     name: publish python package
     if: ${{ github.ref == 'refs/heads/develop' }} || ${{ github.ref == 'refs/heads/main' }} || startsWith(github.ref, 'refs/tags/')
     runs-on: ubuntu-latest
     needs:
       - test-linux
       - mypy-linux
-      - flake8-linux
+      - linting-linux
     env:
         GEMFURY_PUSH_TOKEN: ${{ secrets.GEMFURY_PUSH_TOKEN }}
     steps:
-      - name: Set up Python 3.9
+      - name: Set up Python 3.11
         uses: actions/setup-python@v4
         with:
-          python-version: "3.9"
+          python-version: "3.11"
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
       - name: install pip
         run: pip install pip==21.2.4 setuptools==57.4.0
       - name: install kiara
-        run: pip install -U --extra-index-url https://pypi.fury.io/dharpa/ -e .[all]
+        run: pip install -U -e .[all]
       - name: install 'build' package
         run: pip install -U build
       - name: create packages
         run: python -m build
       - name: upload source package
         run: curl -F package=@$(ls dist/kiara*.tar.gz) https://${GEMFURY_PUSH_TOKEN}@dharpa.fury.land:443/pypi/
       - name: upload wheel
@@ -152,31 +157,33 @@
 
   conda_package_build:
     name: conda package build (and upload if release)
     runs-on: ubuntu-latest
     needs:
       - test-linux
       - mypy-linux
-      - flake8-linux
+      - linting-linux
     steps:
       - name: "Set up Python 3.9"
         uses: actions/setup-python@v4
         with:
           python-version: "3.9"
       - name: pip cache
         id: pip-cache
         uses: actions/cache@v3
         with:
           path: ~/.cache/pip
           key: ${{ runner.os }}-pip-${{ hashFiles('**/setup.*') }}
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
+      - name: install kiara
+        run: pip install kiara
       - name: install required plugin packages
-        run: pip install -U --pre --extra-index-url https://pypi.fury.io/dharpa/ kiara_plugin.develop
+        run: pip install git+https://github.com/DHARPA-Project/kiara_plugin.develop.git@develop
       - name: build conda package
         if: ${{ ( github.ref == 'refs/heads/develop') }}
         run: kiara conda build-package --patch-data ci/conda/conda-pkg-patch.yaml .
       - name: extract tag name
         run: echo "RELEASE_VERSION=${GITHUB_REF#refs/*/}" >> $GITHUB_ENV
       - name: build & publish conda package
         if: ${{ startsWith(github.ref, 'refs/tags/') }}
@@ -185,15 +192,15 @@
   merge_tag_to_main:
     name: merge current tag to main branch
     runs-on: ubuntu-latest
     if: ${{ startsWith(github.ref, 'refs/tags') }}
     needs:
       - test-linux
       - mypy-linux
-      - flake8-linux
+      - linting-linux
     steps:
     - uses: actions/checkout@v3
       with:
         fetch-depth: 0
     - run: git config --global user.email "markus@frkl.io"
     - run: git config --global user.name "Markus Binsteiner"
     - name: extract tag name
```

### Comparing `kiara_plugin.streamlit-0.4.1/.github/workflows/build-windows.yaml` & `kiara_plugin.streamlit-0.4.2/.github/workflows/build-windows.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.1/.gitignore` & `kiara_plugin.streamlit-0.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.1/.pre-commit-config.yaml` & `kiara_plugin.streamlit-0.4.2/.pre-commit-config.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -6,47 +6,36 @@
 - repo: https://github.com/alessandrojcm/commitlint-pre-commit-hook
   rev: 'v9.3.0'
   hooks:
     - id: commitlint
       stages: [commit-msg]
       additional_dependencies: ['@commitlint/config-conventional']
 
-- repo: https://github.com/pycqa/isort
-  rev: 5.10.1
-  hooks:
-    - id: isort
-
 - repo: https://github.com/psf/black
-  rev: 22.10.0
+  rev: 22.12.0
   hooks:
     - id: black
 
-- repo: https://github.com/myint/autoflake
-  rev: 'v2.0.0'
-  hooks:
-    - id: autoflake
-      args: ['--in-place', '--remove-all-unused-imports']
-      # args: ['--in-place', '--remove-all-unused-imports', '--remove-unused-variable']
-
-- repo: https://github.com/PyCQA/flake8
-  rev: 5.0.4
-  hooks:
-    - id: flake8
-
 - repo: https://github.com/pre-commit/mirrors-mypy
   rev: 'v0.991'  # Use the sha / tag you want to point at
   hooks:
   - id: mypy
     files: "^src/"
     pass_filenames: true
     args: ["--config-file", "setup.cfg", "--ignore-missing-imports", "--explicit-package-bases"]
-    additional_dependencies: [pydantic>=1.8.0, rich>=10.0.0, ruamel.yaml, sqlalchemy-stubs, types-python-slugify, types-setuptools, types-python-dateutil]
+    additional_dependencies: [pydantic>=1.8.0, rich>=10.0.0, ruamel.yaml, anyio>=3.0.0, pyzmq>=22.0.3, bidict, sqlalchemy-stubs, types-python-slugify, types-setuptools, types-python-dateutil, dag_cbor, multiformats, textual, regex, types-pytz, types-orjson]
+
+- repo: https://github.com/charliermarsh/ruff-pre-commit
+  # Ruff version.
+  rev: 'v0.0.275'
+  hooks:
+    - id: ruff
 
 - repo: https://github.com/Kludex/no-optional
-  rev: 0.3.1
+  rev: 0.4.0
   hooks:
     - id: no_optional
 
 - repo: https://github.com/pre-commit/pre-commit-hooks
   rev: 'v4.3.0'
   hooks:
   - id: trailing-whitespace
```

### Comparing `kiara_plugin.streamlit-0.4.1/LICENSE` & `kiara_plugin.streamlit-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.1/Makefile` & `kiara_plugin.streamlit-0.4.2/Makefile`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.1/PKG-INFO` & `kiara_plugin.streamlit-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiara_plugin.streamlit
-Version: 0.4.1
+Version: 0.4.2
 Summary: Streamlit UI and widgets for kiara
 Author-email: Markus Binsteiner <markus@frkl.io>
 License: MPL-2.0
 Project-URL: homepage, https://github.com/DHARPA-Project/kiara_plugin.streamlit
 Project-URL: documentation, https://DHARPA-Project.github.io/kiara_plugin.streamlit
 Project-URL: repository, https://github.com/DHARPA-Project/kiara_plugin.streamlit
 Keywords: kiara,streamlit
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: workflow_app
 Provides-Extra: all_plugins
 Provides-Extra: dev_documentation
 Provides-Extra: dev_testing
 Provides-Extra: dev_utils
 Provides-Extra: dev_all
 License-File: LICENSE
 License-File: AUTHORS.md
```

### Comparing `kiara_plugin.streamlit-0.4.1/README.md` & `kiara_plugin.streamlit-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.1/apps/components.py` & `kiara_plugin.streamlit-0.4.2/apps/components.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.1/apps/operations.py` & `kiara_plugin.streamlit-0.4.2/apps/operations.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.1/apps/pipelines/components_doc_onboarding.yaml` & `kiara_plugin.streamlit-0.4.2/apps/pipelines/components_doc_onboarding.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.1/apps/pipelines/operations_doc_onboarding.yaml` & `kiara_plugin.streamlit-0.4.2/apps/pipelines/operations_doc_onboarding.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.1/docs/development.md` & `kiara_plugin.streamlit-0.4.2/docs/development.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.1/docs/index.md` & `kiara_plugin.streamlit-0.4.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.1/examples/data/journals/JournalEdges1902.csv` & `kiara_plugin.streamlit-0.4.2/examples/data/journals/JournalEdges1902.csv`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.1/examples/data/journals/JournalNodes1902.csv` & `kiara_plugin.streamlit-0.4.2/examples/data/journals/JournalNodes1902.csv`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.1/examples/streamlit/pipeline.py` & `kiara_plugin.streamlit-0.4.2/examples/streamlit/pipeline.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.1/examples/streamlit/pipelines/example.yaml` & `kiara_plugin.streamlit-0.4.2/examples/streamlit/pipelines/example.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.1/examples/streamlit/pipelines/topic_modeling.yaml` & `kiara_plugin.streamlit-0.4.2/examples/streamlit/pipelines/topic_modeling.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -3,22 +3,14 @@
 steps:
   - module_type: create.table.from.file_bundle
     step_id: create_text_corpus
   - module_type: table.pick.column
     step_id: extract_texts_column
     input_links:
       table: create_text_corpus.table
-  - module_type: table.pick.column
-    step_id: extract_filename_column
-    input_links:
-      table: create_text_corpus.table
-  - module_type: parse.date_array
-    step_id: create_date_array
-    input_links:
-      array: extract_filename_column.array
   - module_type: tokenize.texts_array
     step_id: tokenize_content
     input_links:
       texts_array: extract_texts_column.array
   - module_type: create.stopwords_list
     step_id: create_stopwords_list
   - module_type: preprocess.tokens_array
```

### Comparing `kiara_plugin.streamlit-0.4.1/examples/streamlit/workflow_dynamic.py` & `kiara_plugin.streamlit-0.4.2/examples/streamlit/workflow_dynamic.py`

 * *Files 24% similar despite different names*

```diff
@@ -18,14 +18,30 @@
 If you use any of those (preferable the nodes one), you can convert it into a table and once you do that you'll have access to the 'table-related' operations, like 'cut-column', or an sql-query one, which are at lest semi-useful for playing around with.
 
 As contrast, check out the pipeline auto-rendered UI example: https://kiara-static-workflow.streamlit.app/
 
 This has better usability by default for novice users, but obviously that would only work for one specific, pre-assembled scenario/pipeline, and there would be no freedom for the user to 'explore' on their own.
 
 Another thing I want to show in the future is the whole area of onboarding data into kiara, and making it usable and flexible enough to be useful. I think that's our biggest challenge, so I am still thinking about how to best do it.
+
+An example workflow, to create network_data from an edges file would be:
+
+- select `journal_edges_file` as the inital value -- this is the data we want to work with for this workflow
+- select `create_table.from.file` as the first operation -- this will convert the edges file into a table (with typed columns etc.) -- check out the 'Show operation details' to get information about the operation you selected.
+- check 'first_row_is_header', and click process
+- this module only has one output, so we can just select that using 'Select for next step'. This means that this result-dataset will be used as input for the next step
+- now the app will show you all available operations that take a 'table' as one of the inputs
+- maybe pick 'query.table' to run some sql against it:
+- set the query to `select * from data where weight > 1` and leave relation name to 'data'
+- click process
+- again, we only have one result, so we can just select that
+- now the app will show you the same operations as with the last step, since both values were of type `table`
+- select `assemble.network_data.from.tables` as the next operation
+- click the 'Preview' box above to see the table you are working with as input, select the inputs accordingly: 'Source', 'Target' (we don't need the 'id_column_name' in this particular instance because we don't hava a separate nodes table)
+- select the only result for the next step again, tihs is of type 'network_data'. We don't have many modules yet to work with 'network_data', but I hope you get the idea where this is going...
 """
 
 with st.expander("Notes (click to hide)", expanded=True):
     st.markdown(EXPLANATION)
 
 current = kst.api.get_current_context_name()
 with st.sidebar:
@@ -42,21 +58,21 @@
 
 if not st.kiara.api.list_alias_names():
     with st.spinner("Downloading example data ..."):
 
         result = st.kiara.api.run_job(
             operation="download.file",
             inputs={
-                "url": "https://github.com/DHARPA-Project/kiara.examples/raw/main/examples/data/journals/JournalNodes1902.csv"
+                "url": "https://github.com/DHARPA-Project/kiara.examples/raw/main/examples/data/network_analysis/journals/JournalNodes1902.csv"
             },
         )
         st.kiara.api.store_value(value=result["file"], alias="journal_nodes_file")
 
         result = st.kiara.api.run_job(
             operation="download.file",
             inputs={
-                "url": "https://github.com/DHARPA-Project/kiara.examples/raw/main/examples/data/journals/JournalEdges1902.csv"
+                "url": "https://github.com/DHARPA-Project/kiara.examples/raw/main/examples/data/network_analysis/journals/JournalEdges1902.csv"
             },
         )
         st.kiara.api.store_value(value=result["file"], alias="journal_edges_file")
 
 st.kiara.workflow(workflow_session)
```

### Comparing `kiara_plugin.streamlit-0.4.1/examples/streamlit/workflow_static.py` & `kiara_plugin.streamlit-0.4.2/examples/streamlit/workflow_static.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 import os
 
 import nltk
 import streamlit as st
-from kiara.interfaces.python_api import OperationInfo
 
 import kiara_plugin.streamlit as kiara_streamlit
+from kiara.interfaces.python_api import OperationInfo
 from kiara_plugin.streamlit.components.workflow.static import WorkflowSessionStatic
 
 st.set_page_config(layout="wide")
 
 nltk.download("punkt")
 nltk.download("stopwords")
 
@@ -36,27 +36,27 @@
 - Stage 1
 
    - Select the corpus (only 1 available for this demo, for now) -- this is basically just a folder with text files
    - languages and stopword lists are not supported yet, so just leave them as they are
 
 - Stage 2
 
-   - this needs to know the names of the columns where the required data is, you can look that up in the 'Outputs (previous stages)' expander, or just use: 'content' for `extract_texts_column__column_name` and 'file_name' for `extract_filename_column__column_name`
+   - this needs to know the names of the column where the required data is, you can look that up in the 'Outputs (previous stages)' expander, or just use: 'content' for `extract_texts_column__column_name`. A 'production' UI would give the user a combobox or similar with only the available column names here...
 
 - Stage 3
 
-   - this stage tokenizes the text content, and extracts a date column from the file name column. This is a bit difficult to do right now, because the date parser is not very good and needs the start and end position of the word it should parse (file name in our case): just use '11' for `create_date_array__min_index` and '21' for `create_date_array__max_index`
+   - this stage tokenizes the text content and also creates a list of stop words that will be used later in the pre-processing step. Just keep the `tokenize_by_word` input checked (unchecked would make sense for some asian languages), and maybe add 'italian' to the `languages` input. To test, you can also add some stopwords manually here.
 
 - Stage 4
 
-   - this stage pre-processes the tokens we computed in the previous stage, you can't do anything wrong. Just play a bit with the options and see how the result changes
+   - this stage pre-processes the tokens we computed in the previous stage, removes stopwords, etc. You can't do anything wrong. Just play a bit with the options and see how the result changes
 
 - Stage 5
 
-   - the final step, also nothing that can go wrong here. If you know about topic modeling, then the results will make sense, otherwise, probably not :)
+   - the final step, if you know about topic modeling, then the results will make sense, otherwise, probably not. Select to create a few topics (maybe `num_topics_min` 5 and num_topics_max 9), check `compute_coherence` and words_per_topic 3. Our production app would have a lot more explanations and documentation what any of the inputs and outputs mean, what exactly happens, what LDA is, etc.
 """
 with st.expander("Notes (click to hide)", expanded=True):
     st.markdown(EXPLANATION)
 
 
 current = kst.api.get_current_context_name()
 with st.sidebar:
@@ -79,15 +79,14 @@
     new_pipeline_info: OperationInfo = st.kiara.select_pipeline(
         filters=["topic_modeling"]
     )
     new_pipeline = new_pipeline_info.operation.operation_id
     st.session_state["selected_pipeline"] = new_pipeline
 
 # new_pipeline = "/home/markus/projects/kiara/kiara.examples/examples/pipelines/topic_modeling/topic_modeling.yaml"
-print(st.kiara.api.context.id)
 workflow_ref = "workflow_static"
 
 if workflow_ref not in st.session_state or context_changed or pipeline != new_pipeline:
     workflow = st.kiara.api.create_workflow(initial_pipeline=new_pipeline)
     workflow_session: WorkflowSessionStatic = WorkflowSessionStatic(workflow=workflow)
     st.session_state[workflow_ref] = workflow_session
 
@@ -96,31 +95,31 @@
 
 if "example_corpus" not in st.kiara.api.list_alias_names():
     with st.spinner("Downloading example data ..."):
 
         result = st.kiara.api.run_job(
             operation="download.file",
             inputs={
-                "url": "https://github.com/DHARPA-Project/kiara.examples/raw/main/examples/data/journals/JournalNodes1902.csv"
+                "url": "https://github.com/DHARPA-Project/kiara.examples/raw/main/examples/data/network_analysis/journals/JournalNodes1902.csv"
             },
         )
         st.kiara.api.store_value(value=result["file"], alias="journal_nodes_file")
 
         result = st.kiara.api.run_job(
             operation="download.file",
             inputs={
-                "url": "https://github.com/DHARPA-Project/kiara.examples/raw/main/examples/data/journals/JournalEdges1902.csv"
+                "url": "https://github.com/DHARPA-Project/kiara.examples/raw/main/examples/data/network_analysis/journals/JournalEdges1902.csv"
             },
         )
         st.kiara.api.store_value(value=result["file"], alias="journal_edges_file")
 
         result = st.kiara.api.run_job(
             operation="download.file_bundle",
             inputs={
                 "url": "https://github.com/DHARPA-Project/kiara.examples/archive/refs/heads/main.zip",
-                "sub_path": "kiara.examples-main/examples/data/text_corpus/data",
+                "sub_path": "kiara.examples-main/examples/data/language_processing/text_corpus/data",
             },
         )
         st.kiara.api.store_value(value=result["file_bundle"], alias="example_corpus")
 
 
 st.kiara.workflow(workflow_session)
```

### Comparing `kiara_plugin.streamlit-0.4.1/examples/streamlit/workflows.py` & `kiara_plugin.streamlit-0.4.2/examples/streamlit/workflows.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 import streamlit as st
-from kiara.api import KiaraAPI
 
 import kiara_plugin.streamlit as kst
+from kiara.api import KiaraAPI
 from kiara_plugin.streamlit.modules import DummyModuleConfig
 
 kst.init()
 
 st.write("Kiara example")
 
 api: KiaraAPI = st.kiara.api
```

### Comparing `kiara_plugin.streamlit-0.4.1/examples/streamlit/workshop.py` & `kiara_plugin.streamlit-0.4.2/examples/streamlit/workshop.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 import streamlit as st
-from kiara.api import KiaraAPI
 
 import kiara_plugin.streamlit as kst
+from kiara.api import KiaraAPI
 
 # st.set_page_config(layout="wide")
 
 # This example app introduces kiara, a data orchestration software. It will walk you through creating a simple streamilt application, and some basic but essential functions that can be built on in further notebooks.
 
 # first, we initialize the kiara streamlit integration
 # that way, we'll get access to the kiara api and some custom components
```

### Comparing `kiara_plugin.streamlit-0.4.1/mkdocs.yml` & `kiara_plugin.streamlit-0.4.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.1/scripts/documentation/gen_api_doc_pages.py` & `kiara_plugin.streamlit-0.4.2/scripts/documentation/gen_api_doc_pages.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.1/scripts/documentation/gen_info_pages.py` & `kiara_plugin.streamlit-0.4.2/scripts/documentation/gen_info_pages.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.1/scripts/documentation/gen_module_doc.py` & `kiara_plugin.streamlit-0.4.2/scripts/documentation/gen_module_doc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 import os
 
 import mkdocs_gen_files
+
 from kiara.context import Kiara
 
 kiara = Kiara.instance()
 
 modules_file_path = os.path.join("modules_list.md")
 modules_page_content = """# Available module types
```

### Comparing `kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/__init__.py` & `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,28 +12,27 @@
     find_data_types_under,
     find_kiara_model_classes_under,
     find_kiara_modules_under,
     find_kiara_renderers_under,
     find_pipeline_base_path_for_module,
 )
 
-# import kiara_plugin.streamlit.utils.monkey_patches  # noqa
+# import kiara_plugin.streamlit.utils.monkey_patches
 from kiara_plugin.streamlit.utils.class_loading import (
     find_kiara_streamlit_components_under,
 )
 
 if typing.TYPE_CHECKING:
     from kiara.context import KiaraContextConfig, KiaraRuntimeConfig
-
     from kiara_plugin.streamlit.streamlit import KiaraStreamlit
 
 
 __author__ = """Markus Binsteiner"""
 __email__ = "markus@frkl.io"
-warnings.simplefilter(action="ignore", category=FutureWarning)  # noqa
+warnings.simplefilter(action="ignore", category=FutureWarning)
 
 
 KIARA_METADATA = {
     "authors": [{"name": __author__, "email": __email__}],
     "description": "Kiara modules for: streamlit",
     "references": {
         "source_repo": {
@@ -104,22 +103,21 @@
 
 
 def init(
     context_config: Union[None, "KiaraContextConfig"] = None,
     runtime_config: Union[None, "KiaraRuntimeConfig"] = None,
 ) -> "KiaraStreamlit":
 
-    import streamlit as st
-
     import kiara_plugin.streamlit.utils.monkey_patches  # noqa
+    import streamlit as st
     from kiara_plugin.streamlit.streamlit import KiaraStreamlit
 
-    @st.experimental_singleton
+    @st.cache_resource
     def get_ktx() -> "KiaraStreamlit":
-        print("CREATE KIARA STREAMLIT")
+        # print("CREATE KIARA STREAMLIT")
         ktx = KiaraStreamlit(
             context_config=context_config, runtime_config=runtime_config
         )
         return ktx
 
     if not hasattr(st, "kiara"):
         ktx = get_ktx()
```

### Comparing `kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/components/__init__.py` & `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 # -*- coding: utf-8 -*-
 import abc
 import warnings
 from functools import partial
 from typing import Any, Callable, Dict, Generic, List, Type, TypeVar, Union
 
+from pydantic import BaseModel, Field
+from pydantic.fields import ModelField
+
 import streamlit as st
 from kiara.interfaces.python_api.models.info import InfoItemGroup, ItemInfo
 from kiara.models.documentation import (
     AuthorsMetadataModel,
     ContextMetadataModel,
     DocumentationMetadataModel,
 )
-from pydantic import BaseModel, Field
-from pydantic.fields import ModelField
-from streamlit.runtime.state import SessionStateProxy
-
 from kiara_plugin.streamlit.defaults import AUTO_GEN_MARKER
+from streamlit.runtime.state import SessionStateProxy
 
 with warnings.catch_warnings():
     pass
 
 from typing import TYPE_CHECKING
 
 from streamlit.delta_generator import DeltaGenerator
 
 if TYPE_CHECKING:
     from kiara.api import Kiara, KiaraAPI
-
     from kiara_plugin.streamlit.streamlit import KiaraStreamlit
 
 
 class ComponentOptions(BaseModel):
 
     key: str = Field(
         description="The (base) key to use for this component.", default=AUTO_GEN_MARKER
```

### Comparing `kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/components/context/__init__.py` & `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/context/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
-from typing import Any, Callable, List, Union
+from typing import Any, Callable, ClassVar, List, Union
 
 from pydantic import Field
-from streamlit.delta_generator import DeltaGenerator
 
 from kiara_plugin.streamlit.components import ComponentOptions, KiaraComponent
+from streamlit.delta_generator import DeltaGenerator
 
 
 class ContextSwitchOptions(ComponentOptions):
 
     allow_create: bool = Field(
         description="Allow the user to create a new context.", default=False
     )
@@ -23,15 +23,15 @@
     A *kiara* context is used to separate different sets of data and configuration, and is
     useful to keep datasets and processing results organized.
     """
 
     _options = ContextSwitchOptions
     _component_name = "context_switch_control"
 
-    _examples = [
+    _examples: ClassVar = [
         {
             "doc": "Show a context switch control.\n\nAllow the user to create a new context, and don't immediately switch to the selected context. You can compare the result of this component call with a call to `st.api.current_context_name`, to figure out whether the user wants to switch or not.",
             "args": {
                 "switch_to_selected": False,
                 "allow_create": True,
             },
         }
```

### Comparing `kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/components/info/__init__.py` & `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/info/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # -*- coding: utf-8 -*-
 import abc
 from typing import Generic, List, Mapping, Tuple, Type, TypeVar, Union
 
-from kiara.interfaces.python_api.models.info import ItemInfo
 from pydantic import Field
-from streamlit.delta_generator import DeltaGenerator
 
+from kiara.interfaces.python_api.models.info import ItemInfo
 from kiara_plugin.streamlit.components import ComponentOptions, KiaraComponent
 from kiara_plugin.streamlit.utils.components import create_list_component
+from streamlit.delta_generator import DeltaGenerator
 
 
 class InfoCompOptions(ComponentOptions):
     class Config:
         arbitrary_types_allowed = True
 
     columns: Union[
```

### Comparing `kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/components/info/api.py` & `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/info/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # -*- coding: utf-8 -*-
-from typing import Mapping, Type, Union
+from typing import ClassVar, Mapping, Type, Union
 
 from kiara.interfaces.python_api import OperationInfo
-from streamlit.delta_generator import DeltaGenerator
-
 from kiara_plugin.streamlit.components import ComponentOptions, KiaraComponent
 from kiara_plugin.streamlit.components.info import InfoCompOptions, KiaraInfoComponent
+from streamlit.delta_generator import DeltaGenerator
 
 # class KiaraApiHelpCompOptions(ComponentOptions):
 #     class Config:
 #         arbitrary_types_allowed = True
 #
 #     columns: Union[Tuple[int, int], Tuple[DeltaGenerator, DeltaGenerator]] = Field(
 #         description="The column layout to use for the next step.", default=(1, 4)
@@ -59,15 +58,15 @@
     """Displays information for all or a single operation.
 
     If you only provide a single item, documentation for this item will be shown. Otherwise, a list
     will be rendered on the left, and users can select one of the available items to get information for.
     """
 
     _component_name = "operation_info"
-    _examples = [
+    _examples: ClassVar = [
         {
             "doc": "Show information for the 'create.table.from.file' operation.",
             "args": {"items": "create.table.from.file"},
         },
         {"doc": "Show informations for all available operations.", "args": {}},
     ]
```

### Comparing `kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/components/info/components.py` & `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/info/components.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # -*- coding: utf-8 -*-
 from typing import Any, Dict, List, Mapping, Type
 
 from kiara.api import Value, ValueMap
 from kiara.models.documentation import DocumentationMetadataModel
-from streamlit.delta_generator import DeltaGenerator
-
 from kiara_plugin.streamlit.components import ComponentInfo, ComponentsInfo
 from kiara_plugin.streamlit.components.info import InfoCompOptions, KiaraInfoComponent
+from streamlit.delta_generator import DeltaGenerator
 
 
 class KiaraComponentInfoComponent(KiaraInfoComponent[ComponentInfo]):
     """Display information about a kiara streamlit component.
 
     This is used to create what you see here.
     """
```

### Comparing `kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/components/input/__init__.py` & `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/input/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # -*- coding: utf-8 -*-
 import abc
 import copy
 import uuid
 from typing import TYPE_CHECKING, Any, Callable, Iterable, List, Tuple, TypeVar, Union
 
+from pydantic import Field
+
 from kiara.api import Value, ValueSchema
 from kiara.defaults import SpecialValue
 from kiara.registries.data import ValueLink
-from pydantic import Field
-from streamlit.delta_generator import DeltaGenerator
-
 from kiara_plugin.streamlit.components import ComponentOptions, KiaraComponent
 from kiara_plugin.streamlit.defaults import NO_LABEL_MARKER, NO_VALUE_MARKER
+from streamlit.delta_generator import DeltaGenerator
 
 if TYPE_CHECKING:
     from kiara_plugin.streamlit.streamlit import KiaraStreamlit
 
 
 class InputOptions(ComponentOptions):
 
@@ -214,15 +214,15 @@
 
             def format_func(v: Any) -> str:
                 if v == NO_VALUE_MARKER:
                     return v
                 return f"{v} ({available_values[v].data_type_name})"
 
         if optional:
-            _item_options = [NO_VALUE_MARKER] + list(available_values.keys())
+            _item_options = [NO_VALUE_MARKER, *available_values.keys()]
             if not default:
                 default = NO_VALUE_MARKER
         else:
             _item_options = list(available_values.keys())
 
         with_preview = options.preview
```

### Comparing `kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/components/input/assemblies.py` & `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/input/assemblies.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # -*- coding: utf-8 -*-
 import abc
 import uuid
 from typing import Dict, Mapping, TypeVar, Union
 
+from pydantic import Field
+
 from kiara.api import ValueMap, ValueSchema
 from kiara.registries.data import ValueLink
 from kiara.utils.values import construct_valuemap
-from pydantic import Field
-from streamlit.delta_generator import DeltaGenerator
-
 from kiara_plugin.streamlit.components import ComponentOptions, KiaraComponent
 from kiara_plugin.streamlit.components.input import DefaultInputOptions, InputComponent
+from streamlit.delta_generator import DeltaGenerator
 
 
 class AssemblyOptions(ComponentOptions):
 
     max_columns: int = Field(
         description="The maximum number of columns to use for the assembly.", default=3
     )
@@ -65,19 +65,18 @@
         max_columns = options.max_columns
 
         if not fields:
             return construct_valuemap(kiara_api=self.api, values={})
 
         if not max_columns:
             num_columns = len(fields)
+        elif len(fields) >= max_columns:
+            num_columns = max_columns
         else:
-            if len(fields) >= max_columns:
-                num_columns = max_columns
-            else:
-                num_columns = len(fields)
+            num_columns = len(fields)
 
         columns = st.columns(num_columns)
         values: Dict[str, Union[None, ValueLink, str, uuid.UUID]] = {}
         for idx, field_name in enumerate(fields.keys()):
             schema = fields[field_name]
             help = None
             if schema.doc.is_set:
@@ -122,19 +121,18 @@
                 optional[input_name] = input_schema
 
         values = {}
         if required:
             req_expander = st.expander("Required inputs", expanded=True)
             if not max_columns:
                 num_columns = len(required)
+            elif len(required) >= max_columns:
+                num_columns = max_columns
             else:
-                if len(required) >= max_columns:
-                    num_columns = max_columns
-                else:
-                    num_columns = len(required)
+                num_columns = len(required)
 
             columns = req_expander.columns(num_columns)
             for idx, field_name in enumerate(required.keys()):
                 schema = required[field_name]
                 help = None
                 if schema.doc.is_set:
                     help = schema.doc.full_doc
@@ -156,19 +154,18 @@
                 values[field_name] = r
 
         if optional:
             opt_expander = st.expander("Optional inputs", expanded=optional_expanded)
 
             if not max_columns:
                 num_columns = len(optional)
+            elif len(optional) >= max_columns:
+                num_columns = max_columns
             else:
-                if len(optional) >= max_columns:
-                    num_columns = max_columns
-                else:
-                    num_columns = len(optional)
+                num_columns = len(optional)
 
             opt_columns = opt_expander.columns(num_columns)
 
             for idx, field_name in enumerate(optional.keys()):
                 schema = optional[field_name]
                 help = None
                 if schema.doc.is_set:
```

### Comparing `kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/components/input/container_types.py` & `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/input/container_types.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
-from streamlit.delta_generator import DeltaGenerator
 from streamlit_tags import st_tags
 
 from kiara_plugin.streamlit.components.input import InputComponent, InputOptions
+from streamlit.delta_generator import DeltaGenerator
 
 
 class ListInput(InputComponent):
     """Render a widget for input a list.
 
     Currently, only lists of strings are supported.
     """
```

### Comparing `kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/components/input/scalars.py` & `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/input/scalars.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # -*- coding: utf-8 -*-
 import abc
 from typing import Any
 
 from kiara.defaults import SpecialValue
-from streamlit.delta_generator import DeltaGenerator
-
 from kiara_plugin.streamlit.components.input import InputComponent, InputOptions
+from streamlit.delta_generator import DeltaGenerator
 
 
 class ScalarInput(InputComponent):
     @classmethod
     def get_default_label(cls) -> str:
         return "Provide value"
```

### Comparing `kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/components/operations/__init__.py` & `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/operations/__init__.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # -*- coding: utf-8 -*-
 from typing import Union
 
+from pydantic import Field, validator
+
 from kiara.api import ValueMap
 from kiara.exceptions import KiaraException
 from kiara.interfaces.python_api import OperationInfo
 from kiara.models.module.operation import Operation
-from pydantic import Field, validator
-from streamlit.delta_generator import DeltaGenerator
-
 from kiara_plugin.streamlit.components import ComponentOptions, KiaraComponent
+from streamlit.delta_generator import DeltaGenerator
 
 
 class OperationProcessOptions(ComponentOptions):
 
     operation_id: str = Field(description="The id of the operation to use.")
 
     @validator("operation_id")
```

### Comparing `kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/components/pipelines/__init__.py` & `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/pipelines/__init__.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # -*- coding: utf-8 -*-
 from typing import List, Literal, Union
 
 import networkx as nx
+from pydantic import Field
+
 from kiara.interfaces.python_api import OperationInfo
 from kiara.models.module.operation import Operation
 from kiara.models.module.pipeline import PipelineConfig
 from kiara.models.module.pipeline.pipeline import Pipeline
-from pydantic import Field
-from streamlit.delta_generator import DeltaGenerator
-
 from kiara_plugin.streamlit.components import ComponentOptions, KiaraComponent
+from streamlit.delta_generator import DeltaGenerator
 
 
 class PipelineSelectOptions(ComponentOptions):
     filters: List[str] = Field(
         description="Filter tokens that must be present in the pipeline/operation name.",
         default_factory=list,
     )
```

### Comparing `kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/components/preview/__init__.py` & `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/preview/__init__.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # -*- coding: utf-8 -*-
 import uuid
 from abc import abstractmethod
 from typing import List, Mapping, Union
 
-from kiara.api import Value, ValueMap
 from pydantic import Field
-from streamlit.delta_generator import DeltaGenerator
 
+from kiara.api import Value, ValueMap
 from kiara_plugin.streamlit.components import ComponentOptions, KiaraComponent
 from kiara_plugin.streamlit.utils.components import create_list_component
+from streamlit.delta_generator import DeltaGenerator
 
 
 class PreviewOptions(ComponentOptions):
 
     height: Union[int, None] = Field(
         description="The height of the preview.", default=None
     )
```

### Comparing `kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/components/preview/assemblies.py` & `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/preview/assemblies.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
 from typing import Mapping
 
-from kiara.api import ValueSchema
-from kiara.utils.output import create_dict_from_field_schemas
 from pydantic import Field
-from streamlit.delta_generator import DeltaGenerator
 
+from kiara.api import ValueSchema
+from kiara.utils.output import create_dict_from_field_schemas
 from kiara_plugin.streamlit.components import ComponentOptions, KiaraComponent
+from streamlit.delta_generator import DeltaGenerator
 
 
 class FieldsInfoOptions(ComponentOptions):
 
     fields: Mapping[str, ValueSchema] = Field(
         description="The fields and their schema."
     )
@@ -42,10 +42,10 @@
 
     def _render(self, st: DeltaGenerator, options: FieldsInfoOptions):
 
         import pandas as pd
 
         fields = options.fields
         fields_data = create_dict_from_field_schemas(fields)
-        df = pd.DataFrame(fields_data, columns=list(fields_data.keys()))
-        df.set_index("field_name", inplace=True)
-        st.table(df)
+        dataframe = pd.DataFrame(fields_data, columns=list(fields_data.keys()))
+        dataframe.set_index("field_name", inplace=True)  # noqa
+        st.table(dataframe)
```

### Comparing `kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/components/preview/core_types.py` & `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/preview/core_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 # -*- coding: utf-8 -*-
 from typing import Any, Dict
 
-from kiara.models.data_types import DictModel
+from kiara.models.data_types import KiaraDict
 from kiara.models.filesystem import FileBundle, FileModel
 from kiara.utils.json import orjson_dumps
-from kiara_plugin.core_types.models import ListModel
-from streamlit.delta_generator import DeltaGenerator
-
+from kiara_plugin.core_types.models import KiaraList
 from kiara_plugin.streamlit.components.preview import PreviewComponent, PreviewOptions
+from streamlit.delta_generator import DeltaGenerator
 
 
 class DictPreview(PreviewComponent):
     """Preview a value of type 'dict'."""
 
     _component_name = "preview_dict"
 
     @classmethod
     def get_data_type(cls) -> str:
         return "dict"
 
     def render_preview(self, st: DeltaGenerator, options: PreviewOptions) -> None:
 
         _value = self.api.get_value(options.value)
-        dict_data: DictModel = _value.data
+        dict_data: KiaraDict = _value.data
 
         data, schema = st.tabs(["Data", "Schema"])
 
         try:
             json_str = orjson_dumps(dict_data.dict_data)
         except Exception as e:
             json_str = f"Error parsing data: {e}"
@@ -34,30 +33,28 @@
 
         try:
             json_str = orjson_dumps(dict_data.data_schema)
         except Exception as e:
             json_str = f"Error parsing schema: {e}"
         schema.json(json_str)
 
-        return
-
 
 class ListPreview(PreviewComponent):
     """Preview a value of type 'list'."""
 
     _component_name = "preview_list"
 
     @classmethod
     def get_data_type(cls) -> str:
         return "list"
 
     def render_preview(self, st: DeltaGenerator, options: PreviewOptions) -> None:
 
         _value = self.api.get_value(options.value)
-        list_data: ListModel = _value.data
+        list_data: KiaraList = _value.data
 
         data, schema = st.tabs(["Data", "Schema"])
 
         try:
             json_str = orjson_dumps(list_data.list_data)
         except Exception as e:
             json_str = f"Error parsing data: {e}"
@@ -65,16 +62,14 @@
 
         try:
             json_str = orjson_dumps(list_data.item_schema)
         except Exception as e:
             json_str = f"Error parsing schema: {e}"
         schema.json(json_str)
 
-        return
-
 
 class FileBundlePreview(PreviewComponent):
     """Preview a value of type 'file_bundle'."""
 
     _component_name = "preview_file_bundle"
 
     @classmethod
@@ -90,16 +85,14 @@
         for file_path, file_info in bundle.included_files.items():
             table.setdefault("path", []).append(file_path)
             table.setdefault("size", []).append(file_info.size)
             table.setdefault("mime-type", []).append(file_info.mime_type)
 
         st.dataframe(table, use_container_width=True)
 
-        return
-
 
 class FilePreview(PreviewComponent):
     """Preview a value of type 'file'."""
 
     _component_name = "preview_file"
 
     @classmethod
@@ -120,16 +113,14 @@
         table["value"].append(file_model.mime_type)
         table["key"].append("content")
         table["value"].append(file_model.read_text())
         st.table(table)
 
         # st.table(table, use_container_width=True)
 
-        return
-
 
 class BooleanPreview(PreviewComponent):
     """Preview a value of type 'boolean'."""
 
     _component_name = "preview_boolean"
 
     @classmethod
```

### Comparing `kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/components/preview/network_data.py` & `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/preview/network_data.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # -*- coding: utf-8 -*-
-from streamlit.delta_generator import DeltaGenerator
-
 from kiara_plugin.streamlit.components.preview import PreviewComponent, PreviewOptions
+from streamlit.delta_generator import DeltaGenerator
 
 
 class NetworkDataPreview(PreviewComponent):
     """Preview a value of type 'network data'.
 
     Currently, this displays a graph, as well as the nodes and edges tables. The graph is only a preview, and takes a while to render depending on the network data size, this will replaced at some point.
     """
@@ -15,17 +14,18 @@
     @classmethod
     def get_data_type(cls) -> str:
         return "network_data"
 
     def render_preview(self, st: DeltaGenerator, options: PreviewOptions):
 
         import networkx as nx
+        from pyvis.network import Network
+
         import streamlit.components.v1 as components
         from kiara_plugin.network_analysis.models import NetworkData
-        from pyvis.network import Network
 
         _value = self.api.get_value(options.value)
         db: NetworkData = _value.data
         tab_names = ["graph"]
         tab_names.extend(db.table_names)
         tabs = st.tabs(tab_names)
```

### Comparing `kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/components/preview/tabular.py` & `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/preview/tabular.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # -*- coding: utf-8 -*-
+from kiara_plugin.streamlit.components.preview import PreviewComponent, PreviewOptions
 from kiara_plugin.tabular.models.array import KiaraArray
 from kiara_plugin.tabular.models.db import KiaraDatabase
 from kiara_plugin.tabular.models.table import KiaraTable
 from streamlit.delta_generator import DeltaGenerator
 
-from kiara_plugin.streamlit.components.preview import PreviewComponent, PreviewOptions
-
 
 class ArrayPreview(PreviewComponent):
     """Preview a value of type 'array'."""
 
     _component_name = "preview_array"
 
     @classmethod
@@ -34,15 +33,15 @@
         return "table"
 
     def render_preview(self, st: DeltaGenerator, options: PreviewOptions):
 
         _value = self.api.get_value(options.value)
         table: KiaraTable = _value.data
 
-        st.dataframe(table.to_pandas(), use_container_width=True)
+        st.dataframe(table.to_pandas_dataframe(), use_container_width=True)
 
 
 class DatabasePreview(PreviewComponent):
     """Preview a value of type 'database'."""
 
     _component_name = "preview_database"
```

### Comparing `kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/components/workflow/__init__.py` & `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/workflow/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
-from kiara.interfaces.python_api import Workflow
 from pydantic import BaseModel, Field
-from streamlit.delta_generator import DeltaGenerator
 
+from kiara.interfaces.python_api import Workflow
 from kiara_plugin.streamlit.components import ComponentOptions, KiaraComponent
+from streamlit.delta_generator import DeltaGenerator
 
 KIARA_METADATA = {
     "description": "Kiara streamlit compoents to work with workflows",
     "tags": ["workflows"],
     "labels": {"package": "kiara_plugin.core_types"},
 }
```

### Comparing `kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/components/workflow/dynamic/__init__.py` & `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/workflow/dynamic/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 from typing import Dict, List, Union
 
-from kiara.api import Value
-from kiara.interfaces.python_api import OperationInfo, Workflow
 from pydantic import Field
 
+from kiara.api import Value
+from kiara.interfaces.python_api import OperationInfo, Workflow
 from kiara_plugin.streamlit.components.workflow import WorkflowSession
 
 LEFT_COLUMN = 1
 RIGHT_COLUMN = 4
 
 
 class WorkflowSessionDynamic(WorkflowSession):
```

### Comparing `kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/components/workflow/dynamic/components.py` & `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/workflow/dynamic/components.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # -*- coding: utf-8 -*-
 from typing import Dict, Mapping, Tuple, TypeVar, Union
 
-from kiara.api import Value
-from kiara.models.module.operation import Operation
 from pydantic import Field
-from streamlit.delta_generator import DeltaGenerator
 
+from kiara.api import Value
+from kiara.models.module.operation import Operation
 from kiara_plugin.streamlit.components import ComponentOptions, KiaraComponent
 from kiara_plugin.streamlit.components.preview import PreviewOptions
 from kiara_plugin.streamlit.components.workflow.dynamic import WorkflowSessionDynamic
+from streamlit.delta_generator import DeltaGenerator
 
 
 class DynamicWorkflowOptions(ComponentOptions):
 
     session: WorkflowSessionDynamic = Field(description="The current workflow session.")
```

### Comparing `kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/components/workflow/dynamic/workflow_page.py` & `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/workflow/dynamic/workflow_page.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 # -*- coding: utf-8 -*-
 from typing import List, Union
 
 from kiara.api import Value
 from kiara.interfaces.python_api import OperationInfo
 from kiara.models.documentation import DocumentationMetadataModel
 from kiara.models.module.pipeline import PipelineStep, generate_pipeline_endpoint_name
-from streamlit.delta_generator import DeltaGenerator
-
 from kiara_plugin.streamlit.components import KiaraComponent
 from kiara_plugin.streamlit.components.workflow.dynamic import (
     LEFT_COLUMN,
     RIGHT_COLUMN,
     WorkflowSessionDynamic,
 )
 from kiara_plugin.streamlit.components.workflow.dynamic.components import (
     DynamicWorkflowOptions,
 )
+from streamlit.delta_generator import DeltaGenerator
 
 
 class DynamicWorkflow(KiaraComponent):
 
     _component_name = "workflow_dynamic"
     _options = DynamicWorkflowOptions
```

### Comparing `kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/components/workflow/requirements/__init__.py` & `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/workflow/requirements/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # -*- coding: utf-8 -*-
 from typing import Union
 
-from streamlit.delta_generator import DeltaGenerator
-
 from kiara_plugin.streamlit.components import ComponentOptions, KiaraComponent
 from kiara_plugin.streamlit.modules import DummyModuleConfig
+from streamlit.delta_generator import DeltaGenerator
 
 
 class StepRequirementsOptions(ComponentOptions):
     pass
 
 
 class StepRequirement(KiaraComponent[StepRequirementsOptions]):
```

### Comparing `kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/components/workflow/static/components.py` & `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/workflow/static/components.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # -*- coding: utf-8 -*-
 import uuid
 from typing import Dict, List, TypeVar, Union
 
-from kiara.api import ValueMap
 from pydantic import Field
-from streamlit.delta_generator import DeltaGenerator
 
+from kiara.api import ValueMap
 from kiara_plugin.streamlit.components import ComponentOptions, KiaraComponent
 from kiara_plugin.streamlit.components.workflow.static import WorkflowSessionStatic
+from streamlit.delta_generator import DeltaGenerator
 
 
 class StaticWorkflowOptions(ComponentOptions):
 
     session: WorkflowSessionStatic = Field(description="The current workflow session.")
```

### Comparing `kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/components/workflow/static/workflow_page.py` & `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/workflow/static/workflow_page.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 # -*- coding: utf-8 -*-
 from typing import Dict
 
 from kiara.api import ValueSchema
 from kiara.exceptions import KiaraException
 from kiara.models.module.pipeline import StepStatus
 from kiara.models.module.pipeline.structure import PipelineStructure
-from streamlit.delta_generator import DeltaGenerator
-
 from kiara_plugin.streamlit.components import KiaraComponent
 from kiara_plugin.streamlit.components.workflow.static.components import (
     StaticWorkflowOptions,
 )
+from streamlit.delta_generator import DeltaGenerator
 
 
 class WorkflowStatic(KiaraComponent[StaticWorkflowOptions]):
 
     _component_name = "workflow_static"
     _options = StaticWorkflowOptions
 
@@ -81,15 +80,15 @@
         #     if step_states[step].status != StepStatus.RESULTS_READY:
         #         print(f"NOT READY: {step}")
         #         ready = False
         #         break
 
         steps_to_process = []
         stages_to_process = [session.current_stage]
-        for stage in stages[0 : session.current_stage]:  # noqa
+        for stage in stages[0 : session.current_stage]:
             steps_to_process.append(stage)
 
         cur = session.current_stage + 1
 
         while cur in no_input_stages:
             stages_to_process.append(cur)
             steps_to_process.append(stages[cur - 1])
```

### Comparing `kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/interfaces/cli/streamlit.py` & `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/interfaces/cli/streamlit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 from typing import Iterable
 
 import rich_click as click
+
 from kiara.utils.cli import output_format_option, terminal_print_model
 
 #  Copyright (c) 2021, Markus Binsteiner
 #
 #  Mozilla Public License, version 2.0 (see LICENSE or https://www.mozilla.org/en-US/MPL/2.0/)
```

### Comparing `kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/models.py` & `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/models.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/modules/__init__.py` & `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/modules/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 # -*- coding: utf-8 -*-
 from typing import Any, Dict, Mapping
 
 from boltons.strutils import slugify
+from pydantic import Field
+
 from kiara.api import KiaraModule, KiaraModuleConfig, ValueMap, ValueMapSchema
 from kiara.models.module.pipeline import PipelineConfig
-from pydantic import Field
 
 
 class DummyModuleConfig(KiaraModuleConfig):
     @classmethod
-    def create_pipeline_config(cls, *steps: "DummyModuleConfig") -> PipelineConfig:
+    def create_pipeline_config(
+        cls, title: str, description: str, author: str, *steps: "DummyModuleConfig"
+    ) -> PipelineConfig:
 
-        data: Dict[str, Any] = {"pipeline_name": "dummy", "steps": []}
+        data: Dict[str, Any] = {
+            "pipeline_name": slugify(title),
+            "doc": description,
+            "context": {"authors": [author]},
+            "steps": [],
+        }
         for step in steps:
             step_data = {
                 "step_id": slugify(step.title),
                 "module_type": "dummy",
                 "module_config": {
                     "title": step.title,
                     "inputs_schema": step.inputs_schema,
```

### Comparing `kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/renderers/__init__.py` & `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/renderers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 from typing import Any, Iterable, Mapping, Union
 
 from jinja2 import Template
+
 from kiara.models.module.pipeline.pipeline import Pipeline
 from kiara.renderers import RenderInputsSchema, SourceTransformer
 from kiara.renderers.included_renderers.pipeline import PipelineTransformer
 from kiara.renderers.jinja import BaseJinjaRenderer, JinjaEnv
 from kiara.utils import log_message
```

### Comparing `kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/resources/templates/pipeline/streamlit_app.py.j2` & `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/resources/templates/pipeline/streamlit_app.py.j2`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/streamlit.py` & `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/streamlit.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,23 +5,22 @@
 import uuid
 from pathlib import Path
 from typing import Dict, Mapping, Union
 
 import streamlit as st
 from kiara.api import KiaraAPI
 from kiara.context import KiaraConfig, KiaraContextConfig, KiaraRuntimeConfig
-from streamlit.runtime.scriptrunner import get_script_run_ctx
-
 from kiara_plugin.streamlit.components import KiaraComponent
 from kiara_plugin.streamlit.components.input import InputComponent
 from kiara_plugin.streamlit.components.preview import PreviewComponent
 from kiara_plugin.streamlit.defaults import kiara_stremalit_app_dirs
 from kiara_plugin.streamlit.utils.class_loading import (
     find_all_kiara_streamlit_components,
 )
+from streamlit.runtime.scriptrunner import get_script_run_ctx
 
 
 class ComponentMgmt(object):
     def __init__(
         self,
         kiara_streamlit: "KiaraStreamlit",
         example_base_dir: Union[str, Path, None] = None,
@@ -141,21 +140,21 @@
         self._preview_components = preview_components
         self._input_components = input_components
         return self._components
 
     @property
     def preview_components(self) -> Mapping[str, Mapping[str, PreviewComponent]]:
         if self._preview_components is None:
-            self.components  # noqa
+            self.components
         return self._preview_components  # type: ignore
 
     @property
     def input_components(self) -> Mapping[str, InputComponent]:
         if self._input_components is None:
-            self.components  # noqa
+            self.components
         return self._input_components  # type: ignore
 
 
 class KiaraStreamlit(object):
     def __init__(
         self,
         context_config: Union[None, KiaraContextConfig] = None,
@@ -190,15 +189,15 @@
         )
 
         def del_temp_dir():
             shutil.rmtree(self._temp_dir, ignore_errors=True)
 
         atexit.register(del_temp_dir)
 
-        self.api  # noqa
+        self.api
 
         # self.add_component("test", TestComponent(kiara_streamlit=self))
         # self.add_component("help", HelpComponent(kiara_streamlit=self))
 
     def __getattr__(self, item):
 
         # if item in ["api", "components", "get_component"]:
```

### Comparing `kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/utils/class_loading.py` & `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/utils/class_loading.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 
 
 def find_kiara_streamlit_components_under(
     module: Union[str, ModuleType],
 ) -> List[Type["KiaraComponent"]]:
 
     from kiara.utils.class_loading import find_subclasses_under
-
     from kiara_plugin.streamlit.components import KiaraComponent
 
     return find_subclasses_under(
         base_class=KiaraComponent,  # type: ignore
         python_module=module,
     )
 
@@ -35,15 +34,14 @@
 def find_all_kiara_streamlit_components() -> Dict[str, Type["KiaraComponent"]]:
     """Find all [KiaraComponent][kiara_plugin.streamilt.components.KiaraComponent] subclasses via package entry points.
 
     TODO
     """
 
     from kiara.utils.class_loading import load_all_subclasses_for_entry_point
-
     from kiara_plugin.streamlit.components import KiaraComponent
 
     components = load_all_subclasses_for_entry_point(
         entry_point_name="kiara.streamlit_components",
         base_class=KiaraComponent,  # type: ignore
         type_id_key="_component_name",
         type_id_func=_cls_name_id_func,
```

### Comparing `kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/utils/components.py` & `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/utils/components.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 import warnings
 from typing import List, Union
 
 import pandas as pd
 from st_aggrid import AgGrid, ColumnsAutoSizeMode, GridOptionsBuilder
+
 from streamlit.delta_generator import DeltaGenerator
 
 
 def create_list_component(
     st: DeltaGenerator,
     key: str,
     title: str,
```

### Comparing `kiara_plugin.streamlit-0.4.1/src/kiara_plugin/streamlit/utils/monkey_patches.py` & `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/utils/monkey_patches.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 # -*- coding: utf-8 -*-
-from typing import TYPE_CHECKING
 
-from streamlit.delta_generator import *  # noqa
-from streamlit.delta_generator import _enqueue_message
-
-if TYPE_CHECKING:
-    from streamlit.delta_generator import DeltaGenerator
+from streamlit.delta_generator import (
+    Block_pb2,
+    DeltaGenerator,
+    ForwardMsg_pb2,
+    _enqueue_message,
+    caching,
+    current_form_id,
+    cursor,
+)
+from streamlit.elements.form import FormData
 
 # copied from: https://github.com/joy13975/streamlit-nested-layout/blob/main/streamlit_nested_layout/nest.py
 # License: Apache License 2.0
 # Copyright Joy Yeh
 
 
 def _nestable_block(
@@ -40,25 +44,25 @@
     msg.delta.add_block.CopyFrom(block_proto)
 
     # Normally we'd return a new DeltaGenerator that uses the locked cursor
     # below. But in this case we want to return a DeltaGenerator that uses
     # a brand new cursor for this new block we're creating.
     block_cursor: cursor.RunningCursor = cursor.RunningCursor(  # type: ignore
         root_container=dg._root_container,  # type: ignore
-        parent_path=dg._cursor.parent_path + (dg._cursor.index,),  # type: ignore
+        parent_path=dg._cursor.parent_path + (dg._cursor.index,),  # type: ignore  # noqa
     )
     block_dg = DeltaGenerator(
         root_container=dg._root_container,
         cursor=block_cursor,
         parent=dg,
         block_type=block_type,
     )
     # Blocks inherit their parent form ids.
     # NOTE: Container form ids aren't set in proto.
-    block_dg._form_data = FormData(current_form_id(dg))  # type: ignore
+    block_dg._form_data = FormData(current_form_id(dg))
 
     # Must be called to increment this cursor's index.
     dg._cursor.get_locked_cursor(last_index=None)
     _enqueue_message(msg)
 
     caching.save_block_message(  # type: ignore
         block_proto,
```

### Comparing `kiara_plugin.streamlit-0.4.1/src/kiara_plugin.streamlit.egg-info/PKG-INFO` & `kiara_plugin.streamlit-0.4.2/src/kiara_plugin.streamlit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiara-plugin.streamlit
-Version: 0.4.1
+Version: 0.4.2
 Summary: Streamlit UI and widgets for kiara
 Author-email: Markus Binsteiner <markus@frkl.io>
 License: MPL-2.0
 Project-URL: homepage, https://github.com/DHARPA-Project/kiara_plugin.streamlit
 Project-URL: documentation, https://DHARPA-Project.github.io/kiara_plugin.streamlit
 Project-URL: repository, https://github.com/DHARPA-Project/kiara_plugin.streamlit
 Keywords: kiara,streamlit
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: workflow_app
 Provides-Extra: all_plugins
 Provides-Extra: dev_documentation
 Provides-Extra: dev_testing
 Provides-Extra: dev_utils
 Provides-Extra: dev_all
 License-File: LICENSE
 License-File: AUTHORS.md
```

### Comparing `kiara_plugin.streamlit-0.4.1/src/kiara_plugin.streamlit.egg-info/SOURCES.txt` & `kiara_plugin.streamlit-0.4.2/src/kiara_plugin.streamlit.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -30,17 +30,20 @@
 docs/index.md
 docs/usage.md
 docs/stylesheets/extra.css
 examples/data/Readme.md
 examples/data/journals/JournalEdges1902.csv
 examples/data/journals/JournalNodes1902.csv
 examples/data/journals/Readme.md
+examples/jobs/Readme.md
+examples/pipelines/Readme.md
 examples/streamlit/example.py
 examples/streamlit/help.py
 examples/streamlit/pipeline.py
+examples/streamlit/step_inputs.py
 examples/streamlit/workflow_dynamic.py
 examples/streamlit/workflow_static.py
 examples/streamlit/workflows.py
 examples/streamlit/workshop.py
 examples/streamlit/pipelines/example.yaml
 examples/streamlit/pipelines/topic_modeling.yaml
 scripts/documentation/gen_api_doc_pages.py
@@ -93,8 +96,10 @@
 src/kiara_plugin/streamlit/resources/.gitkeep
 src/kiara_plugin/streamlit/resources/templates/pipeline/streamlit_app.py.j2
 src/kiara_plugin/streamlit/utils/__init__.py
 src/kiara_plugin/streamlit/utils/class_loading.py
 src/kiara_plugin/streamlit/utils/components.py
 src/kiara_plugin/streamlit/utils/monkey_patches.py
 tests/conftest.py
-tests/test_kiara_modules_default.py
+tests/test_job_descs.py
+tests/test_kiara_modules_default.py
+tests/resources/.gitkeep
```

### Comparing `kiara_plugin.streamlit-0.4.1/src/kiara_plugin.streamlit.egg-info/entry_points.txt` & `kiara_plugin.streamlit-0.4.2/src/kiara_plugin.streamlit.egg-info/entry_points.txt`

 * *Files identical despite different names*

