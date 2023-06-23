# Comparing `tmp/taipy-core-2.3.0.dev6.tar.gz` & `tmp/taipy-core-3.0.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taipy-core-2.3.0.dev6.tar", last modified: Fri Jun 16 11:36:36 2023, max compression
+gzip compressed data, was "taipy-core-3.0.0.dev0.tar", last modified: Fri Jun 23 09:48:19 2023, max compression
```

## Comparing `taipy-core-2.3.0.dev6.tar` & `taipy-core-3.0.0.dev0.tar`

### file list

```diff
@@ -1,195 +1,196 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:36:36.609575 taipy-core-2.3.0.dev6/
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-06-16 11:36:36.609575 taipy-core-2.3.0.dev6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 11:36:36.609575 taipy-core-2.3.0.dev6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-06-16 11:36:28.000000 taipy-core-2.3.0.dev6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:36:36.581573 taipy-core-2.3.0.dev6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:36:36.581573 taipy-core-2.3.0.dev6/src/taipy/
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:36:36.581573 taipy-core-2.3.0.dev6/src/taipy/core/
--rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:36:36.585573 taipy-core-2.3.0.dev6/src/taipy/core/_backup/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/_backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/_backup/_backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/_core_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:36:36.585573 taipy-core-2.3.0.dev6/src/taipy/core/_entity/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/_entity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/_entity/_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/_entity/_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/_entity/_entity_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/_entity/_labeled.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/_entity/_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/_entity/_reload.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/_entity/_submittable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:36:36.585573 taipy-core-2.3.0.dev6/src/taipy/core/_manager/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/_manager/_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/_manager/_manager_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:36:36.585573 taipy-core-2.3.0.dev6/src/taipy/core/_orchestrator/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/_orchestrator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/_orchestrator/_abstract_orchestrator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:36:36.585573 taipy-core-2.3.0.dev6/src/taipy/core/_orchestrator/_dispatcher/
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/_orchestrator/_dispatcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/_orchestrator/_dispatcher/_development_job_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/_orchestrator/_dispatcher/_job_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/_orchestrator/_dispatcher/_standalone_job_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/_orchestrator/_orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/_orchestrator/_orchestrator_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/_orchestrator/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:36:36.589573 taipy-core-2.3.0.dev6/src/taipy/core/_repository/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/_repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11894 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/_repository/_filesystem_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     6200 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/_repository/_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/_repository/_repository_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/_repository/_repository_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/_repository/_sql_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    19696 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/_repository/_sql_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:36:36.589573 taipy-core-2.3.0.dev6/src/taipy/core/_version/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/_version/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:36:36.589573 taipy-core-2.3.0.dev6/src/taipy/core/_version/_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/_version/_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/_version/_cli/_bcolor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8976 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/_version/_cli/_version_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/_version/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/_version/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/_version/_version_fs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     8951 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/_version/_version_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/_version/_version_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/_version/_version_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/_version/_version_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/_version/_version_repository_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/_version/_version_sql_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:36:36.589573 taipy-core-2.3.0.dev6/src/taipy/core/common/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/common/_listattributes.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/common/_repr_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/common/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/common/_warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/common/default_custom_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/common/warn_if_inputs_not_ready.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:36:36.593574 taipy-core-2.3.0.dev6/src/taipy/core/config/
--rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:36:36.593574 taipy-core-2.3.0.dev6/src/taipy/core/config/checkers/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/config/checkers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/config/checkers/_config_id_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)    11456 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/config/checkers/_data_node_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/config/checkers/_global_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/config/checkers/_job_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/config/checkers/_pipeline_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/config/checkers/_scenario_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/config/checkers/_task_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)    14637 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/config/config.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/config/core_section.py
--rw-r--r--   0 runner    (1001) docker     (123)    49075 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/config/data_node_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/config/job_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/config/pipeline_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11621 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/config/scenario_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9467 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/config/task_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:36:36.593574 taipy-core-2.3.0.dev6/src/taipy/core/cycle/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/cycle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/cycle/_cycle_fs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/cycle/_cycle_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/cycle/_cycle_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/cycle/_cycle_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/cycle/_cycle_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/cycle/_cycle_repository_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/cycle/_cycle_sql_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/cycle/cycle.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/cycle/cycle_id.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:36:36.597574 taipy-core-2.3.0.dev6/src/taipy/core/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/data/_data_fs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/data/_data_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/data/_data_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/data/_data_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    13249 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/data/_data_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/data/_data_repository_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/data/_data_sql_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/data/_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/data/abstract_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9905 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/data/abstract_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     9586 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/data/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)    21520 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/data/data_node.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/data/data_node_id.py
--rw-r--r--   0 runner    (1001) docker     (123)    13905 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/data/excel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/data/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/data/in_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     7672 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/data/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     9057 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/data/mongo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/data/operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11994 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/data/parquet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/data/pickle.py
--rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/data/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     8189 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/data/sql_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:36:36.597574 taipy-core-2.3.0.dev6/src/taipy/core/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8378 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:36:36.601574 taipy-core-2.3.0.dev6/src/taipy/core/job/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/job/_job_fs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/job/_job_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/job/_job_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/job/_job_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/job/_job_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/job/_job_repository_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/job/_job_sql_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     9939 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/job/job.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/job/job_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/job/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:36:36.601574 taipy-core-2.3.0.dev6/src/taipy/core/notification/
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/notification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/notification/core_event_consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/notification/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/notification/notifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/notification/registration.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/notification/registration_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/notification/topic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:36:36.605574 taipy-core-2.3.0.dev6/src/taipy/core/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/pipeline/_pipeline_fs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     7292 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/pipeline/_pipeline_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/pipeline/_pipeline_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/pipeline/_pipeline_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/pipeline/_pipeline_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/pipeline/_pipeline_repository_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/pipeline/_pipeline_sql_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    10549 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/pipeline/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/pipeline/pipeline_id.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:36:36.605574 taipy-core-2.3.0.dev6/src/taipy/core/scenario/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/scenario/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/scenario/_scenario_fs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    13561 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/scenario/_scenario_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/scenario/_scenario_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/scenario/_scenario_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/scenario/_scenario_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/scenario/_scenario_repository_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/scenario/_scenario_sql_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/scenario/scenario.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/scenario/scenario_id.py
--rw-r--r--   0 runner    (1001) docker     (123)    26101 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/taipy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:36:36.609575 taipy-core-2.3.0.dev6/src/taipy/core/task/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/task/_task_fs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/task/_task_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/task/_task_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/task/_task_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/task/_task_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/task/_task_repository_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/task/_task_sql_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/task/task.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/task/task_id.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/src/taipy/core/version.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:36:36.609575 taipy-core-2.3.0.dev6/src/taipy_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-06-16 11:36:36.000000 taipy-core-2.3.0.dev6/src/taipy_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-06-16 11:36:36.000000 taipy-core-2.3.0.dev6/src/taipy_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 11:36:36.000000 taipy-core-2.3.0.dev6/src/taipy_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 11:36:29.000000 taipy-core-2.3.0.dev6/src/taipy_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-16 11:36:36.000000 taipy-core-2.3.0.dev6/src/taipy_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-16 11:36:36.000000 taipy-core-2.3.0.dev6/src/taipy_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:36:36.609575 taipy-core-2.3.0.dev6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9955 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/tests/test_complex_application.py
--rw-r--r--   0 runner    (1001) docker     (123)    30198 2023-06-16 11:36:21.000000 taipy-core-2.3.0.dev6/tests/test_taipy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:48:18.999586 taipy-core-3.0.0.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-06-23 09:48:18.999586 taipy-core-3.0.0.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 09:48:18.999586 taipy-core-3.0.0.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-06-23 09:48:10.000000 taipy-core-3.0.0.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:48:18.971586 taipy-core-3.0.0.dev0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:48:18.971586 taipy-core-3.0.0.dev0/src/taipy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:48:18.975586 taipy-core-3.0.0.dev0/src/taipy/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:48:18.975586 taipy-core-3.0.0.dev0/src/taipy/core/_backup/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_backup/_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_core_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:48:18.975586 taipy-core-3.0.0.dev0/src/taipy/core/_entity/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_entity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_entity/_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_entity/_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_entity/_entity_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_entity/_labeled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_entity/_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_entity/_reload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_entity/_submittable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:48:18.975586 taipy-core-3.0.0.dev0/src/taipy/core/_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_manager/_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_manager/_manager_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:48:18.975586 taipy-core-3.0.0.dev0/src/taipy/core/_orchestrator/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_orchestrator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_orchestrator/_abstract_orchestrator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:48:18.979586 taipy-core-3.0.0.dev0/src/taipy/core/_orchestrator/_dispatcher/
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_orchestrator/_dispatcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_orchestrator/_dispatcher/_development_job_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_orchestrator/_dispatcher/_job_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_orchestrator/_dispatcher/_standalone_job_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_orchestrator/_orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_orchestrator/_orchestrator_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_orchestrator/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:48:18.979586 taipy-core-3.0.0.dev0/src/taipy/core/_repository/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11894 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_repository/_filesystem_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6200 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_repository/_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_repository/_repository_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_repository/_repository_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_repository/_sql_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19696 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_repository/_sql_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:48:18.979586 taipy-core-3.0.0.dev0/src/taipy/core/_version/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_version/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:48:18.979586 taipy-core-3.0.0.dev0/src/taipy/core/_version/_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_version/_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_version/_cli/_bcolor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8976 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_version/_cli/_version_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_version/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_version/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_version/_version_fs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8951 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_version/_version_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_version/_version_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_version/_version_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_version/_version_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_version/_version_repository_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_version/_version_sql_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:48:18.983586 taipy-core-3.0.0.dev0/src/taipy/core/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/common/_listattributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/common/_repr_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/common/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/common/_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/common/default_custom_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/common/warn_if_inputs_not_ready.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:48:18.983586 taipy-core-3.0.0.dev0/src/taipy/core/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:48:18.983586 taipy-core-3.0.0.dev0/src/taipy/core/config/checkers/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/config/checkers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/config/checkers/_config_id_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11456 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/config/checkers/_data_node_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/config/checkers/_global_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/config/checkers/_job_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/config/checkers/_pipeline_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/config/checkers/_scenario_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/config/checkers/_task_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14637 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/config/config.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/config/core_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49075 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/config/data_node_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/config/job_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/config/pipeline_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11621 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/config/scenario_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9467 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/config/task_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:48:18.987586 taipy-core-3.0.0.dev0/src/taipy/core/cycle/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/cycle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/cycle/_cycle_fs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/cycle/_cycle_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/cycle/_cycle_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/cycle/_cycle_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/cycle/_cycle_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/cycle/_cycle_repository_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/cycle/_cycle_sql_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/cycle/cycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/cycle/cycle_id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:48:18.987586 taipy-core-3.0.0.dev0/src/taipy/core/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/data/_data_fs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/data/_data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/data/_data_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/data/_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13249 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/data/_data_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/data/_data_repository_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/data/_data_sql_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/data/_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/data/abstract_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9905 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/data/abstract_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9586 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/data/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21520 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/data/data_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/data/data_node_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13905 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/data/excel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/data/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/data/in_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7672 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/data/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9057 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/data/mongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/data/operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11994 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/data/parquet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/data/pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/data/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8189 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/data/sql_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:48:18.991586 taipy-core-3.0.0.dev0/src/taipy/core/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8378 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:48:18.991586 taipy-core-3.0.0.dev0/src/taipy/core/job/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/job/_job_fs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/job/_job_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/job/_job_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/job/_job_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/job/_job_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/job/_job_repository_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/job/_job_sql_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9939 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/job/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/job/job_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/job/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:48:18.991586 taipy-core-3.0.0.dev0/src/taipy/core/notification/
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/notification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/notification/core_event_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/notification/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/notification/notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/notification/registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/notification/registration_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/notification/topic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:48:18.995586 taipy-core-3.0.0.dev0/src/taipy/core/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/pipeline/_pipeline_fs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7520 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/pipeline/_pipeline_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/pipeline/_pipeline_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/pipeline/_pipeline_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/pipeline/_pipeline_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/pipeline/_pipeline_repository_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/pipeline/_pipeline_sql_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10549 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/pipeline/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/pipeline/pipeline_id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:48:18.995586 taipy-core-3.0.0.dev0/src/taipy/core/scenario/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/scenario/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/scenario/_scenario_fs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14080 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/scenario/_scenario_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/scenario/_scenario_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/scenario/_scenario_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/scenario/_scenario_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/scenario/_scenario_repository_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/scenario/_scenario_sql_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/scenario/scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/scenario/scenario_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27303 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/taipy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:48:18.999586 taipy-core-3.0.0.dev0/src/taipy/core/task/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/task/_task_fs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/task/_task_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/task/_task_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/task/_task_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/task/_task_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/task/_task_repository_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/task/_task_sql_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/task/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/task/task_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/version.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:48:18.999586 taipy-core-3.0.0.dev0/src/taipy_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-06-23 09:48:18.000000 taipy-core-3.0.0.dev0/src/taipy_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-06-23 09:48:18.000000 taipy-core-3.0.0.dev0/src/taipy_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 09:48:18.000000 taipy-core-3.0.0.dev0/src/taipy_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 09:48:11.000000 taipy-core-3.0.0.dev0/src/taipy_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-23 09:48:18.000000 taipy-core-3.0.0.dev0/src/taipy_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-23 09:48:18.000000 taipy-core-3.0.0.dev0/src/taipy_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:48:18.999586 taipy-core-3.0.0.dev0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9955 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/tests/test_complex_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33298 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/tests/test_taipy.py
```

### Comparing `taipy-core-2.3.0.dev6/LICENSE` & `taipy-core-3.0.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/PKG-INFO` & `taipy-core-3.0.0.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipy-core
-Version: 2.3.0.dev6
+Version: 3.0.0.dev0
 Summary: A Python library to build powerful and customized data-driven back-end applications.
 Home-page: https://github.com/avaiga/taipy-core
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy-core
 Classifier: Intended Audience :: Developers
```

### Comparing `taipy-core-2.3.0.dev6/README.md` & `taipy-core-3.0.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/setup.py` & `taipy-core-3.0.0.dev0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     "pyarrow>=10.0.1,<11.0",
     "networkx>=2.6,<3.0",
     "openpyxl>=3.0.7,<3.1",
     "modin[dask]>=0.16.2,<1.0",
     "pymongo>=4.2.0,<5.0",
     "sqlalchemy>2.0",
     "toml>=0.10,<0.11",
-    "taipy-config==2.3.0.dev3",
+    "taipy-config==3.0.0.dev0",
 ]
 
 test_requirements = ["pytest>=3.8"]
 
 extras_require = {
     "fastparquet": ["fastparquet==2022.11.0"],
     "mssql": ["pyodbc>=4,<4.1"],
```

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/_backup/__init__.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_backup/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/_backup/_backup.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_backup/_backup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 # an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
 
 
 import os
 
-from taipy import Config
+from taipy.config import Config
 
 __BACKUP_FILE_PATH_ENVIRONMENT_VARIABLE_NAME = "TAIPY_BACKUP_FILE_PATH"
 
 
 def _init_backup_file_with_storage_folder():
     if preserve_file_path := os.getenv(__BACKUP_FILE_PATH_ENVIRONMENT_VARIABLE_NAME):
         with open(preserve_file_path, "a") as f:
```

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/_core.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_core.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/_core_cli.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_core_cli.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/_entity/__init__.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_entity/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/_entity/_dag.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_entity/_dag.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/_entity/_entity.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_entity/_entity.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/_entity/_entity_ids.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_entity/_entity_ids.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/_entity/_labeled.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_entity/_labeled.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,17 +40,17 @@
         return self._get_explicit_label() or self._generate_label(True)
 
     def _generate_label(self, simple=False) -> str:
         ls = []
         if not simple:
             if owner_id := self._get_owner_id():
                 if getattr(self, "id") != owner_id:
-                    from ... import core
+                    from ... import core as tp
 
-                    owner = core.get(owner_id)
+                    owner = tp.get(owner_id)
                     ls.append(owner.get_label())
         ls.append(self._generate_entity_label())
         return self.__LABEL_SEPARATOR.join(ls)
 
     def _get_explicit_label(self) -> Optional[str]:
         if hasattr(self, "_properties"):
             return getattr(self, "_properties").get("label")
```

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/_entity/_properties.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_entity/_properties.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/_entity/_reload.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_entity/_reload.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/_entity/_submittable.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_entity/_submittable.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/_manager/__init__.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/_manager/_manager.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_manager/_manager.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/_manager/_manager_factory.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_manager/_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/_orchestrator/__init__.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_orchestrator/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/_orchestrator/_abstract_orchestrator.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_orchestrator/_abstract_orchestrator.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/_orchestrator/_dispatcher/__init__.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_orchestrator/_dispatcher/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/_orchestrator/_dispatcher/_development_job_dispatcher.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_orchestrator/_dispatcher/_development_job_dispatcher.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/_orchestrator/_dispatcher/_job_dispatcher.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_orchestrator/_dispatcher/_job_dispatcher.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/_orchestrator/_dispatcher/_standalone_job_dispatcher.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_orchestrator/_dispatcher/_standalone_job_dispatcher.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/_orchestrator/_orchestrator.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_orchestrator/_orchestrator.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/_orchestrator/_orchestrator_factory.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_orchestrator/_orchestrator_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/_orchestrator/utils.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_orchestrator/utils.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/_repository/__init__.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_repository/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/_repository/_filesystem_repository.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_repository/_filesystem_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/_repository/_repository.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_repository/_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/_repository/_repository_adapter.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_repository/_repository_adapter.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/_repository/_repository_factory.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_repository/_repository_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/_repository/_sql_model.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_repository/_sql_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/_repository/_sql_repository.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_repository/_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/_version/__init__.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_version/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/_version/_cli/__init__.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_version/_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/_version/_cli/_bcolor.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_version/_cli/_bcolor.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/_version/_cli/_version_cli.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_version/_cli/_version_cli.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/_version/_utils.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_version/_utils.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/_version/_version.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_version/_version.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/_version/_version_fs_repository.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_version/_version_fs_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/_version/_version_manager.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_version/_version_manager.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/_version/_version_manager_factory.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_version/_version_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/_version/_version_model.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_version/_version_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/_version/_version_repository.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_version/_version_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/_version/_version_repository_factory.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_version/_version_repository_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/_version/_version_sql_repository.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_version/_version_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/common/__init__.py` & `taipy-core-3.0.0.dev0/src/taipy/core/common/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/common/_listattributes.py` & `taipy-core-3.0.0.dev0/src/taipy/core/common/_listattributes.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/common/_repr_enum.py` & `taipy-core-3.0.0.dev0/src/taipy/core/common/_repr_enum.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/common/_utils.py` & `taipy-core-3.0.0.dev0/src/taipy/core/common/_utils.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/common/_warnings.py` & `taipy-core-3.0.0.dev0/src/taipy/core/common/_warnings.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/common/default_custom_document.py` & `taipy-core-3.0.0.dev0/src/taipy/core/common/default_custom_document.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/common/warn_if_inputs_not_ready.py` & `taipy-core-3.0.0.dev0/src/taipy/core/common/warn_if_inputs_not_ready.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/config/__init__.py` & `taipy-core-3.0.0.dev0/src/taipy/core/config/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/config/checkers/__init__.py` & `taipy-core-3.0.0.dev0/src/taipy/core/config/checkers/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/config/checkers/_config_id_checker.py` & `taipy-core-3.0.0.dev0/src/taipy/core/config/checkers/_config_id_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/config/checkers/_data_node_config_checker.py` & `taipy-core-3.0.0.dev0/src/taipy/core/config/checkers/_data_node_config_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/config/checkers/_global_config_checker.py` & `taipy-core-3.0.0.dev0/src/taipy/core/config/checkers/_global_config_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/config/checkers/_job_config_checker.py` & `taipy-core-3.0.0.dev0/src/taipy/core/config/checkers/_job_config_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/config/checkers/_pipeline_config_checker.py` & `taipy-core-3.0.0.dev0/src/taipy/core/config/checkers/_pipeline_config_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/config/checkers/_scenario_config_checker.py` & `taipy-core-3.0.0.dev0/src/taipy/core/config/checkers/_scenario_config_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/config/checkers/_task_config_checker.py` & `taipy-core-3.0.0.dev0/src/taipy/core/config/checkers/_task_config_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/config/config.schema.json` & `taipy-core-3.0.0.dev0/src/taipy/core/config/config.schema.json`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/config/core_section.py` & `taipy-core-3.0.0.dev0/src/taipy/core/config/core_section.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,14 +14,31 @@
 
 from taipy.config import Config, UniqueSection
 from taipy.config._config import _Config
 from taipy.config.common._template_handler import _TemplateHandler as _tpl
 
 
 class CoreSection(UniqueSection):
+    """
+    Configuration fields needed to run the `Core^` service.
+
+
+    Attributes:
+        mode (str): The Taipy operating mode. By default, the `Core^` service runs in "development" mode.
+            An "experiment" and a "production" mode are also available. Please refer to the
+            [Versioning management](../../../manuals/core/versioning/index.md) documentation page.
+        version_number (str)): The identifier of the user application version. Please refer to the
+            [Versioning management](../../../manuals/core/versioning/index.md) documentation page.
+        force (bool): Parameter to force the application run even if there are some conflicts in the
+            configuration.
+        clean_entities(bool): Parameter to remove all entities (from previous run) before running
+            the application.
+        **properties (dict[str, any]): A dictionary of additional properties.
+    """
+
     name = "CORE"
     _MODE_KEY = "mode"
     _DEVELOPMENT_MODE = "development"
     _EXPERIMENT_MODE = "experiment"
     _PRODUCTION_MODE = "production"
     _DEFAULT_MODE = _DEVELOPMENT_MODE
     _VERSION_NUMBER_KEY = "version_number"
```

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/config/data_node_config.py` & `taipy-core-3.0.0.dev0/src/taipy/core/config/data_node_config.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/config/job_config.py` & `taipy-core-3.0.0.dev0/src/taipy/core/config/job_config.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/config/pipeline_config.py` & `taipy-core-3.0.0.dev0/src/taipy/core/config/pipeline_config.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/config/scenario_config.py` & `taipy-core-3.0.0.dev0/src/taipy/core/config/scenario_config.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/config/task_config.py` & `taipy-core-3.0.0.dev0/src/taipy/core/config/task_config.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/cycle/__init__.py` & `taipy-core-3.0.0.dev0/src/taipy/core/cycle/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/cycle/_cycle_fs_repository.py` & `taipy-core-3.0.0.dev0/src/taipy/core/cycle/_cycle_fs_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/cycle/_cycle_manager.py` & `taipy-core-3.0.0.dev0/src/taipy/core/cycle/_cycle_manager.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/cycle/_cycle_manager_factory.py` & `taipy-core-3.0.0.dev0/src/taipy/core/cycle/_cycle_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/cycle/_cycle_model.py` & `taipy-core-3.0.0.dev0/src/taipy/core/cycle/_cycle_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/cycle/_cycle_repository.py` & `taipy-core-3.0.0.dev0/src/taipy/core/cycle/_cycle_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/cycle/_cycle_repository_factory.py` & `taipy-core-3.0.0.dev0/src/taipy/core/cycle/_cycle_repository_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/cycle/_cycle_sql_repository.py` & `taipy-core-3.0.0.dev0/src/taipy/core/cycle/_cycle_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/cycle/cycle.py` & `taipy-core-3.0.0.dev0/src/taipy/core/cycle/cycle.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/cycle/cycle_id.py` & `taipy-core-3.0.0.dev0/src/taipy/core/cycle/cycle_id.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/data/__init__.py` & `taipy-core-3.0.0.dev0/src/taipy/core/data/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/data/_data_fs_repository.py` & `taipy-core-3.0.0.dev0/src/taipy/core/data/_data_fs_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/data/_data_manager.py` & `taipy-core-3.0.0.dev0/src/taipy/core/data/_data_manager.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/data/_data_manager_factory.py` & `taipy-core-3.0.0.dev0/src/taipy/core/data/_data_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/data/_data_model.py` & `taipy-core-3.0.0.dev0/src/taipy/core/data/_data_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/data/_data_repository.py` & `taipy-core-3.0.0.dev0/src/taipy/core/data/_data_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/data/_data_repository_factory.py` & `taipy-core-3.0.0.dev0/src/taipy/core/data/_data_repository_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/data/_data_sql_repository.py` & `taipy-core-3.0.0.dev0/src/taipy/core/data/_data_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/data/_filter.py` & `taipy-core-3.0.0.dev0/src/taipy/core/data/_filter.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/data/abstract_file.py` & `taipy-core-3.0.0.dev0/src/taipy/core/data/abstract_file.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/data/abstract_sql.py` & `taipy-core-3.0.0.dev0/src/taipy/core/data/abstract_sql.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/data/csv.py` & `taipy-core-3.0.0.dev0/src/taipy/core/data/csv.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/data/data_node.py` & `taipy-core-3.0.0.dev0/src/taipy/core/data/data_node.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/data/data_node_id.py` & `taipy-core-3.0.0.dev0/src/taipy/core/data/data_node_id.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/data/excel.py` & `taipy-core-3.0.0.dev0/src/taipy/core/data/excel.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/data/generic.py` & `taipy-core-3.0.0.dev0/src/taipy/core/data/generic.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/data/in_memory.py` & `taipy-core-3.0.0.dev0/src/taipy/core/data/in_memory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/data/json.py` & `taipy-core-3.0.0.dev0/src/taipy/core/data/json.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/data/mongo.py` & `taipy-core-3.0.0.dev0/src/taipy/core/data/mongo.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/data/operator.py` & `taipy-core-3.0.0.dev0/src/taipy/core/data/operator.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/data/parquet.py` & `taipy-core-3.0.0.dev0/src/taipy/core/data/parquet.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/data/pickle.py` & `taipy-core-3.0.0.dev0/src/taipy/core/data/pickle.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/data/sql.py` & `taipy-core-3.0.0.dev0/src/taipy/core/data/sql.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/data/sql_table.py` & `taipy-core-3.0.0.dev0/src/taipy/core/data/sql_table.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/exceptions/__init__.py` & `taipy-core-3.0.0.dev0/src/taipy/core/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/exceptions/exceptions.py` & `taipy-core-3.0.0.dev0/src/taipy/core/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/job/__init__.py` & `taipy-core-3.0.0.dev0/src/taipy/core/job/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/job/_job_fs_repository.py` & `taipy-core-3.0.0.dev0/src/taipy/core/job/_job_fs_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/job/_job_manager.py` & `taipy-core-3.0.0.dev0/src/taipy/core/job/_job_manager.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/job/_job_manager_factory.py` & `taipy-core-3.0.0.dev0/src/taipy/core/job/_job_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/job/_job_model.py` & `taipy-core-3.0.0.dev0/src/taipy/core/job/_job_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/job/_job_repository.py` & `taipy-core-3.0.0.dev0/src/taipy/core/job/_job_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/job/_job_repository_factory.py` & `taipy-core-3.0.0.dev0/src/taipy/core/job/_job_repository_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/job/_job_sql_repository.py` & `taipy-core-3.0.0.dev0/src/taipy/core/job/_job_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/job/job.py` & `taipy-core-3.0.0.dev0/src/taipy/core/job/job.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/job/job_id.py` & `taipy-core-3.0.0.dev0/src/taipy/core/job/job_id.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/job/status.py` & `taipy-core-3.0.0.dev0/src/taipy/core/job/status.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/notification/__init__.py` & `taipy-core-3.0.0.dev0/src/taipy/core/notification/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/notification/core_event_consumer.py` & `taipy-core-3.0.0.dev0/src/taipy/core/notification/core_event_consumer.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/notification/event.py` & `taipy-core-3.0.0.dev0/src/taipy/core/notification/event.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/notification/notifier.py` & `taipy-core-3.0.0.dev0/src/taipy/core/notification/notifier.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/notification/registration.py` & `taipy-core-3.0.0.dev0/src/taipy/core/notification/registration.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/notification/registration_id.py` & `taipy-core-3.0.0.dev0/src/taipy/core/notification/registration_id.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/notification/topic.py` & `taipy-core-3.0.0.dev0/src/taipy/core/notification/topic.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/pipeline/__init__.py` & `taipy-core-3.0.0.dev0/src/taipy/core/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/pipeline/_pipeline_fs_repository.py` & `taipy-core-3.0.0.dev0/src/taipy/core/pipeline/_pipeline_fs_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/pipeline/_pipeline_manager.py` & `taipy-core-3.0.0.dev0/src/taipy/core/pipeline/_pipeline_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 # an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
 
 from functools import partial
 from typing import Any, Callable, List, Optional, Union
 
-from taipy import Config
+from taipy.config import Config
 from taipy.config.common.scope import Scope
 
 from .._entity._entity_ids import _EntityIds
 from .._manager._manager import _Manager
 from .._version._version_manager_factory import _VersionManagerFactory
 from ..common.warn_if_inputs_not_ready import _warn_if_inputs_not_ready
 from ..config.pipeline_config import PipelineConfig
@@ -125,14 +125,20 @@
     @classmethod
     def __save_tasks(cls, tasks):
         task_manager = _TaskManagerFactory._build_manager()
         for i in tasks:
             task_manager._set(i)
 
     @classmethod
+    def _is_submittable(cls, pipeline: Union[Pipeline, PipelineId]) -> bool:
+        if isinstance(pipeline, str):
+            pipeline = cls._get(pipeline)
+        return isinstance(pipeline, Pipeline)
+
+    @classmethod
     def _submit(
         cls,
         pipeline: Union[PipelineId, Pipeline],
         callbacks: Optional[List[Callable]] = None,
         force: bool = False,
         wait: bool = False,
         timeout: Optional[Union[float, int]] = None,
```

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/pipeline/_pipeline_manager_factory.py` & `taipy-core-3.0.0.dev0/src/taipy/core/pipeline/_pipeline_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/pipeline/_pipeline_model.py` & `taipy-core-3.0.0.dev0/src/taipy/core/pipeline/_pipeline_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/pipeline/_pipeline_repository.py` & `taipy-core-3.0.0.dev0/src/taipy/core/pipeline/_pipeline_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/pipeline/_pipeline_repository_factory.py` & `taipy-core-3.0.0.dev0/src/taipy/core/pipeline/_pipeline_repository_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/pipeline/_pipeline_sql_repository.py` & `taipy-core-3.0.0.dev0/src/taipy/core/pipeline/_pipeline_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/pipeline/pipeline.py` & `taipy-core-3.0.0.dev0/src/taipy/core/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/pipeline/pipeline_id.py` & `taipy-core-3.0.0.dev0/src/taipy/core/pipeline/pipeline_id.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/scenario/__init__.py` & `taipy-core-3.0.0.dev0/src/taipy/core/scenario/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/scenario/_scenario_fs_repository.py` & `taipy-core-3.0.0.dev0/src/taipy/core/scenario/_scenario_fs_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/scenario/_scenario_manager.py` & `taipy-core-3.0.0.dev0/src/taipy/core/scenario/_scenario_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,14 +136,20 @@
     @classmethod
     def __save_pipelines(cls, pipelines):
         pipeline_manager = _PipelineManagerFactory._build_manager()
         for i in pipelines:
             pipeline_manager._set(i)
 
     @classmethod
+    def _is_submittable(cls, scenario: Union[Scenario, ScenarioId]) -> bool:
+        if isinstance(scenario, str):
+            scenario = cls._get(scenario)
+        return isinstance(scenario, Scenario)
+
+    @classmethod
     def _submit(
         cls,
         scenario: Union[Scenario, ScenarioId],
         callbacks: Optional[List[Callable]] = None,
         force: bool = False,
         wait: bool = False,
         timeout: Optional[Union[float, int]] = None,
@@ -203,14 +209,22 @@
         primary_scenarios = []
         for scenario in cls._get_all():
             if scenario.is_primary:
                 primary_scenarios.append(scenario)
         return primary_scenarios
 
     @classmethod
+    def _is_promotable_to_primary(cls, scenario: Union[Scenario, ScenarioId]) -> bool:
+        if isinstance(scenario, str):
+            scenario = cls._get(scenario)
+        if scenario and not scenario.is_primary and scenario.cycle:
+            return True
+        return False
+
+    @classmethod
     def _set_primary(cls, scenario: Scenario):
         if scenario.cycle:
             primary_scenario = cls._get_primary(scenario.cycle)
             if primary_scenario:
                 primary_scenario.is_primary = False  # type: ignore
             scenario.is_primary = True  # type: ignore
         else:
```

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/scenario/_scenario_manager_factory.py` & `taipy-core-3.0.0.dev0/src/taipy/core/scenario/_scenario_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/scenario/_scenario_model.py` & `taipy-core-3.0.0.dev0/src/taipy/core/scenario/_scenario_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/scenario/_scenario_repository.py` & `taipy-core-3.0.0.dev0/src/taipy/core/scenario/_scenario_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/scenario/_scenario_repository_factory.py` & `taipy-core-3.0.0.dev0/src/taipy/core/scenario/_scenario_repository_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/scenario/_scenario_sql_repository.py` & `taipy-core-3.0.0.dev0/src/taipy/core/scenario/_scenario_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/scenario/scenario.py` & `taipy-core-3.0.0.dev0/src/taipy/core/scenario/scenario.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/scenario/scenario_id.py` & `taipy-core-3.0.0.dev0/src/taipy/core/scenario/scenario_id.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/taipy.py` & `taipy-core-3.0.0.dev0/src/taipy/core/taipy.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,29 @@
         return _PipelineManagerFactory._build_manager()._set(entity)
     if isinstance(entity, Task):
         return _TaskManagerFactory._build_manager()._set(entity)
     if isinstance(entity, DataNode):
         return _DataManagerFactory._build_manager()._set(entity)
 
 
+def is_submittable(entity: Union[Scenario, ScenarioId, Pipeline, PipelineId, Task, TaskId]) -> bool:
+    """Indicate if an entity can be submitted.
+
+    Returns:
+        True if the given entity can be submitted. False otherwise.
+    """
+    if isinstance(entity, Scenario) or (isinstance(entity, str) and entity.startswith(Scenario._ID_PREFIX)):
+        return _ScenarioManagerFactory._build_manager()._is_submittable(entity)  # type: ignore
+    if isinstance(entity, Pipeline) or (isinstance(entity, str) and entity.startswith(Pipeline._ID_PREFIX)):
+        return _PipelineManagerFactory._build_manager()._is_submittable(entity)  # type: ignore
+    if isinstance(entity, Task) or (isinstance(entity, str) and entity.startswith(Task._ID_PREFIX)):
+        return _TaskManagerFactory._build_manager()._is_submittable(entity)  # type: ignore
+    return False
+
+
 @_warn_no_core_service()
 def submit(
     entity: Union[Scenario, Pipeline, Task],
     force: bool = False,
     wait: bool = False,
     timeout: Optional[Union[float, int]] = None,
 ) -> Union[Job, List[Job]]:
@@ -257,14 +272,23 @@
 
     Returns:
         The list of all primary scenarios.
     """
     return _ScenarioManagerFactory._build_manager()._get_primary_scenarios()
 
 
+def is_promotable(scenario: Union[Scenario, ScenarioId]) -> bool:
+    """Indicate if a scenario can be promoted to a primary scenario.
+
+    Returns:
+        True if the given scenario can be promoted to be a primary scenario. False otherwise.
+    """
+    return _ScenarioManagerFactory._build_manager()._is_promotable_to_primary(scenario)
+
+
 def set_primary(scenario: Scenario):
     """Promote a scenario as the primary scenario of its cycle.
 
     If the cycle of _scenario_ already has a primary scenario, it is demoted and
     is no longer the primary scenario for its cycle.
 
     Parameters:
@@ -658,15 +682,15 @@
             cycles_scenarios[scenario.cycle] = [scenario]
     return cycles_scenarios
 
 
 def get_entities_by_config_id(
     config_id: str,
 ) -> Union[List, List[Task], List[DataNode], List[Pipeline], List[Scenario]]:
-    """Get the entities by its cofig id.
+    """Get the entities by its config id.
 
     Parameters:
         config_id (str): The config id of the entities
     Returns:
         The list of all entities by the config id.
     """
```

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/task/__init__.py` & `taipy-core-3.0.0.dev0/src/taipy/core/task/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/task/_task_fs_repository.py` & `taipy-core-3.0.0.dev0/src/taipy/core/task/_task_fs_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/task/_task_manager.py` & `taipy-core-3.0.0.dev0/src/taipy/core/task/_task_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -137,14 +137,20 @@
         jobs = _JobManagerFactory._build_manager()._get_all()
         for job in jobs:
             if job.task.id == task.id:
                 entity_ids.job_ids.add(job.id)
         return entity_ids
 
     @classmethod
+    def _is_submittable(cls, task: Union[Task, TaskId]) -> bool:
+        if isinstance(task, str):
+            task = cls._get(task)
+        return isinstance(task, Task)
+
+    @classmethod
     def _submit(
         cls,
         task: Union[TaskId, Task],
         callbacks: Optional[List[Callable]] = None,
         force: bool = False,
         wait: bool = False,
         timeout: Optional[Union[float, int]] = None,
```

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/task/_task_manager_factory.py` & `taipy-core-3.0.0.dev0/src/taipy/core/task/_task_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/task/_task_model.py` & `taipy-core-3.0.0.dev0/src/taipy/core/task/_task_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/task/_task_repository.py` & `taipy-core-3.0.0.dev0/src/taipy/core/task/_task_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/task/_task_repository_factory.py` & `taipy-core-3.0.0.dev0/src/taipy/core/task/_task_repository_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/task/_task_sql_repository.py` & `taipy-core-3.0.0.dev0/src/taipy/core/task/_task_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/task/task.py` & `taipy-core-3.0.0.dev0/src/taipy/core/task/task.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy/core/task/task_id.py` & `taipy-core-3.0.0.dev0/src/taipy/core/task/task_id.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/src/taipy_core.egg-info/PKG-INFO` & `taipy-core-3.0.0.dev0/src/taipy_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipy-core
-Version: 2.3.0.dev6
+Version: 3.0.0.dev0
 Summary: A Python library to build powerful and customized data-driven back-end applications.
 Home-page: https://github.com/avaiga/taipy-core
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy-core
 Classifier: Intended Audience :: Developers
```

### Comparing `taipy-core-2.3.0.dev6/src/taipy_core.egg-info/SOURCES.txt` & `taipy-core-3.0.0.dev0/src/taipy_core.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 README.md
 pyproject.toml
 setup.py
 src/taipy/__init__.py
 src/taipy/core/__init__.py
 src/taipy/core/_core.py
 src/taipy/core/_core_cli.py
+src/taipy/core/_init.py
 src/taipy/core/taipy.py
 src/taipy/core/version.json
 src/taipy/core/_backup/__init__.py
 src/taipy/core/_backup/_backup.py
 src/taipy/core/_entity/__init__.py
 src/taipy/core/_entity/_dag.py
 src/taipy/core/_entity/_entity.py
```

### Comparing `taipy-core-2.3.0.dev6/tests/test_complex_application.py` & `taipy-core-3.0.0.dev0/tests/test_complex_application.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev6/tests/test_taipy.py` & `taipy-core-3.0.0.dev0/tests/test_taipy.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,22 +14,23 @@
 import pathlib
 import shutil
 from unittest import mock
 
 import pytest
 
 import src.taipy.core.taipy as tp
-from src.taipy.core import Core, CycleId, JobId, PipelineId, Scenario, ScenarioId, TaskId
+from src.taipy.core import Core, Cycle, CycleId, JobId, Pipeline, PipelineId, Scenario, ScenarioId, Task, TaskId
 from src.taipy.core._orchestrator._orchestrator_factory import _OrchestratorFactory
 from src.taipy.core._version._version_manager import _VersionManager
 from src.taipy.core.config.job_config import JobConfig
 from src.taipy.core.config.pipeline_config import PipelineConfig
 from src.taipy.core.config.scenario_config import ScenarioConfig
 from src.taipy.core.cycle._cycle_manager import _CycleManager
 from src.taipy.core.data._data_manager import _DataManager
+from src.taipy.core.data.pickle import PickleDataNode
 from src.taipy.core.exceptions.exceptions import InvalidExportPath
 from src.taipy.core.job._job_manager import _JobManager
 from src.taipy.core.job.job import Job
 from src.taipy.core.pipeline._pipeline_manager import _PipelineManager
 from src.taipy.core.scenario._scenario_manager import _ScenarioManager
 from src.taipy.core.task._task_manager import _TaskManager
 from taipy.config.common.frequency import Frequency
@@ -52,14 +53,69 @@
         with mock.patch("src.taipy.core.scenario._scenario_manager._ScenarioManager._set") as mck:
             tp.set(scenario)
             mck.assert_called_once_with(scenario)
         with mock.patch("src.taipy.core.cycle._cycle_manager._CycleManager._set") as mck:
             tp.set(cycle)
             mck.assert_called_once_with(cycle)
 
+    def test_is_submittable_is_called(self):
+        with mock.patch("src.taipy.core.scenario._scenario_manager._ScenarioManager._is_submittable") as mck:
+            scenario_id = ScenarioId("SCENARIO_id")
+            tp.is_submittable(scenario_id)
+            mck.assert_called_once_with(scenario_id)
+
+        with mock.patch("src.taipy.core.scenario._scenario_manager._ScenarioManager._is_submittable") as mck:
+            scenario = Scenario("scenario_config_id", [], {})
+            tp.is_submittable(scenario)
+            mck.assert_called_once_with(scenario)
+
+        with mock.patch("src.taipy.core.pipeline._pipeline_manager._PipelineManager._is_submittable") as mck:
+            pipeline_id = PipelineId("PIPELINE_id")
+            tp.is_submittable(pipeline_id)
+            mck.assert_called_once_with(pipeline_id)
+
+        with mock.patch("src.taipy.core.pipeline._pipeline_manager._PipelineManager._is_submittable") as mck:
+            pipeline = Pipeline("pipeline_config_id", {}, [])
+            tp.is_submittable(pipeline)
+            mck.assert_called_once_with(pipeline)
+
+        with mock.patch("src.taipy.core.task._task_manager._TaskManager._is_submittable") as mck:
+            task_id = TaskId("TASK_id")
+            tp.is_submittable(task_id)
+            mck.assert_called_once_with(task_id)
+
+        with mock.patch("src.taipy.core.task._task_manager._TaskManager._is_submittable") as mck:
+            task = Task("task_config_id", {}, print)
+            tp.is_submittable(task)
+            mck.assert_called_once_with(task)
+
+    def test_is_submittable(self):
+        current_date = datetime.datetime.now()
+
+        cycle = Cycle(Frequency.DAILY, {}, current_date, current_date, current_date)
+        scenario = Scenario("scenario_config_id", [], {})
+        pipeline = Pipeline("pipeline_config_id", {}, [])
+        task = Task("task_config_id", {}, print)
+        job = Job("job_id", task, "submit_id")
+        dn = PickleDataNode("data_node_config_id", Scope.SCENARIO)
+
+        _CycleManager._set(cycle)
+        _ScenarioManager._set(scenario)
+        _PipelineManager._set(pipeline)
+        _TaskManager._set(task)
+        _JobManager._set(job)
+        _DataManager._set(dn)
+
+        assert tp.is_submittable(scenario)
+        assert tp.is_submittable(pipeline)
+        assert tp.is_submittable(task)
+        assert not tp.is_submittable(cycle)
+        assert not tp.is_submittable(job)
+        assert not tp.is_submittable(dn)
+
     def test_submit(self, scenario, pipeline, task):
         with mock.patch("src.taipy.core.scenario._scenario_manager._ScenarioManager._submit") as mck:
             tp.submit(scenario)
             mck.assert_called_once_with(scenario, force=False, wait=False, timeout=None)
         with mock.patch("src.taipy.core.pipeline._pipeline_manager._PipelineManager._submit") as mck:
             tp.submit(pipeline)
             mck.assert_called_once_with(pipeline, force=False, wait=False, timeout=None)
@@ -113,14 +169,25 @@
             mck.assert_called_once_with(scenario_id)
 
         with mock.patch("src.taipy.core.scenario._scenario_manager._ScenarioManager._is_deletable") as mck:
             scenario = Scenario("config_id", [], {})
             tp.is_deletable(scenario)
             mck.assert_called_once_with(scenario)
 
+    def test_is_promotable(self):
+        with mock.patch("src.taipy.core.scenario._scenario_manager._ScenarioManager._is_promotable_to_primary") as mck:
+            scenario_id = ScenarioId("SCENARIO_id")
+            tp.is_promotable(scenario_id)
+            mck.assert_called_once_with(scenario_id)
+
+        with mock.patch("src.taipy.core.scenario._scenario_manager._ScenarioManager._is_promotable_to_primary") as mck:
+            scenario = Scenario("config_id", [], {})
+            tp.is_promotable(scenario)
+            mck.assert_called_once_with(scenario)
+
     def test_delete_scenario(self):
         with mock.patch("src.taipy.core.scenario._scenario_manager._ScenarioManager._hard_delete") as mck:
             scenario_id = ScenarioId("SCENARIO_id")
             tp.delete(scenario_id)
             mck.assert_called_once_with(scenario_id)
 
     def test_delete(self):
```

