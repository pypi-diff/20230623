# Comparing `tmp/bob.pad.base-6.0.0.tar.gz` & `tmp/bob.pad.base-6.0.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bob.pad.base-6.0.0.tar", last modified: Thu Jun 22 22:09:47 2023, max compression
+gzip compressed data, was "bob.pad.base-6.0.1b0.tar", last modified: Fri Jun 23 19:44:04 2023, max compression
```

## Comparing `bob.pad.base-6.0.0.tar` & `bob.pad.base-6.0.1b0.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 22:09:47.005558 bob.pad.base-6.0.0/
--rw-rw-rw-   0 root         (0) root         (0)    35147 2023-06-22 22:06:12.000000 bob.pad.base-6.0.0/COPYING
--rw-rw-rw-   0 root         (0) root         (0)      222 2023-06-22 22:06:12.000000 bob.pad.base-6.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2975 2023-06-22 22:09:47.005558 bob.pad.base-6.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1881 2023-06-22 22:06:12.000000 bob.pad.base-6.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 22:09:46.993558 bob.pad.base-6.0.0/doc/
--rw-rw-rw-   0 root         (0) root         (0)     7492 2023-06-22 22:06:12.000000 bob.pad.base-6.0.0/doc/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     4026 2023-06-22 22:06:12.000000 bob.pad.base-6.0.0/doc/features.rst
--rw-rw-rw-   0 root         (0) root         (0)     8712 2023-06-22 22:06:12.000000 bob.pad.base-6.0.0/doc/generic_intro.rst
--rw-rw-rw-   0 root         (0) root         (0)     1702 2023-06-22 22:06:12.000000 bob.pad.base-6.0.0/doc/index.rst
--rw-rw-rw-   0 root         (0) root         (0)    11579 2023-06-22 22:06:12.000000 bob.pad.base-6.0.0/doc/intro.rst
--rw-rw-rw-   0 root         (0) root         (0)     1096 2023-06-22 22:06:12.000000 bob.pad.base-6.0.0/doc/links.rst
--rw-rw-rw-   0 root         (0) root         (0)      783 2023-06-22 22:06:12.000000 bob.pad.base-6.0.0/doc/py_api.rst
--rw-rw-rw-   0 root         (0) root         (0)     1212 2023-06-22 22:06:12.000000 bob.pad.base-6.0.0/doc/setup.rst
--rw-rw-rw-   0 root         (0) root         (0)     3592 2023-06-22 22:06:12.000000 bob.pad.base-6.0.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 22:09:47.005558 bob.pad.base-6.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-06-22 22:06:12.000000 bob.pad.base-6.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 22:09:46.989558 bob.pad.base-6.0.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 22:09:46.993558 bob.pad.base-6.0.0/src/bob/
--rw-rw-rw-   0 root         (0) root         (0)      129 2023-06-22 22:06:12.000000 bob.pad.base-6.0.0/src/bob/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 22:09:46.997558 bob.pad.base-6.0.0/src/bob/pad/
--rw-rw-rw-   0 root         (0) root         (0)      129 2023-06-22 22:06:12.000000 bob.pad.base-6.0.0/src/bob/pad/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 22:09:46.997558 bob.pad.base-6.0.0/src/bob/pad/base/
--rw-rw-rw-   0 root         (0) root         (0)      237 2023-06-22 22:06:12.000000 bob.pad.base-6.0.0/src/bob/pad/base/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 22:09:46.997558 bob.pad.base-6.0.0/src/bob/pad/base/config/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 22:09:23.000000 bob.pad.base-6.0.0/src/bob/pad/base/config/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 22:09:46.997558 bob.pad.base-6.0.0/src/bob/pad/base/database/
--rw-rw-rw-   0 root         (0) root         (0)      613 2023-06-22 22:06:12.000000 bob.pad.base-6.0.0/src/bob/pad/base/database/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2522 2023-06-22 22:06:12.000000 bob.pad.base-6.0.0/src/bob/pad/base/database/csv_dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     9197 2023-06-22 22:06:12.000000 bob.pad.base-6.0.0/src/bob/pad/base/error_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 22:09:46.997558 bob.pad.base-6.0.0/src/bob/pad/base/pipelines/
--rw-rw-rw-   0 root         (0) root         (0)      596 2023-06-22 22:06:12.000000 bob.pad.base-6.0.0/src/bob/pad/base/pipelines/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      749 2023-06-22 22:06:12.000000 bob.pad.base-6.0.0/src/bob/pad/base/pipelines/abstract_classes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 22:09:46.997558 bob.pad.base-6.0.0/src/bob/pad/base/script/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 22:09:23.000000 bob.pad.base-6.0.0/src/bob/pad/base/script/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11557 2023-06-22 22:06:12.000000 bob.pad.base-6.0.0/src/bob/pad/base/script/cross.py
--rw-rw-rw-   0 root         (0) root         (0)     2092 2023-06-22 22:06:12.000000 bob.pad.base-6.0.0/src/bob/pad/base/script/finalize_scores.py
--rw-rw-rw-   0 root         (0) root         (0)      321 2023-06-22 22:06:12.000000 bob.pad.base-6.0.0/src/bob/pad/base/script/pad.py
--rw-rw-rw-   0 root         (0) root         (0)    10122 2023-06-22 22:06:12.000000 bob.pad.base-6.0.0/src/bob/pad/base/script/pad_commands.py
--rw-rw-rw-   0 root         (0) root         (0)    13449 2023-06-22 22:06:12.000000 bob.pad.base-6.0.0/src/bob/pad/base/script/pad_figure.py
--rw-rw-rw-   0 root         (0) root         (0)     8566 2023-06-22 22:06:12.000000 bob.pad.base-6.0.0/src/bob/pad/base/script/run_pipeline.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 22:09:46.997558 bob.pad.base-6.0.0/src/bob.pad.base.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2975 2023-06-22 22:09:46.000000 bob.pad.base-6.0.0/src/bob.pad.base.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2036 2023-06-22 22:09:46.000000 bob.pad.base-6.0.0/src/bob.pad.base.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 22:09:46.000000 bob.pad.base-6.0.0/src/bob.pad.base.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      614 2023-06-22 22:09:46.000000 bob.pad.base-6.0.0/src/bob.pad.base.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 22:09:46.000000 bob.pad.base-6.0.0/src/bob.pad.base.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      483 2023-06-22 22:09:46.000000 bob.pad.base-6.0.0/src/bob.pad.base.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-06-22 22:09:46.000000 bob.pad.base-6.0.0/src/bob.pad.base.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 22:09:46.997558 bob.pad.base-6.0.0/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 22:09:47.001558 bob.pad.base-6.0.0/tests/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 22:09:46.993558 bob.pad.base-6.0.0/tests/data/csv_dataset/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 22:09:46.993558 bob.pad.base-6.0.0/tests/data/csv_dataset/protocol1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 22:09:47.001558 bob.pad.base-6.0.0/tests/data/csv_dataset/protocol1/dev/
--rw-rw-rw-   0 root         (0) root         (0)       88 2023-06-22 22:06:12.000000 bob.pad.base-6.0.0/tests/data/csv_dataset/protocol1/dev/for_attack.csv
--rw-rw-rw-   0 root         (0) root         (0)       59 2023-06-22 22:06:12.000000 bob.pad.base-6.0.0/tests/data/csv_dataset/protocol1/dev/for_real.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 22:09:47.001558 bob.pad.base-6.0.0/tests/data/csv_dataset/protocol1/eval/
--rw-rw-rw-   0 root         (0) root         (0)      121 2023-06-22 22:06:12.000000 bob.pad.base-6.0.0/tests/data/csv_dataset/protocol1/eval/for_attack.csv
--rw-rw-rw-   0 root         (0) root         (0)       88 2023-06-22 22:06:12.000000 bob.pad.base-6.0.0/tests/data/csv_dataset/protocol1/eval/for_real.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 22:09:47.001558 bob.pad.base-6.0.0/tests/data/csv_dataset/protocol1/train/
--rw-rw-rw-   0 root         (0) root         (0)       82 2023-06-22 22:06:12.000000 bob.pad.base-6.0.0/tests/data/csv_dataset/protocol1/train/for_attack.csv
--rw-rw-rw-   0 root         (0) root         (0)       55 2023-06-22 22:06:12.000000 bob.pad.base-6.0.0/tests/data/csv_dataset/protocol1/train/for_real.csv
--rw-rw-rw-   0 root         (0) root         (0)      480 2023-06-22 22:06:12.000000 bob.pad.base-6.0.0/tests/data/csv_dataset.tar.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 22:09:47.001558 bob.pad.base-6.0.0/tests/data/csv_scores/
--rw-rw-rw-   0 root         (0) root         (0)     3140 2023-06-22 22:06:12.000000 bob.pad.base-6.0.0/tests/data/csv_scores/scores-dev.csv
--rw-rw-rw-   0 root         (0) root         (0)     3126 2023-06-22 22:06:12.000000 bob.pad.base-6.0.0/tests/data/csv_scores/scores-eval.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 22:09:47.001558 bob.pad.base-6.0.0/tests/data/licit/
--rw-rw-rw-   0 root         (0) root         (0)   174982 2023-06-22 22:06:12.000000 bob.pad.base-6.0.0/tests/data/licit/scores-dev
--rw-rw-rw-   0 root         (0) root         (0)   174982 2023-06-22 22:06:12.000000 bob.pad.base-6.0.0/tests/data/licit/scores-eval
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 22:09:47.005558 bob.pad.base-6.0.0/tests/data/per_pai_scores/
--rw-rw-rw-   0 root         (0) root         (0)   210266 2023-06-22 22:06:12.000000 bob.pad.base-6.0.0/tests/data/per_pai_scores/scores-dev
--rw-rw-rw-   0 root         (0) root         (0)    94288 2023-06-22 22:06:12.000000 bob.pad.base-6.0.0/tests/data/per_pai_scores/scores-dev-0.hdf5
--rw-rw-rw-   0 root         (0) root         (0)    91992 2023-06-22 22:06:12.000000 bob.pad.base-6.0.0/tests/data/per_pai_scores/scores-dev-1.hdf5
--rw-rw-rw-   0 root         (0) root         (0)   265319 2023-06-22 22:06:12.000000 bob.pad.base-6.0.0/tests/data/per_pai_scores/scores-dev.csv
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-06-22 22:06:12.000000 bob.pad.base-6.0.0/tests/data/scores-dev
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-06-22 22:06:12.000000 bob.pad.base-6.0.0/tests/data/scores-dev-attack
--rw-rw-rw-   0 root         (0) root         (0)       32 2023-06-22 22:06:12.000000 bob.pad.base-6.0.0/tests/data/scores-dev-real
--rw-rw-rw-   0 root         (0) root         (0)       71 2023-06-22 22:06:12.000000 bob.pad.base-6.0.0/tests/data/scores-eval
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-06-22 22:06:12.000000 bob.pad.base-6.0.0/tests/data/scores-eval-attack
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-06-22 22:06:12.000000 bob.pad.base-6.0.0/tests/data/scores-eval-real
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-06-22 22:06:12.000000 bob.pad.base-6.0.0/tests/data/scores-train
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-06-22 22:06:12.000000 bob.pad.base-6.0.0/tests/data/scores-train-attack
--rw-rw-rw-   0 root         (0) root         (0)       34 2023-06-22 22:06:12.000000 bob.pad.base-6.0.0/tests/data/scores-train-real
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 22:09:47.005558 bob.pad.base-6.0.0/tests/data/spoof/
--rw-rw-rw-   0 root         (0) root         (0)   197461 2023-06-22 22:06:12.000000 bob.pad.base-6.0.0/tests/data/spoof/scores-dev
--rw-rw-rw-   0 root         (0) root         (0)   197461 2023-06-22 22:06:12.000000 bob.pad.base-6.0.0/tests/data/spoof/scores-eval
--rw-rw-rw-   0 root         (0) root         (0)     3839 2023-06-22 22:06:12.000000 bob.pad.base-6.0.0/tests/test_commands.py
--rw-rw-rw-   0 root         (0) root         (0)     2776 2023-06-22 22:06:12.000000 bob.pad.base-6.0.0/tests/test_error_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3615 2023-06-22 22:06:12.000000 bob.pad.base-6.0.0/tests/test_pipelines.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:44:04.839956 bob.pad.base-6.0.1b0/
+-rw-rw-rw-   0 root         (0) root         (0)    35147 2023-06-22 22:06:12.000000 bob.pad.base-6.0.1b0/COPYING
+-rw-rw-rw-   0 root         (0) root         (0)      222 2023-06-22 22:06:12.000000 bob.pad.base-6.0.1b0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2977 2023-06-23 19:44:04.839956 bob.pad.base-6.0.1b0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1881 2023-06-23 19:39:17.000000 bob.pad.base-6.0.1b0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:44:04.823957 bob.pad.base-6.0.1b0/doc/
+-rw-rw-rw-   0 root         (0) root         (0)     7492 2023-06-22 22:06:12.000000 bob.pad.base-6.0.1b0/doc/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     4026 2023-06-22 22:06:12.000000 bob.pad.base-6.0.1b0/doc/features.rst
+-rw-rw-rw-   0 root         (0) root         (0)     8712 2023-06-22 22:06:12.000000 bob.pad.base-6.0.1b0/doc/generic_intro.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1702 2023-06-22 22:06:12.000000 bob.pad.base-6.0.1b0/doc/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)    11579 2023-06-22 22:06:12.000000 bob.pad.base-6.0.1b0/doc/intro.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1096 2023-06-22 22:06:12.000000 bob.pad.base-6.0.1b0/doc/links.rst
+-rw-rw-rw-   0 root         (0) root         (0)      783 2023-06-22 22:06:12.000000 bob.pad.base-6.0.1b0/doc/py_api.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1212 2023-06-22 22:06:12.000000 bob.pad.base-6.0.1b0/doc/setup.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3284 2023-06-23 19:39:17.000000 bob.pad.base-6.0.1b0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 19:44:04.839956 bob.pad.base-6.0.1b0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-06-22 22:06:12.000000 bob.pad.base-6.0.1b0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:44:04.815957 bob.pad.base-6.0.1b0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:44:04.823957 bob.pad.base-6.0.1b0/src/bob/
+-rw-rw-rw-   0 root         (0) root         (0)      129 2023-06-22 22:06:12.000000 bob.pad.base-6.0.1b0/src/bob/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:44:04.827957 bob.pad.base-6.0.1b0/src/bob/pad/
+-rw-rw-rw-   0 root         (0) root         (0)      129 2023-06-22 22:06:12.000000 bob.pad.base-6.0.1b0/src/bob/pad/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:44:04.827957 bob.pad.base-6.0.1b0/src/bob/pad/base/
+-rw-rw-rw-   0 root         (0) root         (0)      237 2023-06-22 22:06:12.000000 bob.pad.base-6.0.1b0/src/bob/pad/base/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:44:04.827957 bob.pad.base-6.0.1b0/src/bob/pad/base/config/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-23 19:43:38.000000 bob.pad.base-6.0.1b0/src/bob/pad/base/config/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:44:04.827957 bob.pad.base-6.0.1b0/src/bob/pad/base/database/
+-rw-rw-rw-   0 root         (0) root         (0)      613 2023-06-22 22:06:12.000000 bob.pad.base-6.0.1b0/src/bob/pad/base/database/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2522 2023-06-22 22:06:12.000000 bob.pad.base-6.0.1b0/src/bob/pad/base/database/csv_dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     9197 2023-06-22 22:06:12.000000 bob.pad.base-6.0.1b0/src/bob/pad/base/error_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:44:04.827957 bob.pad.base-6.0.1b0/src/bob/pad/base/pipelines/
+-rw-rw-rw-   0 root         (0) root         (0)      596 2023-06-22 22:06:12.000000 bob.pad.base-6.0.1b0/src/bob/pad/base/pipelines/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      749 2023-06-22 22:06:12.000000 bob.pad.base-6.0.1b0/src/bob/pad/base/pipelines/abstract_classes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:44:04.827957 bob.pad.base-6.0.1b0/src/bob/pad/base/script/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-23 19:43:38.000000 bob.pad.base-6.0.1b0/src/bob/pad/base/script/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11557 2023-06-22 22:06:12.000000 bob.pad.base-6.0.1b0/src/bob/pad/base/script/cross.py
+-rw-rw-rw-   0 root         (0) root         (0)     2092 2023-06-22 22:06:12.000000 bob.pad.base-6.0.1b0/src/bob/pad/base/script/finalize_scores.py
+-rw-rw-rw-   0 root         (0) root         (0)      321 2023-06-22 22:06:12.000000 bob.pad.base-6.0.1b0/src/bob/pad/base/script/pad.py
+-rw-rw-rw-   0 root         (0) root         (0)    10122 2023-06-22 22:06:12.000000 bob.pad.base-6.0.1b0/src/bob/pad/base/script/pad_commands.py
+-rw-rw-rw-   0 root         (0) root         (0)    13449 2023-06-22 22:06:12.000000 bob.pad.base-6.0.1b0/src/bob/pad/base/script/pad_figure.py
+-rw-rw-rw-   0 root         (0) root         (0)     8566 2023-06-22 22:06:12.000000 bob.pad.base-6.0.1b0/src/bob/pad/base/script/run_pipeline.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:44:04.827957 bob.pad.base-6.0.1b0/src/bob.pad.base.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2977 2023-06-23 19:44:04.000000 bob.pad.base-6.0.1b0/src/bob.pad.base.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2036 2023-06-23 19:44:04.000000 bob.pad.base-6.0.1b0/src/bob.pad.base.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 19:44:04.000000 bob.pad.base-6.0.1b0/src/bob.pad.base.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      614 2023-06-23 19:44:04.000000 bob.pad.base-6.0.1b0/src/bob.pad.base.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 19:44:04.000000 bob.pad.base-6.0.1b0/src/bob.pad.base.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      308 2023-06-23 19:44:04.000000 bob.pad.base-6.0.1b0/src/bob.pad.base.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-06-23 19:44:04.000000 bob.pad.base-6.0.1b0/src/bob.pad.base.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:44:04.831956 bob.pad.base-6.0.1b0/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:44:04.831956 bob.pad.base-6.0.1b0/tests/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:44:04.819957 bob.pad.base-6.0.1b0/tests/data/csv_dataset/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:44:04.819957 bob.pad.base-6.0.1b0/tests/data/csv_dataset/protocol1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:44:04.831956 bob.pad.base-6.0.1b0/tests/data/csv_dataset/protocol1/dev/
+-rw-rw-rw-   0 root         (0) root         (0)       88 2023-06-22 22:06:12.000000 bob.pad.base-6.0.1b0/tests/data/csv_dataset/protocol1/dev/for_attack.csv
+-rw-rw-rw-   0 root         (0) root         (0)       59 2023-06-22 22:06:12.000000 bob.pad.base-6.0.1b0/tests/data/csv_dataset/protocol1/dev/for_real.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:44:04.831956 bob.pad.base-6.0.1b0/tests/data/csv_dataset/protocol1/eval/
+-rw-rw-rw-   0 root         (0) root         (0)      121 2023-06-22 22:06:12.000000 bob.pad.base-6.0.1b0/tests/data/csv_dataset/protocol1/eval/for_attack.csv
+-rw-rw-rw-   0 root         (0) root         (0)       88 2023-06-22 22:06:12.000000 bob.pad.base-6.0.1b0/tests/data/csv_dataset/protocol1/eval/for_real.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:44:04.835956 bob.pad.base-6.0.1b0/tests/data/csv_dataset/protocol1/train/
+-rw-rw-rw-   0 root         (0) root         (0)       82 2023-06-22 22:06:12.000000 bob.pad.base-6.0.1b0/tests/data/csv_dataset/protocol1/train/for_attack.csv
+-rw-rw-rw-   0 root         (0) root         (0)       55 2023-06-22 22:06:12.000000 bob.pad.base-6.0.1b0/tests/data/csv_dataset/protocol1/train/for_real.csv
+-rw-rw-rw-   0 root         (0) root         (0)      480 2023-06-22 22:06:12.000000 bob.pad.base-6.0.1b0/tests/data/csv_dataset.tar.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:44:04.835956 bob.pad.base-6.0.1b0/tests/data/csv_scores/
+-rw-rw-rw-   0 root         (0) root         (0)     3140 2023-06-22 22:06:12.000000 bob.pad.base-6.0.1b0/tests/data/csv_scores/scores-dev.csv
+-rw-rw-rw-   0 root         (0) root         (0)     3126 2023-06-22 22:06:12.000000 bob.pad.base-6.0.1b0/tests/data/csv_scores/scores-eval.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:44:04.835956 bob.pad.base-6.0.1b0/tests/data/licit/
+-rw-rw-rw-   0 root         (0) root         (0)   174982 2023-06-22 22:06:12.000000 bob.pad.base-6.0.1b0/tests/data/licit/scores-dev
+-rw-rw-rw-   0 root         (0) root         (0)   174982 2023-06-22 22:06:12.000000 bob.pad.base-6.0.1b0/tests/data/licit/scores-eval
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:44:04.835956 bob.pad.base-6.0.1b0/tests/data/per_pai_scores/
+-rw-rw-rw-   0 root         (0) root         (0)   210266 2023-06-22 22:06:12.000000 bob.pad.base-6.0.1b0/tests/data/per_pai_scores/scores-dev
+-rw-rw-rw-   0 root         (0) root         (0)    94288 2023-06-22 22:06:12.000000 bob.pad.base-6.0.1b0/tests/data/per_pai_scores/scores-dev-0.hdf5
+-rw-rw-rw-   0 root         (0) root         (0)    91992 2023-06-22 22:06:12.000000 bob.pad.base-6.0.1b0/tests/data/per_pai_scores/scores-dev-1.hdf5
+-rw-rw-rw-   0 root         (0) root         (0)   265319 2023-06-22 22:06:12.000000 bob.pad.base-6.0.1b0/tests/data/per_pai_scores/scores-dev.csv
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-06-22 22:06:12.000000 bob.pad.base-6.0.1b0/tests/data/scores-dev
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-06-22 22:06:12.000000 bob.pad.base-6.0.1b0/tests/data/scores-dev-attack
+-rw-rw-rw-   0 root         (0) root         (0)       32 2023-06-22 22:06:12.000000 bob.pad.base-6.0.1b0/tests/data/scores-dev-real
+-rw-rw-rw-   0 root         (0) root         (0)       71 2023-06-22 22:06:12.000000 bob.pad.base-6.0.1b0/tests/data/scores-eval
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-06-22 22:06:12.000000 bob.pad.base-6.0.1b0/tests/data/scores-eval-attack
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-06-22 22:06:12.000000 bob.pad.base-6.0.1b0/tests/data/scores-eval-real
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-06-22 22:06:12.000000 bob.pad.base-6.0.1b0/tests/data/scores-train
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-06-22 22:06:12.000000 bob.pad.base-6.0.1b0/tests/data/scores-train-attack
+-rw-rw-rw-   0 root         (0) root         (0)       34 2023-06-22 22:06:12.000000 bob.pad.base-6.0.1b0/tests/data/scores-train-real
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:44:04.839956 bob.pad.base-6.0.1b0/tests/data/spoof/
+-rw-rw-rw-   0 root         (0) root         (0)   197461 2023-06-22 22:06:12.000000 bob.pad.base-6.0.1b0/tests/data/spoof/scores-dev
+-rw-rw-rw-   0 root         (0) root         (0)   197461 2023-06-22 22:06:12.000000 bob.pad.base-6.0.1b0/tests/data/spoof/scores-eval
+-rw-rw-rw-   0 root         (0) root         (0)     3839 2023-06-22 22:06:12.000000 bob.pad.base-6.0.1b0/tests/test_commands.py
+-rw-rw-rw-   0 root         (0) root         (0)     2776 2023-06-22 22:06:12.000000 bob.pad.base-6.0.1b0/tests/test_error_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3615 2023-06-22 22:06:12.000000 bob.pad.base-6.0.1b0/tests/test_pipelines.py
```

### Comparing `bob.pad.base-6.0.0/COPYING` & `bob.pad.base-6.0.1b0/COPYING`

 * *Files identical despite different names*

### Comparing `bob.pad.base-6.0.0/PKG-INFO` & `bob.pad.base-6.0.1b0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: bob.pad.base
-Version: 6.0.0
+Version: 6.0.1b0
 Summary: A framework for executing the chain of presentation attack detection (PAD) experiments
 Author: Pavel Korshunov
 Author-email: pavel.korshunov@idiap.ch
 License: GPLv3 License
-Project-URL: documentation, https://www.idiap.ch/software/bob/docs/bob/bob.pad.base/v6.0.0/sphinx/
+Project-URL: documentation, https://www.idiap.ch/software/bob/docs/bob/bob.pad.base/master/sphinx/
 Project-URL: homepage, https://pypi.org/project/bob.pad.base/
 Project-URL: repository, https://gitlab.idiap.ch/bob/bob.pad.base
 Project-URL: changelog, https://gitlab.idiap.ch/bob/bob.pad.base/-/releases
 Keywords: PAD framework,grid support,pipeline organization
 Classifier: Framework :: Bob
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -20,17 +20,17 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: qa
 Provides-Extra: doc
 Provides-Extra: test
 License-File: COPYING
 
-[![badge doc](https://img.shields.io/badge/docs-v6.0.0-orange.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.pad.base/v6.0.0/sphinx/index.html)
-[![badge pipeline](https://gitlab.idiap.ch/bob/bob.pad.base/badges/v6.0.0/pipeline.svg)](https://gitlab.idiap.ch/bob/bob.pad.base/commits/v6.0.0)
-[![badge coverage](https://gitlab.idiap.ch/bob/bob.pad.base/badges/v6.0.0/coverage.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.pad.base/v6.0.0/coverage/)
+[![badge doc](https://img.shields.io/badge/docs-latest-orange.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.pad.base/master/sphinx/index.html)
+[![badge pipeline](https://gitlab.idiap.ch/bob/bob.pad.base/badges/master/pipeline.svg)](https://gitlab.idiap.ch/bob/bob.pad.base/commits/master)
+[![badge coverage](https://gitlab.idiap.ch/bob/bob.pad.base/badges/master/coverage.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.pad.base/master/coverage/)
 [![badge gitlab](https://img.shields.io/badge/gitlab-project-0000c0.svg)](https://gitlab.idiap.ch/bob/bob.pad.base)
 
 # Scripts to run anti-spoofing experiments
 
 This package is part of the signal-processing and machine learning toolbox
 [Bob](https://www.idiap.ch/software/bob).
 This package is the base of the `bob.pad` family of packages, which allow to
```

### Comparing `bob.pad.base-6.0.0/README.md` & `bob.pad.base-6.0.1b0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-[![badge doc](https://img.shields.io/badge/docs-v6.0.0-orange.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.pad.base/v6.0.0/sphinx/index.html)
-[![badge pipeline](https://gitlab.idiap.ch/bob/bob.pad.base/badges/v6.0.0/pipeline.svg)](https://gitlab.idiap.ch/bob/bob.pad.base/commits/v6.0.0)
-[![badge coverage](https://gitlab.idiap.ch/bob/bob.pad.base/badges/v6.0.0/coverage.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.pad.base/v6.0.0/coverage/)
+[![badge doc](https://img.shields.io/badge/docs-latest-orange.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.pad.base/master/sphinx/index.html)
+[![badge pipeline](https://gitlab.idiap.ch/bob/bob.pad.base/badges/master/pipeline.svg)](https://gitlab.idiap.ch/bob/bob.pad.base/commits/master)
+[![badge coverage](https://gitlab.idiap.ch/bob/bob.pad.base/badges/master/coverage.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.pad.base/master/coverage/)
 [![badge gitlab](https://img.shields.io/badge/gitlab-project-0000c0.svg)](https://gitlab.idiap.ch/bob/bob.pad.base)
 
 # Scripts to run anti-spoofing experiments
 
 This package is part of the signal-processing and machine learning toolbox
 [Bob](https://www.idiap.ch/software/bob).
 This package is the base of the `bob.pad` family of packages, which allow to
```

### Comparing `bob.pad.base-6.0.0/doc/conf.py` & `bob.pad.base-6.0.1b0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `bob.pad.base-6.0.0/doc/features.rst` & `bob.pad.base-6.0.1b0/doc/features.rst`

 * *Files identical despite different names*

### Comparing `bob.pad.base-6.0.0/doc/generic_intro.rst` & `bob.pad.base-6.0.1b0/doc/generic_intro.rst`

 * *Files identical despite different names*

### Comparing `bob.pad.base-6.0.0/doc/index.rst` & `bob.pad.base-6.0.1b0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `bob.pad.base-6.0.0/doc/intro.rst` & `bob.pad.base-6.0.1b0/doc/intro.rst`

 * *Files identical despite different names*

### Comparing `bob.pad.base-6.0.0/doc/links.rst` & `bob.pad.base-6.0.1b0/doc/links.rst`

 * *Files identical despite different names*

### Comparing `bob.pad.base-6.0.0/doc/py_api.rst` & `bob.pad.base-6.0.1b0/doc/py_api.rst`

 * *Files identical despite different names*

### Comparing `bob.pad.base-6.0.0/doc/setup.rst` & `bob.pad.base-6.0.1b0/doc/setup.rst`

 * *Files identical despite different names*

### Comparing `bob.pad.base-6.0.0/pyproject.toml` & `bob.pad.base-6.0.1b0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
     requires = ["setuptools>=61.0.0", "wheel"]
     build-backend = "setuptools.build_meta"
 
 [project]
     name = "bob.pad.base"
-    version = "6.0.0"
+    version = "6.0.1b0"
     requires-python = ">=3.9"
     description = "A framework for executing the chain of presentation attack detection (PAD) experiments"
     dynamic = ["readme"]
     license = {text = "GPLv3 License"}
     authors = [
     {name = "Pavel Korshunov"},
     {email = "pavel.korshunov@idiap.ch"},
@@ -21,51 +21,51 @@
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Natural Language :: English",
         "Programming Language :: Python",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
     ]
     dependencies = [
-        "bob==12.0.0",
-        "bob.io.base==5.1.0",
-        "bob.measure==6.1.0",
-        "bob.pipelines==4.0.0",
-        "bob.bio.base==8.0.0",
-        "clapper==1.0.1",
-        "click==8.1.3",
-        "click-plugins==1.1.1",
-        "dask==2023.1.0",
-        "matplotlib==3.6.2",
-        "numpy==1.23.5",
-        "scikit-learn==1.1.2",
-        "scipy==1.10.0",
-        "sqlalchemy==1.4.46",
-        "tabulate==0.9.0",
+        "bob",
+        "bob.io.base",
+        "bob.measure",
+        "bob.pipelines",
+        "bob.bio.base",
+        "clapper",
+        "click",
+        "click-plugins",
+        "dask",
+        "matplotlib",
+        "numpy",
+        "scikit-learn",
+        "scipy",
+        "sqlalchemy",
+        "tabulate",
     ]
 
 [project.urls]
-    documentation = "https://www.idiap.ch/software/bob/docs/bob/bob.pad.base/v6.0.0/sphinx/"
+    documentation = "https://www.idiap.ch/software/bob/docs/bob/bob.pad.base/master/sphinx/"
     homepage = "https://pypi.org/project/bob.pad.base/"
     repository = "https://gitlab.idiap.ch/bob/bob.pad.base"
     changelog = "https://gitlab.idiap.ch/bob/bob.pad.base/-/releases"
 
 [project.optional-dependencies]
     qa = ["pre-commit"]
     doc = [
-        "sphinx==5.3.0",
-        "sphinx-rtd-theme==1.1.1",
-        "sphinx-autodoc-typehints==1.21.8",
-        "auto-intersphinx==1.0.2",
-        "sphinxcontrib-programoutput==0.17",
-        "matplotlib==3.6.2",
+        "sphinx",
+        "sphinx_rtd_theme",
+        "sphinx-autodoc-typehints",
+        "auto-intersphinx",
+        "sphinxcontrib-programoutput",
+        "matplotlib",
         ]
     test = [
-        "pytest==7.2.1",
-        "pytest-cov==4.0.0",
-        "coverage==7.0.5",
+        "pytest",
+        "pytest-cov",
+        "coverage",
         ]
 
 [tool.setuptools]
     zip-safe = false
     package-dir = {"" = "src"}
 
 [tool.setuptools.dynamic]
@@ -102,11 +102,7 @@
     addopts = [
         "--import-mode=append",
         "--cov-report=term-missing",
         "--cov=bob.pad.base",
     ]
     junit_logging = "all"
     junit_log_passing_tests = false
-
-[profile]
-    repository_url = "git@gitlab.idiap.ch:bob/dev-profile.git"
-    commit_hash = "ade723be1f11feddb7bece235de32cc98953dc07"
```

### Comparing `bob.pad.base-6.0.0/src/bob/pad/base/database/__init__.py` & `bob.pad.base-6.0.1b0/src/bob/pad/base/database/__init__.py`

 * *Files identical despite different names*

### Comparing `bob.pad.base-6.0.0/src/bob/pad/base/database/csv_dataset.py` & `bob.pad.base-6.0.1b0/src/bob/pad/base/database/csv_dataset.py`

 * *Files identical despite different names*

### Comparing `bob.pad.base-6.0.0/src/bob/pad/base/error_utils.py` & `bob.pad.base-6.0.1b0/src/bob/pad/base/error_utils.py`

 * *Files identical despite different names*

### Comparing `bob.pad.base-6.0.0/src/bob/pad/base/pipelines/__init__.py` & `bob.pad.base-6.0.1b0/src/bob/pad/base/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `bob.pad.base-6.0.0/src/bob/pad/base/pipelines/abstract_classes.py` & `bob.pad.base-6.0.1b0/src/bob/pad/base/pipelines/abstract_classes.py`

 * *Files identical despite different names*

### Comparing `bob.pad.base-6.0.0/src/bob/pad/base/script/cross.py` & `bob.pad.base-6.0.1b0/src/bob/pad/base/script/cross.py`

 * *Files identical despite different names*

### Comparing `bob.pad.base-6.0.0/src/bob/pad/base/script/finalize_scores.py` & `bob.pad.base-6.0.1b0/src/bob/pad/base/script/finalize_scores.py`

 * *Files identical despite different names*

### Comparing `bob.pad.base-6.0.0/src/bob/pad/base/script/pad_commands.py` & `bob.pad.base-6.0.1b0/src/bob/pad/base/script/pad_commands.py`

 * *Files identical despite different names*

### Comparing `bob.pad.base-6.0.0/src/bob/pad/base/script/pad_figure.py` & `bob.pad.base-6.0.1b0/src/bob/pad/base/script/pad_figure.py`

 * *Files identical despite different names*

### Comparing `bob.pad.base-6.0.0/src/bob/pad/base/script/run_pipeline.py` & `bob.pad.base-6.0.1b0/src/bob/pad/base/script/run_pipeline.py`

 * *Files identical despite different names*

### Comparing `bob.pad.base-6.0.0/src/bob.pad.base.egg-info/PKG-INFO` & `bob.pad.base-6.0.1b0/src/bob.pad.base.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: bob.pad.base
-Version: 6.0.0
+Version: 6.0.1b0
 Summary: A framework for executing the chain of presentation attack detection (PAD) experiments
 Author: Pavel Korshunov
 Author-email: pavel.korshunov@idiap.ch
 License: GPLv3 License
-Project-URL: documentation, https://www.idiap.ch/software/bob/docs/bob/bob.pad.base/v6.0.0/sphinx/
+Project-URL: documentation, https://www.idiap.ch/software/bob/docs/bob/bob.pad.base/master/sphinx/
 Project-URL: homepage, https://pypi.org/project/bob.pad.base/
 Project-URL: repository, https://gitlab.idiap.ch/bob/bob.pad.base
 Project-URL: changelog, https://gitlab.idiap.ch/bob/bob.pad.base/-/releases
 Keywords: PAD framework,grid support,pipeline organization
 Classifier: Framework :: Bob
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -20,17 +20,17 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: qa
 Provides-Extra: doc
 Provides-Extra: test
 License-File: COPYING
 
-[![badge doc](https://img.shields.io/badge/docs-v6.0.0-orange.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.pad.base/v6.0.0/sphinx/index.html)
-[![badge pipeline](https://gitlab.idiap.ch/bob/bob.pad.base/badges/v6.0.0/pipeline.svg)](https://gitlab.idiap.ch/bob/bob.pad.base/commits/v6.0.0)
-[![badge coverage](https://gitlab.idiap.ch/bob/bob.pad.base/badges/v6.0.0/coverage.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.pad.base/v6.0.0/coverage/)
+[![badge doc](https://img.shields.io/badge/docs-latest-orange.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.pad.base/master/sphinx/index.html)
+[![badge pipeline](https://gitlab.idiap.ch/bob/bob.pad.base/badges/master/pipeline.svg)](https://gitlab.idiap.ch/bob/bob.pad.base/commits/master)
+[![badge coverage](https://gitlab.idiap.ch/bob/bob.pad.base/badges/master/coverage.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.pad.base/master/coverage/)
 [![badge gitlab](https://img.shields.io/badge/gitlab-project-0000c0.svg)](https://gitlab.idiap.ch/bob/bob.pad.base)
 
 # Scripts to run anti-spoofing experiments
 
 This package is part of the signal-processing and machine learning toolbox
 [Bob](https://www.idiap.ch/software/bob).
 This package is the base of the `bob.pad` family of packages, which allow to
```

### Comparing `bob.pad.base-6.0.0/src/bob.pad.base.egg-info/SOURCES.txt` & `bob.pad.base-6.0.1b0/src/bob.pad.base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bob.pad.base-6.0.0/src/bob.pad.base.egg-info/entry_points.txt` & `bob.pad.base-6.0.1b0/src/bob.pad.base.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `bob.pad.base-6.0.0/tests/data/csv_scores/scores-dev.csv` & `bob.pad.base-6.0.1b0/tests/data/csv_scores/scores-dev.csv`

 * *Files identical despite different names*

### Comparing `bob.pad.base-6.0.0/tests/data/csv_scores/scores-eval.csv` & `bob.pad.base-6.0.1b0/tests/data/csv_scores/scores-eval.csv`

 * *Files identical despite different names*

### Comparing `bob.pad.base-6.0.0/tests/data/licit/scores-dev` & `bob.pad.base-6.0.1b0/tests/data/licit/scores-dev`

 * *Files identical despite different names*

### Comparing `bob.pad.base-6.0.0/tests/data/licit/scores-eval` & `bob.pad.base-6.0.1b0/tests/data/licit/scores-eval`

 * *Files identical despite different names*

### Comparing `bob.pad.base-6.0.0/tests/data/per_pai_scores/scores-dev` & `bob.pad.base-6.0.1b0/tests/data/per_pai_scores/scores-dev`

 * *Files identical despite different names*

### Comparing `bob.pad.base-6.0.0/tests/data/per_pai_scores/scores-dev-0.hdf5` & `bob.pad.base-6.0.1b0/tests/data/per_pai_scores/scores-dev-0.hdf5`

 * *Files identical despite different names*

### Comparing `bob.pad.base-6.0.0/tests/data/per_pai_scores/scores-dev-1.hdf5` & `bob.pad.base-6.0.1b0/tests/data/per_pai_scores/scores-dev-1.hdf5`

 * *Files identical despite different names*

### Comparing `bob.pad.base-6.0.0/tests/data/per_pai_scores/scores-dev.csv` & `bob.pad.base-6.0.1b0/tests/data/per_pai_scores/scores-dev.csv`

 * *Files identical despite different names*

### Comparing `bob.pad.base-6.0.0/tests/data/spoof/scores-dev` & `bob.pad.base-6.0.1b0/tests/data/spoof/scores-dev`

 * *Files identical despite different names*

### Comparing `bob.pad.base-6.0.0/tests/data/spoof/scores-eval` & `bob.pad.base-6.0.1b0/tests/data/spoof/scores-eval`

 * *Files identical despite different names*

### Comparing `bob.pad.base-6.0.0/tests/test_commands.py` & `bob.pad.base-6.0.1b0/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `bob.pad.base-6.0.0/tests/test_error_utils.py` & `bob.pad.base-6.0.1b0/tests/test_error_utils.py`

 * *Files identical despite different names*

### Comparing `bob.pad.base-6.0.0/tests/test_pipelines.py` & `bob.pad.base-6.0.1b0/tests/test_pipelines.py`

 * *Files identical despite different names*

