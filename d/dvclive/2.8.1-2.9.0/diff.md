# Comparing `tmp/dvclive-2.8.1.tar.gz` & `tmp/dvclive-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvclive-2.8.1.tar", last modified: Tue May  2 09:01:22 2023, max compression
+gzip compressed data, was "dvclive-2.9.0.tar", last modified: Mon May 15 12:09:17 2023, max compression
```

## Comparing `dvclive-2.8.1.tar` & `dvclive-2.9.0.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:01:22.139661 dvclive-2.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-02 09:00:58.000000 dvclive-2.8.1/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 09:00:58.000000 dvclive-2.8.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:01:22.131661 dvclive-2.8.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-02 09:00:58.000000 dvclive-2.8.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-02 09:00:58.000000 dvclive-2.8.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:01:22.131661 dvclive-2.8.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-02 09:00:58.000000 dvclive-2.8.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-02 09:00:58.000000 dvclive-2.8.1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-02 09:00:58.000000 dvclive-2.8.1/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-02 09:00:58.000000 dvclive-2.8.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-02 09:00:58.000000 dvclive-2.8.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-05-02 09:00:58.000000 dvclive-2.8.1/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-05-02 09:00:58.000000 dvclive-2.8.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-05-02 09:00:58.000000 dvclive-2.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-05-02 09:01:22.139661 dvclive-2.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-05-02 09:00:58.000000 dvclive-2.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:01:22.131661 dvclive-2.8.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)   321138 2023-05-02 09:00:58.000000 dvclive-2.8.1/docs/dvc_plots_diff.png
--rw-r--r--   0 runner    (1001) docker     (123)   676021 2023-05-02 09:00:58.000000 dvclive-2.8.1/docs/studio_compare.png
--rw-r--r--   0 runner    (1001) docker     (123)   501824 2023-05-02 09:00:58.000000 dvclive-2.8.1/docs/vscode_experiments.png
--rw-r--r--   0 runner    (1001) docker     (123)   627561 2023-05-02 09:00:58.000000 dvclive-2.8.1/docs/vscode_plots.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:01:22.135661 dvclive-2.8.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    10070 2023-05-02 09:00:58.000000 dvclive-2.8.1/examples/DVCLive-Quickstart.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-02 09:00:58.000000 dvclive-2.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-05-02 09:01:22.139661 dvclive-2.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-02 09:00:58.000000 dvclive-2.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:01:22.127661 dvclive-2.8.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:01:22.135661 dvclive-2.8.1/src/dvclive/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-02 09:00:58.000000 dvclive-2.8.1/src/dvclive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-02 09:00:58.000000 dvclive-2.8.1/src/dvclive/catalyst.py
--rw-r--r--   0 runner    (1001) docker     (123)    19688 2023-05-02 09:00:58.000000 dvclive-2.8.1/src/dvclive/dvc.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-02 09:00:58.000000 dvclive-2.8.1/src/dvclive/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-02 09:00:58.000000 dvclive-2.8.1/src/dvclive/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-05-02 09:00:58.000000 dvclive-2.8.1/src/dvclive/fastai.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-02 09:00:58.000000 dvclive-2.8.1/src/dvclive/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-02 09:00:58.000000 dvclive-2.8.1/src/dvclive/keras.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-02 09:00:58.000000 dvclive-2.8.1/src/dvclive/lgbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-05-02 09:00:58.000000 dvclive-2.8.1/src/dvclive/lightning.py
--rw-r--r--   0 runner    (1001) docker     (123)    18332 2023-05-02 09:00:58.000000 dvclive-2.8.1/src/dvclive/live.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-02 09:00:58.000000 dvclive-2.8.1/src/dvclive/optuna.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:01:22.139661 dvclive-2.8.1/src/dvclive/plots/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-02 09:00:58.000000 dvclive-2.8.1/src/dvclive/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-02 09:00:58.000000 dvclive-2.8.1/src/dvclive/plots/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-02 09:00:58.000000 dvclive-2.8.1/src/dvclive/plots/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-02 09:00:58.000000 dvclive-2.8.1/src/dvclive/plots/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-02 09:00:58.000000 dvclive-2.8.1/src/dvclive/plots/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-05-02 09:00:58.000000 dvclive-2.8.1/src/dvclive/plots/sklearn.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-02 09:00:58.000000 dvclive-2.8.1/src/dvclive/plots/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-05-02 09:00:58.000000 dvclive-2.8.1/src/dvclive/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-02 09:00:58.000000 dvclive-2.8.1/src/dvclive/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-02 09:00:58.000000 dvclive-2.8.1/src/dvclive/studio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-05-02 09:00:58.000000 dvclive-2.8.1/src/dvclive/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-02 09:00:58.000000 dvclive-2.8.1/src/dvclive/xgb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:01:22.135661 dvclive-2.8.1/src/dvclive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-05-02 09:01:22.000000 dvclive-2.8.1/src/dvclive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-05-02 09:01:22.000000 dvclive-2.8.1/src/dvclive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 09:01:22.000000 dvclive-2.8.1/src/dvclive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 09:01:21.000000 dvclive-2.8.1/src/dvclive.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-02 09:01:22.000000 dvclive-2.8.1/src/dvclive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-02 09:01:22.000000 dvclive-2.8.1/src/dvclive.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:01:22.139661 dvclive-2.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 09:00:58.000000 dvclive-2.8.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-02 09:00:58.000000 dvclive-2.8.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:01:22.139661 dvclive-2.8.1/tests/plots/
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-02 09:00:58.000000 dvclive-2.8.1/tests/plots/test_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-05-02 09:00:58.000000 dvclive-2.8.1/tests/plots/test_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-02 09:00:58.000000 dvclive-2.8.1/tests/plots/test_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-05-02 09:00:58.000000 dvclive-2.8.1/tests/plots/test_sklearn.py
--rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-05-02 09:00:58.000000 dvclive-2.8.1/tests/test_dvc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:01:22.139661 dvclive-2.8.1/tests/test_frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-05-02 09:00:58.000000 dvclive-2.8.1/tests/test_frameworks/test_catalyst.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-05-02 09:00:58.000000 dvclive-2.8.1/tests/test_frameworks/test_fastai.py
--rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-05-02 09:00:58.000000 dvclive-2.8.1/tests/test_frameworks/test_huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-05-02 09:00:58.000000 dvclive-2.8.1/tests/test_frameworks/test_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-02 09:00:58.000000 dvclive-2.8.1/tests/test_frameworks/test_lgbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-05-02 09:00:58.000000 dvclive-2.8.1/tests/test_frameworks/test_lightning.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-02 09:00:58.000000 dvclive-2.8.1/tests/test_frameworks/test_optuna.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-02 09:00:58.000000 dvclive-2.8.1/tests/test_frameworks/test_xgboost.py
--rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-05-02 09:00:58.000000 dvclive-2.8.1/tests/test_log_artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)    13062 2023-05-02 09:00:58.000000 dvclive-2.8.1/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     7545 2023-05-02 09:00:58.000000 dvclive-2.8.1/tests/test_report.py
--rw-r--r--   0 runner    (1001) docker     (123)    11311 2023-05-02 09:00:58.000000 dvclive-2.8.1/tests/test_studio.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-02 09:00:58.000000 dvclive-2.8.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:09:17.897939 dvclive-2.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-15 12:09:00.000000 dvclive-2.9.0/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-15 12:09:00.000000 dvclive-2.9.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:09:17.877939 dvclive-2.9.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-15 12:09:00.000000 dvclive-2.9.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-15 12:09:00.000000 dvclive-2.9.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:09:17.877939 dvclive-2.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-15 12:09:00.000000 dvclive-2.9.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-15 12:09:00.000000 dvclive-2.9.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-15 12:09:00.000000 dvclive-2.9.0/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-15 12:09:00.000000 dvclive-2.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-05-15 12:09:00.000000 dvclive-2.9.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-05-15 12:09:00.000000 dvclive-2.9.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-05-15 12:09:00.000000 dvclive-2.9.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-05-15 12:09:00.000000 dvclive-2.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-05-15 12:09:17.897939 dvclive-2.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-05-15 12:09:00.000000 dvclive-2.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:09:17.881939 dvclive-2.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)   321138 2023-05-15 12:09:00.000000 dvclive-2.9.0/docs/dvc_plots_diff.png
+-rw-r--r--   0 runner    (1001) docker     (123)   676021 2023-05-15 12:09:00.000000 dvclive-2.9.0/docs/studio_compare.png
+-rw-r--r--   0 runner    (1001) docker     (123)   501824 2023-05-15 12:09:00.000000 dvclive-2.9.0/docs/vscode_experiments.png
+-rw-r--r--   0 runner    (1001) docker     (123)   627561 2023-05-15 12:09:00.000000 dvclive-2.9.0/docs/vscode_plots.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:09:17.885939 dvclive-2.9.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    10070 2023-05-15 12:09:00.000000 dvclive-2.9.0/examples/DVCLive-Quickstart.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-15 12:09:00.000000 dvclive-2.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-05-15 12:09:17.897939 dvclive-2.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-15 12:09:00.000000 dvclive-2.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:09:17.873939 dvclive-2.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:09:17.889939 dvclive-2.9.0/src/dvclive/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-15 12:09:00.000000 dvclive-2.9.0/src/dvclive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-15 12:09:00.000000 dvclive-2.9.0/src/dvclive/catalyst.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19687 2023-05-15 12:09:00.000000 dvclive-2.9.0/src/dvclive/dvc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-15 12:09:00.000000 dvclive-2.9.0/src/dvclive/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-15 12:09:00.000000 dvclive-2.9.0/src/dvclive/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-05-15 12:09:00.000000 dvclive-2.9.0/src/dvclive/fastai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-15 12:09:00.000000 dvclive-2.9.0/src/dvclive/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-15 12:09:00.000000 dvclive-2.9.0/src/dvclive/keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-15 12:09:00.000000 dvclive-2.9.0/src/dvclive/lgbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-05-15 12:09:00.000000 dvclive-2.9.0/src/dvclive/lightning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18585 2023-05-15 12:09:00.000000 dvclive-2.9.0/src/dvclive/live.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-15 12:09:00.000000 dvclive-2.9.0/src/dvclive/optuna.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:09:17.893939 dvclive-2.9.0/src/dvclive/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-15 12:09:00.000000 dvclive-2.9.0/src/dvclive/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-15 12:09:00.000000 dvclive-2.9.0/src/dvclive/plots/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-15 12:09:00.000000 dvclive-2.9.0/src/dvclive/plots/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-15 12:09:00.000000 dvclive-2.9.0/src/dvclive/plots/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-15 12:09:00.000000 dvclive-2.9.0/src/dvclive/plots/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-05-15 12:09:00.000000 dvclive-2.9.0/src/dvclive/plots/sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-15 12:09:00.000000 dvclive-2.9.0/src/dvclive/plots/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-05-15 12:09:00.000000 dvclive-2.9.0/src/dvclive/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-15 12:09:00.000000 dvclive-2.9.0/src/dvclive/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-05-15 12:09:00.000000 dvclive-2.9.0/src/dvclive/studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-05-15 12:09:00.000000 dvclive-2.9.0/src/dvclive/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-15 12:09:00.000000 dvclive-2.9.0/src/dvclive/xgb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:09:17.889939 dvclive-2.9.0/src/dvclive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-05-15 12:09:17.000000 dvclive-2.9.0/src/dvclive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-05-15 12:09:17.000000 dvclive-2.9.0/src/dvclive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 12:09:17.000000 dvclive-2.9.0/src/dvclive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 12:09:17.000000 dvclive-2.9.0/src/dvclive.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-15 12:09:17.000000 dvclive-2.9.0/src/dvclive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 12:09:17.000000 dvclive-2.9.0/src/dvclive.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:09:17.893939 dvclive-2.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:09:00.000000 dvclive-2.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-15 12:09:00.000000 dvclive-2.9.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:09:17.893939 dvclive-2.9.0/tests/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-15 12:09:00.000000 dvclive-2.9.0/tests/plots/test_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-05-15 12:09:00.000000 dvclive-2.9.0/tests/plots/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-15 12:09:00.000000 dvclive-2.9.0/tests/plots/test_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-05-15 12:09:00.000000 dvclive-2.9.0/tests/plots/test_sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-05-15 12:09:00.000000 dvclive-2.9.0/tests/test_dvc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:09:17.897939 dvclive-2.9.0/tests/test_frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-05-15 12:09:00.000000 dvclive-2.9.0/tests/test_frameworks/test_catalyst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-05-15 12:09:00.000000 dvclive-2.9.0/tests/test_frameworks/test_fastai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-05-15 12:09:00.000000 dvclive-2.9.0/tests/test_frameworks/test_huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-05-15 12:09:00.000000 dvclive-2.9.0/tests/test_frameworks/test_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-15 12:09:00.000000 dvclive-2.9.0/tests/test_frameworks/test_lgbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-05-15 12:09:00.000000 dvclive-2.9.0/tests/test_frameworks/test_lightning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-15 12:09:00.000000 dvclive-2.9.0/tests/test_frameworks/test_optuna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-15 12:09:00.000000 dvclive-2.9.0/tests/test_frameworks/test_xgboost.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-05-15 12:09:00.000000 dvclive-2.9.0/tests/test_log_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13062 2023-05-15 12:09:00.000000 dvclive-2.9.0/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7545 2023-05-15 12:09:00.000000 dvclive-2.9.0/tests/test_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-05-15 12:09:00.000000 dvclive-2.9.0/tests/test_studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-15 12:09:00.000000 dvclive-2.9.0/tests/test_utils.py
```

### Comparing `dvclive-2.8.1/.cruft.json` & `dvclive-2.9.0/.cruft.json`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.1/.github/dependabot.yml` & `dvclive-2.9.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.1/.github/workflows/release.yml` & `dvclive-2.9.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.1/.github/workflows/tests.yml` & `dvclive-2.9.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.1/.gitignore` & `dvclive-2.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.1/.pre-commit-config.yaml` & `dvclive-2.9.0/.pre-commit-config.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -30,15 +30,16 @@
   - repo: https://github.com/codespell-project/codespell
     rev: v2.2.4
     hooks:
       - id: codespell
         additional_dependencies: ["tomli"]
   - repo: https://github.com/charliermarsh/ruff-pre-commit
     # Ruff version.
-    rev: 'v0.0.263'
+    rev: 'v0.0.265'
     hooks:
       - id: ruff
   - repo: https://github.com/executablebooks/mdformat
     rev: 0.7.16
     hooks:
     - id: mdformat
+      exclude: ^\.github/.+_TEMPLATE.md$
       args: ["--wrap=80"]
```

### Comparing `dvclive-2.8.1/CODE_OF_CONDUCT.rst` & `dvclive-2.9.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.1/CONTRIBUTING.rst` & `dvclive-2.9.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.1/LICENSE` & `dvclive-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.1/PKG-INFO` & `dvclive-2.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvclive
-Version: 2.8.1
+Version: 2.9.0
 Summary: Metric logger for ML projects.
 Home-page: https://github.com/iterative/dvclive
 Maintainer-email: support@dvc.org
 License: Apache-2.0
 Project-URL: Documentation, https://dvc.org/doc/dvclive
 Project-URL: Source, https://github.com/iterative/dvclive
 Keywords: data-science,metrics,machine-learning,developer-tools,ai
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dvclive Version: 2.8.1 Summary: Metric logger for
+Metadata-Version: 2.1 Name: dvclive Version: 2.9.0 Summary: Metric logger for
 ML projects. Home-page: https://github.com/iterative/dvclive Maintainer-email:
 support@dvc.org License: Apache-2.0 Project-URL: Documentation, https://
 dvc.org/doc/dvclive Project-URL: Source, https://github.com/iterative/dvclive
 Keywords: data-science,metrics,machine-learning,developer-tools,ai Platform:
 any Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
```

### Comparing `dvclive-2.8.1/README.md` & `dvclive-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.1/docs/dvc_plots_diff.png` & `dvclive-2.9.0/docs/dvc_plots_diff.png`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.1/docs/studio_compare.png` & `dvclive-2.9.0/docs/studio_compare.png`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.1/docs/vscode_experiments.png` & `dvclive-2.9.0/docs/vscode_experiments.png`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.1/docs/vscode_plots.png` & `dvclive-2.9.0/docs/vscode_plots.png`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.1/examples/DVCLive-Quickstart.ipynb` & `dvclive-2.9.0/examples/DVCLive-Quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.1/pyproject.toml` & `dvclive-2.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.1/setup.cfg` & `dvclive-2.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.1/src/dvclive/catalyst.py` & `dvclive-2.9.0/src/dvclive/catalyst.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.1/src/dvclive/dvc.py` & `dvclive-2.9.0/src/dvclive/dvc.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
             plots.append({plot_path.as_posix(): plot.plot_config})
     if plots:
         dvcyaml["plots"] = plots
 
     if live._artifacts:
         dvcyaml["artifacts"] = live._artifacts
         for artifact in dvcyaml["artifacts"].values():
-            abs_path = os.path.realpath(artifact["path"])
+            abs_path = os.path.abspath(artifact["path"])
             abs_dir = os.path.realpath(live.dir)
             relative_path = os.path.relpath(abs_path, abs_dir)
             artifact["path"] = Path(relative_path).as_posix()
 
     dump_yaml(dvcyaml, live.dvc_file)
```

### Comparing `dvclive-2.8.1/src/dvclive/error.py` & `dvclive-2.9.0/src/dvclive/error.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.1/src/dvclive/fastai.py` & `dvclive-2.9.0/src/dvclive/fastai.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.1/src/dvclive/huggingface.py` & `dvclive-2.9.0/src/dvclive/huggingface.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.1/src/dvclive/keras.py` & `dvclive-2.9.0/src/dvclive/keras.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.1/src/dvclive/lgbm.py` & `dvclive-2.9.0/src/dvclive/lgbm.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.1/src/dvclive/lightning.py` & `dvclive-2.9.0/src/dvclive/lightning.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.1/src/dvclive/live.py` & `dvclive-2.9.0/src/dvclive/live.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,25 +26,31 @@
     InvalidPlotTypeError,
     InvalidReportModeError,
 )
 from .plots import PLOT_TYPES, SKLEARN_PLOTS, CustomPlot, Image, Metric, NumpyEncoder
 from .report import BLANK_NOTEBOOK_REPORT, make_report
 from .serialize import dump_json, dump_yaml, load_yaml
 from .studio import get_studio_updates
-from .utils import env2bool, inside_notebook, matplotlib_installed, open_file_in_browser
+from .utils import (
+    StrPath,
+    clean_and_copy_into,
+    env2bool,
+    inside_notebook,
+    matplotlib_installed,
+    open_file_in_browser,
+)
 
 logger = logging.getLogger("dvclive")
 handler = logging.StreamHandler()
 formatter = logging.Formatter("%(levelname)s:%(name)s:%(message)s")
 handler.setFormatter(formatter)
 logger.addHandler(handler)
 logger.setLevel(os.getenv(env.DVCLIVE_LOGLEVEL, "INFO").upper())
 
 ParamLike = Union[int, float, str, bool, List["ParamLike"], Dict[str, "ParamLike"]]
-StrPath = Union[str, Path]
 
 
 class Live:
     def __init__(
         self,
         dir: str = "dvclive",  # noqa: A002
         resume: bool = False,
@@ -227,14 +233,18 @@
         return os.path.join(self.dir, "dvc.yaml")
 
     @property
     def plots_dir(self) -> str:
         return os.path.join(self.dir, "plots")
 
     @property
+    def artifacts_dir(self) -> str:
+        return os.path.join(self.dir, "artifacts")
+
+    @property
     def report_file(self) -> Optional[str]:
         if self._report_mode in ("html", "md", "notebook"):
             suffix = "html" if self._report_mode == "notebook" else self._report_mode
             return os.path.join(self.dir, f"report.{suffix}")
         return None
 
     @property
@@ -376,22 +386,26 @@
         self,
         path: StrPath,
         type: Optional[str] = None,  # noqa: A002
         name: Optional[str] = None,
         desc: Optional[str] = None,  # noqa: ARG002
         labels: Optional[List[str]] = None,  # noqa: ARG002
         meta: Optional[Dict[str, Any]] = None,  # noqa: ARG002
+        copy: bool = False,
     ):
         """Tracks a local file or directory with DVC"""
         if not isinstance(path, (str, Path)):
             raise InvalidDataTypeError(path, type(path))
 
         if self._dvc_repo is not None:
             from dvc.repo.artifacts import name_is_compatible
 
+            if copy:
+                path = clean_and_copy_into(path, self.artifacts_dir)
+
             try:
                 stage = self._dvc_repo.add(path)
             except Exception as e:  # noqa: BLE001
                 logger.warning(f"Failed to dvc add {path}: {e}")
                 return
 
             name = name or Path(path).stem
```

### Comparing `dvclive-2.8.1/src/dvclive/optuna.py` & `dvclive-2.9.0/src/dvclive/optuna.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.1/src/dvclive/plots/base.py` & `dvclive-2.9.0/src/dvclive/plots/base.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.1/src/dvclive/plots/custom.py` & `dvclive-2.9.0/src/dvclive/plots/custom.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.1/src/dvclive/plots/image.py` & `dvclive-2.9.0/src/dvclive/plots/image.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.1/src/dvclive/plots/metric.py` & `dvclive-2.9.0/src/dvclive/plots/metric.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.1/src/dvclive/plots/sklearn.py` & `dvclive-2.9.0/src/dvclive/plots/sklearn.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.1/src/dvclive/plots/utils.py` & `dvclive-2.9.0/src/dvclive/plots/utils.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.1/src/dvclive/report.py` & `dvclive-2.9.0/src/dvclive/report.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.1/src/dvclive/serialize.py` & `dvclive-2.9.0/src/dvclive/serialize.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.1/src/dvclive/studio.py` & `dvclive-2.9.0/src/dvclive/studio.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # ruff: noqa: SLF001
+import base64
 import os
 from pathlib import Path
 
 from dvclive.serialize import load_yaml
 from dvclive.utils import parse_metrics
 
 
@@ -39,14 +40,29 @@
 
 
 def _adapt_plot_datapoints(live, plot):
     datapoints = _get_unsent_datapoints(plot, live._latest_studio_step)
     return _cast_to_numbers(datapoints)
 
 
+def _adapt_image(image_path):
+    with open(image_path, "rb") as fobj:
+        return base64.b64encode(fobj.read()).decode("utf-8")
+
+
+def _adapt_images(live):
+    return {
+        _adapt_plot_name(live, image.output_path): {
+            "image": _adapt_image(image.output_path)
+        }
+        for image in live._images.values()
+        if image.step > live._latest_studio_step
+    }
+
+
 def get_studio_updates(live):
     if os.path.isfile(live.params_file):
         params_file = live.params_file
         if live._dvc_repo is not None:
             params_file = _rel_path(params_file, live._dvc_repo.root_dir)
         params = {params_file: load_yaml(live.params_file)}
     else:
@@ -61,8 +77,10 @@
 
     plots = {
         _adapt_plot_name(live, name): _adapt_plot_datapoints(live, plot)
         for name, plot in plots.items()
     }
     plots = {k: {"data": v} for k, v in plots.items()}
 
+    plots.update(_adapt_images(live))
+
     return metrics, params, plots
```

### Comparing `dvclive-2.8.1/src/dvclive/utils.py` & `dvclive-2.9.0/src/dvclive/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import csv
 import json
 import os
 import re
+import shutil
 import webbrowser
 from pathlib import Path
 from platform import uname
+from typing import Union
+
+StrPath = Union[str, Path]
 
 
 def run_once(f):
     def wrapper(*args, **kwargs):
         if not wrapper.has_run:
             wrapper.has_run = True
             return f(*args, **kwargs)
@@ -121,7 +125,26 @@
         return False
 
     if shell == "ZMQInteractiveShell":
         import IPython
 
         return IPython.__version__ >= "6.0.0"
     return False
+
+
+def clean_and_copy_into(src: StrPath, dst: StrPath) -> str:
+    Path(dst).mkdir(exist_ok=True)
+
+    basename = os.path.basename(os.path.normpath(src))
+    dst_path = Path(os.path.join(dst, basename))
+
+    if dst_path.is_file() or dst_path.is_symlink():
+        dst_path.unlink()
+    elif dst_path.is_dir():
+        shutil.rmtree(dst_path)
+
+    if os.path.isdir(src):
+        shutil.copytree(src, dst_path)
+    else:
+        shutil.copy2(src, dst_path)
+
+    return str(dst_path)
```

### Comparing `dvclive-2.8.1/src/dvclive/xgb.py` & `dvclive-2.9.0/src/dvclive/xgb.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.1/src/dvclive.egg-info/PKG-INFO` & `dvclive-2.9.0/src/dvclive.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvclive
-Version: 2.8.1
+Version: 2.9.0
 Summary: Metric logger for ML projects.
 Home-page: https://github.com/iterative/dvclive
 Maintainer-email: support@dvc.org
 License: Apache-2.0
 Project-URL: Documentation, https://dvc.org/doc/dvclive
 Project-URL: Source, https://github.com/iterative/dvclive
 Keywords: data-science,metrics,machine-learning,developer-tools,ai
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dvclive Version: 2.8.1 Summary: Metric logger for
+Metadata-Version: 2.1 Name: dvclive Version: 2.9.0 Summary: Metric logger for
 ML projects. Home-page: https://github.com/iterative/dvclive Maintainer-email:
 support@dvc.org License: Apache-2.0 Project-URL: Documentation, https://
 dvc.org/doc/dvclive Project-URL: Source, https://github.com/iterative/dvclive
 Keywords: data-science,metrics,machine-learning,developer-tools,ai Platform:
 any Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
```

### Comparing `dvclive-2.8.1/src/dvclive.egg-info/SOURCES.txt` & `dvclive-2.9.0/src/dvclive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.1/src/dvclive.egg-info/requires.txt` & `dvclive-2.9.0/src/dvclive.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.1/tests/conftest.py` & `dvclive-2.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.1/tests/plots/test_custom.py` & `dvclive-2.9.0/tests/plots/test_custom.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.1/tests/plots/test_image.py` & `dvclive-2.9.0/tests/plots/test_image.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.1/tests/plots/test_metric.py` & `dvclive-2.9.0/tests/plots/test_metric.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.1/tests/plots/test_sklearn.py` & `dvclive-2.9.0/tests/plots/test_sklearn.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.1/tests/test_dvc.py` & `dvclive-2.9.0/tests/test_dvc.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.1/tests/test_frameworks/test_catalyst.py` & `dvclive-2.9.0/tests/test_frameworks/test_catalyst.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.1/tests/test_frameworks/test_fastai.py` & `dvclive-2.9.0/tests/test_frameworks/test_fastai.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.1/tests/test_frameworks/test_huggingface.py` & `dvclive-2.9.0/tests/test_frameworks/test_huggingface.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.1/tests/test_frameworks/test_keras.py` & `dvclive-2.9.0/tests/test_frameworks/test_keras.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.1/tests/test_frameworks/test_lgbm.py` & `dvclive-2.9.0/tests/test_frameworks/test_lgbm.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.1/tests/test_frameworks/test_lightning.py` & `dvclive-2.9.0/tests/test_frameworks/test_lightning.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.1/tests/test_frameworks/test_optuna.py` & `dvclive-2.9.0/tests/test_frameworks/test_optuna.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.1/tests/test_frameworks/test_xgboost.py` & `dvclive-2.9.0/tests/test_frameworks/test_xgboost.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.1/tests/test_main.py` & `dvclive-2.9.0/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.1/tests/test_report.py` & `dvclive-2.9.0/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.1/tests/test_studio.py` & `dvclive-2.9.0/tests/test_studio.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from pathlib import Path
 
 import pytest
+from PIL import Image as ImagePIL
 
 from dvclive import Live
 from dvclive.env import DVC_EXP_BASELINE_REV, DVC_EXP_NAME
-from dvclive.plots import Metric
+from dvclive.plots import Image, Metric
+from dvclive.studio import _adapt_image
 
 
 def test_post_to_studio(tmp_dir, mocked_dvc_repo, mocked_studio_post):
     live = Live(save_dvc_exp=True)
     live.log_param("fooparam", 1)
 
     dvc_path = Path(live.dvc_file).as_posix()
@@ -374,7 +376,40 @@
         timeout=5,
     )
 
 
 def test_post_to_studio_requires_exp(tmp_dir, mocked_dvc_repo, mocked_studio_post):
     assert Live()._studio_events_to_skip == {"start", "data", "done"}
     assert not Live(save_dvc_exp=True)._studio_events_to_skip
+
+
+def test_post_to_studio_images(tmp_dir, mocked_dvc_repo, mocked_studio_post):
+    mocked_post, _ = mocked_studio_post
+
+    live = Live(save_dvc_exp=True)
+    live.log_image("foo.png", ImagePIL.new("RGB", (10, 10), (0, 0, 0)))
+    live.next_step()
+
+    dvc_path = Path(live.dvc_file).as_posix()
+    metrics_path = Path(live.metrics_file).as_posix()
+    foo_path = (Path(live.plots_dir) / Image.subfolder / "foo.png").as_posix()
+
+    mocked_post.assert_called_with(
+        "https://0.0.0.0/api/live",
+        json={
+            "type": "data",
+            "repo_url": "STUDIO_REPO_URL",
+            "baseline_sha": live._baseline_rev,
+            "name": live._exp_name,
+            "step": 0,
+            "metrics": {f"{metrics_path}": {"data": {"step": 0}}},
+            "plots": {
+                f"{dvc_path}::{foo_path}": {"image": _adapt_image(foo_path)},
+            },
+            "client": "dvclive",
+        },
+        headers={
+            "Authorization": "token STUDIO_TOKEN",
+            "Content-type": "application/json",
+        },
+        timeout=5,
+    )
```

### Comparing `dvclive-2.8.1/tests/test_utils.py` & `dvclive-2.9.0/tests/test_utils.py`

 * *Files identical despite different names*

