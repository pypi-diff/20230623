# Comparing `tmp/apptools-5.2.0.tar.gz` & `tmp/apptools-5.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apptools-5.2.0.tar", last modified: Tue Aug 16 07:42:30 2022, max compression
+gzip compressed data, was "apptools-5.2.1.tar", last modified: Fri Jun 23 08:28:33 2023, max compression
```

## Comparing `apptools-5.2.0.tar` & `apptools-5.2.1.tar`

### file list

```diff
@@ -1,265 +1,265 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 07:42:30.505210 apptools-5.2.0/
--rw-r--r--   0 runner    (1001) docker     (121)     5991 2022-08-16 07:42:16.000000 apptools-5.2.0/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1616 2022-08-16 07:42:16.000000 apptools-5.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      418 2022-08-16 07:42:16.000000 apptools-5.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3733 2022-08-16 07:42:30.505210 apptools-5.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2520 2022-08-16 07:42:16.000000 apptools-5.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 07:42:30.461209 apptools-5.2.0/apptools/
--rw-r--r--   0 runner    (1001) docker     (121)      618 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 07:42:30.461209 apptools-5.2.0/apptools/_testing/
--rw-r--r--   0 runner    (1001) docker     (121)      454 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/_testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1348 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/_testing/optional_dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 07:42:30.461209 apptools-5.2.0/apptools/io/
--rw-r--r--   0 runner    (1001) docker     (121)      574 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      495 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/io/api.py
--rw-r--r--   0 runner    (1001) docker     (121)     9280 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/io/file.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 07:42:30.461209 apptools-5.2.0/apptools/io/h5/
--rw-r--r--   0 runner    (1001) docker     (121)      407 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/io/h5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7840 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/io/h5/dict_node.py
--rw-r--r--   0 runner    (1001) docker     (121)    16588 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/io/h5/file.py
--rw-r--r--   0 runner    (1001) docker     (121)     5330 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/io/h5/table_node.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 07:42:30.465209 apptools-5.2.0/apptools/io/h5/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      407 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/io/h5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7380 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/io/h5/tests/test_dict_node.py
--rw-r--r--   0 runner    (1001) docker     (121)    21487 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/io/h5/tests/test_file.py
--rw-r--r--   0 runner    (1001) docker     (121)     2782 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/io/h5/tests/test_table_node.py
--rw-r--r--   0 runner    (1001) docker     (121)      926 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/io/h5/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/io/h5/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 07:42:30.465209 apptools-5.2.0/apptools/io/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      407 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/io/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5796 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/io/tests/test_file.py
--rw-r--r--   0 runner    (1001) docker     (121)     7078 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/io/tests/test_folder.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 07:42:30.465209 apptools-5.2.0/apptools/logger/
--rw-r--r--   0 runner    (1001) docker     (121)      507 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/logger/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 07:42:30.469209 apptools-5.2.0/apptools/logger/agent/
--rw-r--r--   0 runner    (1001) docker     (121)      441 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/logger/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3242 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/logger/agent/attachments.py
--rw-r--r--   0 runner    (1001) docker     (121)     3432 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/logger/agent/quality_agent_mailer.py
--rw-r--r--   0 runner    (1001) docker     (121)    12131 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/logger/agent/quality_agent_view.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 07:42:30.469209 apptools-5.2.0/apptools/logger/agent/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      407 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/logger/agent/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2166 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/logger/agent/tests/test_attachments.py
--rw-r--r--   0 runner    (1001) docker     (121)      710 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/logger/api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1076 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/logger/custom_excepthook.py
--rw-r--r--   0 runner    (1001) docker     (121)     1319 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/logger/log_point.py
--rw-r--r--   0 runner    (1001) docker     (121)     1968 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/logger/log_queue_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)     1766 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/logger/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 07:42:30.469209 apptools-5.2.0/apptools/logger/plugin/
--rw-r--r--   0 runner    (1001) docker     (121)      407 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/logger/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3485 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/logger/plugin/logger_plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)     1226 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/logger/plugin/logger_preferences.py
--rw-r--r--   0 runner    (1001) docker     (121)     5564 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/logger/plugin/logger_service.py
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/logger/plugin/preferences.ini
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 07:42:30.469209 apptools-5.2.0/apptools/logger/plugin/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      407 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/logger/plugin/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1958 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/logger/plugin/tests/test_logger_service.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 07:42:30.469209 apptools-5.2.0/apptools/logger/plugin/view/
--rw-r--r--   0 runner    (1001) docker     (121)      407 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/logger/plugin/view/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 07:42:30.469209 apptools-5.2.0/apptools/logger/plugin/view/images/
--rw-r--r--   0 runner    (1001) docker     (121)      887 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/logger/plugin/view/images/crit_error.png
--rw-r--r--   0 runner    (1001) docker     (121)     3692 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/logger/plugin/view/images/debug.png
--rw-r--r--   0 runner    (1001) docker     (121)     3597 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/logger/plugin/view/images/error.png
--rw-r--r--   0 runner    (1001) docker     (121)     3632 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/logger/plugin/view/images/info.png
--rw-r--r--   0 runner    (1001) docker     (121)     3575 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/logger/plugin/view/images/warning.png
--rw-r--r--   0 runner    (1001) docker     (121)     3125 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/logger/plugin/view/logger_preferences_page.py
--rw-r--r--   0 runner    (1001) docker     (121)     6590 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/logger/plugin/view/logger_view.py
--rw-r--r--   0 runner    (1001) docker     (121)     1437 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/logger/ring_buffer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 07:42:30.477209 apptools-5.2.0/apptools/naming/
--rw-r--r--   0 runner    (1001) docker     (121)     1705 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/naming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      813 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/naming/address.py
--rw-r--r--   0 runner    (1001) docker     (121)     2443 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/naming/api.py
--rw-r--r--   0 runner    (1001) docker     (121)     3196 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/naming/binding.py
--rw-r--r--   0 runner    (1001) docker     (121)    22322 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/naming/context.py
--rw-r--r--   0 runner    (1001) docker     (121)     5650 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/naming/dir_context.py
--rw-r--r--   0 runner    (1001) docker     (121)     6604 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/naming/dynamic_context.py
--rw-r--r--   0 runner    (1001) docker     (121)     1487 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/naming/exception.py
--rw-r--r--   0 runner    (1001) docker     (121)     1875 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/naming/initial_context.py
--rw-r--r--   0 runner    (1001) docker     (121)     1054 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/naming/initial_context_factory.py
--rw-r--r--   0 runner    (1001) docker     (121)      817 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/naming/naming_event.py
--rw-r--r--   0 runner    (1001) docker     (121)     2743 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/naming/naming_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     1245 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/naming/object_factory.py
--rw-r--r--   0 runner    (1001) docker     (121)     2568 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/naming/object_serializer.py
--rw-r--r--   0 runner    (1001) docker     (121)     5756 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/naming/py_context.py
--rw-r--r--   0 runner    (1001) docker     (121)     1501 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/naming/py_object_factory.py
--rw-r--r--   0 runner    (1001) docker     (121)    18188 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/naming/pyfs_context.py
--rw-r--r--   0 runner    (1001) docker     (121)     1287 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/naming/pyfs_context_factory.py
--rw-r--r--   0 runner    (1001) docker     (121)     1798 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/naming/pyfs_initial_context_factory.py
--rw-r--r--   0 runner    (1001) docker     (121)     1256 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/naming/pyfs_object_factory.py
--rw-r--r--   0 runner    (1001) docker     (121)     1502 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/naming/pyfs_state_factory.py
--rw-r--r--   0 runner    (1001) docker     (121)     1594 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/naming/reference.py
--rw-r--r--   0 runner    (1001) docker     (121)      923 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/naming/referenceable.py
--rw-r--r--   0 runner    (1001) docker     (121)     1178 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/naming/referenceable_state_factory.py
--rw-r--r--   0 runner    (1001) docker     (121)     1237 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/naming/state_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 07:42:30.477209 apptools-5.2.0/apptools/naming/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      407 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/naming/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16389 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/naming/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (121)     3940 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/naming/tests/test_dir_context.py
--rw-r--r--   0 runner    (1001) docker     (121)     1647 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/naming/tests/test_object_serializer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1000 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/naming/tests/test_py_context.py
--rw-r--r--   0 runner    (1001) docker     (121)    11650 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/naming/tests/test_pyfs_context.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 07:42:30.477209 apptools-5.2.0/apptools/naming/trait_defs/
--rw-r--r--   0 runner    (1001) docker     (121)      625 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/naming/trait_defs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      537 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/naming/trait_defs/api.py
--rw-r--r--   0 runner    (1001) docker     (121)     6021 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/naming/trait_defs/naming_traits.py
--rw-r--r--   0 runner    (1001) docker     (121)      983 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/naming/unique_name.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 07:42:30.481209 apptools-5.2.0/apptools/persistence/
--rw-r--r--   0 runner    (1001) docker     (121)      568 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/persistence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2940 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/persistence/file_path.py
--rw-r--r--   0 runner    (1001) docker     (121)     4034 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/persistence/project_loader.py
--rw-r--r--   0 runner    (1001) docker     (121)    34769 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/persistence/state_pickler.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 07:42:30.481209 apptools-5.2.0/apptools/persistence/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      407 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/persistence/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1637 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/persistence/tests/state_function_classes.py
--rw-r--r--   0 runner    (1001) docker     (121)     2653 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/persistence/tests/test_class_mapping.py
--rw-r--r--   0 runner    (1001) docker     (121)     4390 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/persistence/tests/test_file_path.py
--rw-r--r--   0 runner    (1001) docker     (121)     4886 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/persistence/tests/test_state_function.py
--rw-r--r--   0 runner    (1001) docker     (121)    16014 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/persistence/tests/test_state_pickler.py
--rw-r--r--   0 runner    (1001) docker     (121)     4444 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/persistence/tests/test_two_stage_unpickler.py
--rw-r--r--   0 runner    (1001) docker     (121)     4128 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/persistence/tests/test_version_registry.py
--rw-r--r--   0 runner    (1001) docker     (121)     1534 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/persistence/updater.py
--rw-r--r--   0 runner    (1001) docker     (121)     3763 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/persistence/version_registry.py
--rw-r--r--   0 runner    (1001) docker     (121)     7883 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/persistence/versioned_unpickler.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 07:42:30.485209 apptools-5.2.0/apptools/preferences/
--rw-r--r--   0 runner    (1001) docker     (121)      509 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/preferences/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/preferences/api.py
--rw-r--r--   0 runner    (1001) docker     (121)     4988 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/preferences/i_preferences.py
--rw-r--r--   0 runner    (1001) docker     (121)     1092 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/preferences/package_globals.py
--rw-r--r--   0 runner    (1001) docker     (121)     6086 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/preferences/preference_binding.py
--rw-r--r--   0 runner    (1001) docker     (121)    17433 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/preferences/preferences.py
--rw-r--r--   0 runner    (1001) docker     (121)     7278 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/preferences/preferences_helper.py
--rw-r--r--   0 runner    (1001) docker     (121)    14541 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/preferences/scoped_preferences.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 07:42:30.485209 apptools-5.2.0/apptools/preferences/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      407 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/preferences/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      228 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/preferences/tests/example.ini
--rw-r--r--   0 runner    (1001) docker     (121)      767 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/preferences/tests/py_config_example.ini
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/preferences/tests/py_config_example_2.ini
--rw-r--r--   0 runner    (1001) docker     (121)     8249 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/preferences/tests/py_config_file.py
--rw-r--r--   0 runner    (1001) docker     (121)    11596 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/preferences/tests/test_preference_binding.py
--rw-r--r--   0 runner    (1001) docker     (121)    18879 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/preferences/tests/test_preferences.py
--rw-r--r--   0 runner    (1001) docker     (121)    20990 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/preferences/tests/test_preferences_helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     7192 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/preferences/tests/test_py_config_file.py
--rw-r--r--   0 runner    (1001) docker     (121)    13482 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/preferences/tests/test_scoped_preferences.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 07:42:30.489209 apptools-5.2.0/apptools/preferences/ui/
--rw-r--r--   0 runner    (1001) docker     (121)      407 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/preferences/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      705 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/preferences/ui/api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1096 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/preferences/ui/i_preferences_page.py
--rw-r--r--   0 runner    (1001) docker     (121)     9301 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/preferences/ui/preferences_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     2776 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/preferences/ui/preferences_node.py
--rw-r--r--   0 runner    (1001) docker     (121)     3857 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/preferences/ui/preferences_page.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 07:42:30.489209 apptools-5.2.0/apptools/preferences/ui/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      407 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/preferences/ui/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3774 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/preferences/ui/tests/test_preferences_page.py
--rw-r--r--   0 runner    (1001) docker     (121)     3843 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/preferences/ui/tree_item.py
--rw-r--r--   0 runner    (1001) docker     (121)     3114 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/preferences/ui/widget_editor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 07:42:30.489209 apptools-5.2.0/apptools/scripting/
--rw-r--r--   0 runner    (1001) docker     (121)      515 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/scripting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      956 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/scripting/api.py
--rw-r--r--   0 runner    (1001) docker     (121)      756 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/scripting/package_globals.py
--rw-r--r--   0 runner    (1001) docker     (121)     1802 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/scripting/recordable.py
--rw-r--r--   0 runner    (1001) docker     (121)    26775 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/scripting/recorder.py
--rw-r--r--   0 runner    (1001) docker     (121)     3208 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/scripting/recorder_with_ui.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 07:42:30.489209 apptools-5.2.0/apptools/scripting/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      407 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/scripting/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14568 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/scripting/tests/test_recorder.py
--rw-r--r--   0 runner    (1001) docker     (121)     1732 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/scripting/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 07:42:30.493209 apptools-5.2.0/apptools/selection/
--rw-r--r--   0 runner    (1001) docker     (121)      407 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/selection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/selection/api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1478 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/selection/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)      903 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/selection/i_selection.py
--rw-r--r--   0 runner    (1001) docker     (121)     1662 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/selection/i_selection_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)     2280 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/selection/list_selection.py
--rw-r--r--   0 runner    (1001) docker     (121)     7276 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/selection/selection_service.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 07:42:30.493209 apptools-5.2.0/apptools/selection/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      407 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/selection/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2249 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/selection/tests/test_list_selection.py
--rw-r--r--   0 runner    (1001) docker     (121)     9960 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/selection/tests/test_selection_service.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 07:42:30.493209 apptools-5.2.0/apptools/type_registry/
--rw-r--r--   0 runner    (1001) docker     (121)      407 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/type_registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      571 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/type_registry/api.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 07:42:30.493209 apptools-5.2.0/apptools/type_registry/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      407 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/type_registry/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      813 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/type_registry/tests/dummies.py
--rw-r--r--   0 runner    (1001) docker     (121)     2506 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/type_registry/tests/test_lazy_registry.py
--rw-r--r--   0 runner    (1001) docker     (121)     5310 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/type_registry/tests/test_type_registry.py
--rw-r--r--   0 runner    (1001) docker     (121)     8705 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/type_registry/type_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 07:42:30.497209 apptools-5.2.0/apptools/undo/
--rw-r--r--   0 runner    (1001) docker     (121)      742 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/undo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      709 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/undo/abstract_command.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 07:42:30.497209 apptools-5.2.0/apptools/undo/action/
--rw-r--r--   0 runner    (1001) docker     (121)      620 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/undo/action/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      761 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/undo/action/abstract_command_stack_action.py
--rw-r--r--   0 runner    (1001) docker     (121)      881 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/undo/action/api.py
--rw-r--r--   0 runner    (1001) docker     (121)      714 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/undo/action/command_action.py
--rw-r--r--   0 runner    (1001) docker     (121)      711 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/undo/action/redo_action.py
--rw-r--r--   0 runner    (1001) docker     (121)      711 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/undo/action/undo_action.py
--rw-r--r--   0 runner    (1001) docker     (121)     1027 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/undo/api.py
--rw-r--r--   0 runner    (1001) docker     (121)      771 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/undo/command_stack.py
--rw-r--r--   0 runner    (1001) docker     (121)      702 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/undo/i_command.py
--rw-r--r--   0 runner    (1001) docker     (121)      707 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/undo/i_command_stack.py
--rw-r--r--   0 runner    (1001) docker     (121)      706 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/undo/i_undo_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)      705 2022-08-16 07:42:16.000000 apptools-5.2.0/apptools/undo/undo_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)      831 2022-08-16 07:42:30.000000 apptools-5.2.0/apptools/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 07:42:30.461209 apptools-5.2.0/apptools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3733 2022-08-16 07:42:30.000000 apptools-5.2.0/apptools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7642 2022-08-16 07:42:30.000000 apptools-5.2.0/apptools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-16 07:42:30.000000 apptools-5.2.0/apptools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-16 07:42:30.000000 apptools-5.2.0/apptools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      209 2022-08-16 07:42:30.000000 apptools-5.2.0/apptools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-08-16 07:42:30.000000 apptools-5.2.0/apptools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 07:42:30.497209 apptools-5.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     3134 2022-08-16 07:42:16.000000 apptools-5.2.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 07:42:30.497209 apptools-5.2.0/docs/releases/
--rw-r--r--   0 runner    (1001) docker     (121)     1038 2022-08-16 07:42:16.000000 apptools-5.2.0/docs/releases/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 07:42:30.497209 apptools-5.2.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 07:42:30.497209 apptools-5.2.0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (121)    13515 2022-08-16 07:42:16.000000 apptools-5.2.0/docs/source/_static/default.css
--rw-r--r--   0 runner    (1001) docker     (121)     3913 2022-08-16 07:42:16.000000 apptools-5.2.0/docs/source/_static/e-logo-rev.png
--rw-r--r--   0 runner    (1001) docker     (121)    10134 2022-08-16 07:42:16.000000 apptools-5.2.0/docs/source/_static/et.ico
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 07:42:30.457209 apptools-5.2.0/docs/source/api/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 07:42:30.501210 apptools-5.2.0/docs/source/api/templates/
--rw-r--r--   0 runner    (1001) docker     (121)      667 2022-08-16 07:42:16.000000 apptools-5.2.0/docs/source/api/templates/module.rst_t
--rw-r--r--   0 runner    (1001) docker     (121)      914 2022-08-16 07:42:16.000000 apptools-5.2.0/docs/source/api/templates/package.rst_t
--rw-r--r--   0 runner    (1001) docker     (121)     3775 2022-08-16 07:42:16.000000 apptools-5.2.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      276 2022-08-16 07:42:16.000000 apptools-5.2.0/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 07:42:30.501210 apptools-5.2.0/docs/source/io/
--rw-r--r--   0 runner    (1001) docker     (121)      784 2022-08-16 07:42:16.000000 apptools-5.2.0/docs/source/io/introduction.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 07:42:30.501210 apptools-5.2.0/docs/source/naming/
--rw-r--r--   0 runner    (1001) docker     (121)      366 2022-08-16 07:42:16.000000 apptools-5.2.0/docs/source/naming/Introduction.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 07:42:30.501210 apptools-5.2.0/docs/source/preferences/
--rw-r--r--   0 runner    (1001) docker     (121)    10398 2022-08-16 07:42:16.000000 apptools-5.2.0/docs/source/preferences/Preferences.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1798 2022-08-16 07:42:16.000000 apptools-5.2.0/docs/source/preferences/PreferencesInEnvisage.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 07:42:30.501210 apptools-5.2.0/docs/source/scripting/
--rw-r--r--   0 runner    (1001) docker     (121)     6619 2022-08-16 07:42:16.000000 apptools-5.2.0/docs/source/scripting/introduction.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 07:42:30.501210 apptools-5.2.0/docs/source/selection/
--rw-r--r--   0 runner    (1001) docker     (121)     6033 2022-08-16 07:42:16.000000 apptools-5.2.0/docs/source/selection/selection.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 07:42:30.501210 apptools-5.2.0/docs/source/undo/
--rw-r--r--   0 runner    (1001) docker     (121)    10329 2022-08-16 07:42:16.000000 apptools-5.2.0/docs/source/undo/Introduction.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 07:42:30.457209 apptools-5.2.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 07:42:30.501210 apptools-5.2.0/examples/naming/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 07:42:30.501210 apptools-5.2.0/examples/naming/images/
--rw-r--r--   0 runner    (1001) docker     (121)      533 2022-08-16 07:42:16.000000 apptools-5.2.0/examples/naming/images/closed_folder.png
--rw-r--r--   0 runner    (1001) docker     (121)      333 2022-08-16 07:42:16.000000 apptools-5.2.0/examples/naming/images/document.png
--rw-r--r--   0 runner    (1001) docker     (121)      441 2022-08-16 07:42:16.000000 apptools-5.2.0/examples/naming/images/image_LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      617 2022-08-16 07:42:16.000000 apptools-5.2.0/examples/naming/images/open_folder.png
--rw-r--r--   0 runner    (1001) docker     (121)     1036 2022-08-16 07:42:16.000000 apptools-5.2.0/examples/naming/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 07:42:30.501210 apptools-5.2.0/examples/preferences/
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-08-16 07:42:16.000000 apptools-5.2.0/examples/preferences/example.ini
--rw-r--r--   0 runner    (1001) docker     (121)     3199 2022-08-16 07:42:16.000000 apptools-5.2.0/examples/preferences/preferences_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 07:42:30.505210 apptools-5.2.0/examples/undo/
--rw-r--r--   0 runner    (1001) docker     (121)     5957 2022-08-16 07:42:16.000000 apptools-5.2.0/examples/undo/commands.py
--rw-r--r--   0 runner    (1001) docker     (121)     2358 2022-08-16 07:42:16.000000 apptools-5.2.0/examples/undo/example.py
--rw-r--r--   0 runner    (1001) docker     (121)     4449 2022-08-16 07:42:16.000000 apptools-5.2.0/examples/undo/example_editor_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     5158 2022-08-16 07:42:16.000000 apptools-5.2.0/examples/undo/example_undo_window.py
--rw-r--r--   0 runner    (1001) docker     (121)     1455 2022-08-16 07:42:16.000000 apptools-5.2.0/examples/undo/model.py
--rw-r--r--   0 runner    (1001) docker     (121)      588 2022-08-16 07:42:16.000000 apptools-5.2.0/image_LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)    19917 2022-08-16 07:42:16.000000 apptools-5.2.0/image_LICENSE_CP.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 07:42:30.457209 apptools-5.2.0/integrationtests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 07:42:30.505210 apptools-5.2.0/integrationtests/persistence/
--rw-r--r--   0 runner    (1001) docker     (121)     2544 2022-08-16 07:42:16.000000 apptools-5.2.0/integrationtests/persistence/test_persistence.py
--rw-r--r--   0 runner    (1001) docker     (121)     1291 2022-08-16 07:42:16.000000 apptools-5.2.0/integrationtests/persistence/update1.py
--rw-r--r--   0 runner    (1001) docker     (121)      973 2022-08-16 07:42:16.000000 apptools-5.2.0/integrationtests/persistence/update2.py
--rw-r--r--   0 runner    (1001) docker     (121)      976 2022-08-16 07:42:16.000000 apptools-5.2.0/integrationtests/persistence/update3.py
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-08-16 07:42:16.000000 apptools-5.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      145 2022-08-16 07:42:30.505210 apptools-5.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)    10140 2022-08-16 07:42:16.000000 apptools-5.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:28:33.382400 apptools-5.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-06-23 08:28:15.000000 apptools-5.2.1/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-06-23 08:28:15.000000 apptools-5.2.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-23 08:28:15.000000 apptools-5.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-06-23 08:28:33.382400 apptools-5.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-06-23 08:28:15.000000 apptools-5.2.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:28:33.350399 apptools-5.2.1/apptools/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:28:33.350399 apptools-5.2.1/apptools/_testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/_testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/_testing/optional_dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:28:33.350399 apptools-5.2.1/apptools/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/io/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9280 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/io/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:28:33.350399 apptools-5.2.1/apptools/io/h5/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/io/h5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7840 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/io/h5/dict_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16588 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/io/h5/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/io/h5/table_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:28:33.350399 apptools-5.2.1/apptools/io/h5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/io/h5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7380 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/io/h5/tests/test_dict_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21487 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/io/h5/tests/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/io/h5/tests/test_table_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/io/h5/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/io/h5/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:28:33.354399 apptools-5.2.1/apptools/io/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/io/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/io/tests/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/io/tests/test_folder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:28:33.354399 apptools-5.2.1/apptools/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/logger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:28:33.354399 apptools-5.2.1/apptools/logger/agent/
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/logger/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/logger/agent/attachments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/logger/agent/quality_agent_mailer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12131 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/logger/agent/quality_agent_view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:28:33.354399 apptools-5.2.1/apptools/logger/agent/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/logger/agent/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/logger/agent/tests/test_attachments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/logger/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/logger/custom_excepthook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/logger/log_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/logger/log_queue_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/logger/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:28:33.354399 apptools-5.2.1/apptools/logger/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/logger/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/logger/plugin/logger_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/logger/plugin/logger_preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/logger/plugin/logger_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/logger/plugin/preferences.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:28:33.354399 apptools-5.2.1/apptools/logger/plugin/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/logger/plugin/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/logger/plugin/tests/test_logger_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:28:33.354399 apptools-5.2.1/apptools/logger/plugin/view/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/logger/plugin/view/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:28:33.358399 apptools-5.2.1/apptools/logger/plugin/view/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/logger/plugin/view/images/crit_error.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/logger/plugin/view/images/debug.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/logger/plugin/view/images/error.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/logger/plugin/view/images/info.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/logger/plugin/view/images/warning.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/logger/plugin/view/logger_preferences_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6590 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/logger/plugin/view/logger_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/logger/ring_buffer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:28:33.362399 apptools-5.2.1/apptools/naming/
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/naming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/naming/address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/naming/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/naming/binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22322 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/naming/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/naming/dir_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6604 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/naming/dynamic_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/naming/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/naming/initial_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/naming/initial_context_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/naming/naming_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/naming/naming_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/naming/object_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/naming/object_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/naming/py_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/naming/py_object_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18188 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/naming/pyfs_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/naming/pyfs_context_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/naming/pyfs_initial_context_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/naming/pyfs_object_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/naming/pyfs_state_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/naming/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/naming/referenceable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/naming/referenceable_state_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/naming/state_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:28:33.362399 apptools-5.2.1/apptools/naming/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/naming/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16389 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/naming/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/naming/tests/test_dir_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/naming/tests/test_object_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/naming/tests/test_py_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11650 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/naming/tests/test_pyfs_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:28:33.362399 apptools-5.2.1/apptools/naming/trait_defs/
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/naming/trait_defs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/naming/trait_defs/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/naming/trait_defs/naming_traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/naming/unique_name.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:28:33.366400 apptools-5.2.1/apptools/persistence/
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/persistence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/persistence/file_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/persistence/project_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34876 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/persistence/state_pickler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:28:33.366400 apptools-5.2.1/apptools/persistence/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/persistence/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/persistence/tests/state_function_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/persistence/tests/test_class_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/persistence/tests/test_file_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/persistence/tests/test_state_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16014 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/persistence/tests/test_state_pickler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/persistence/tests/test_two_stage_unpickler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/persistence/tests/test_version_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/persistence/updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/persistence/version_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/persistence/versioned_unpickler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:28:33.366400 apptools-5.2.1/apptools/preferences/
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/preferences/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/preferences/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/preferences/i_preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/preferences/package_globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6086 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/preferences/preference_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17433 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/preferences/preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/preferences/preferences_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14541 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/preferences/scoped_preferences.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:28:33.370400 apptools-5.2.1/apptools/preferences/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/preferences/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/preferences/tests/example.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/preferences/tests/py_config_example.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/preferences/tests/py_config_example_2.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/preferences/tests/py_config_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11596 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/preferences/tests/test_preference_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18879 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/preferences/tests/test_preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20990 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/preferences/tests/test_preferences_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7192 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/preferences/tests/test_py_config_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13482 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/preferences/tests/test_scoped_preferences.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:28:33.370400 apptools-5.2.1/apptools/preferences/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/preferences/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/preferences/ui/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/preferences/ui/i_preferences_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9301 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/preferences/ui/preferences_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/preferences/ui/preferences_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/preferences/ui/preferences_page.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:28:33.370400 apptools-5.2.1/apptools/preferences/ui/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/preferences/ui/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/preferences/ui/tests/test_preferences_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/preferences/ui/tree_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/preferences/ui/widget_editor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:28:33.370400 apptools-5.2.1/apptools/scripting/
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/scripting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/scripting/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/scripting/package_globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/scripting/recordable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26775 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/scripting/recorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/scripting/recorder_with_ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:28:33.374400 apptools-5.2.1/apptools/scripting/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/scripting/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14568 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/scripting/tests/test_recorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/scripting/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:28:33.374400 apptools-5.2.1/apptools/selection/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/selection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/selection/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/selection/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/selection/i_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/selection/i_selection_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/selection/list_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/selection/selection_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:28:33.374400 apptools-5.2.1/apptools/selection/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/selection/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/selection/tests/test_list_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9960 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/selection/tests/test_selection_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:28:33.374400 apptools-5.2.1/apptools/type_registry/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/type_registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/type_registry/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:28:33.374400 apptools-5.2.1/apptools/type_registry/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/type_registry/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/type_registry/tests/dummies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/type_registry/tests/test_lazy_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/type_registry/tests/test_type_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8705 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/type_registry/type_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:28:33.378400 apptools-5.2.1/apptools/undo/
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/undo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/undo/abstract_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:28:33.378400 apptools-5.2.1/apptools/undo/action/
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/undo/action/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/undo/action/abstract_command_stack_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/undo/action/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/undo/action/command_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/undo/action/redo_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/undo/action/undo_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/undo/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/undo/command_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/undo/i_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/undo/i_command_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/undo/i_undo_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-23 08:28:15.000000 apptools-5.2.1/apptools/undo/undo_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-23 08:28:33.000000 apptools-5.2.1/apptools/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:28:33.350399 apptools-5.2.1/apptools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-06-23 08:28:33.000000 apptools-5.2.1/apptools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-06-23 08:28:33.000000 apptools-5.2.1/apptools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 08:28:33.000000 apptools-5.2.1/apptools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 08:28:33.000000 apptools-5.2.1/apptools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-23 08:28:33.000000 apptools-5.2.1/apptools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-23 08:28:33.000000 apptools-5.2.1/apptools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:28:33.378400 apptools-5.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-06-23 08:28:15.000000 apptools-5.2.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:28:33.378400 apptools-5.2.1/docs/releases/
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-23 08:28:15.000000 apptools-5.2.1/docs/releases/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:28:33.378400 apptools-5.2.1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:28:33.378400 apptools-5.2.1/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    13515 2023-06-23 08:28:15.000000 apptools-5.2.1/docs/source/_static/default.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-06-23 08:28:15.000000 apptools-5.2.1/docs/source/_static/e-logo-rev.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10134 2023-06-23 08:28:15.000000 apptools-5.2.1/docs/source/_static/et.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:28:33.346399 apptools-5.2.1/docs/source/api/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:28:33.378400 apptools-5.2.1/docs/source/api/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-23 08:28:15.000000 apptools-5.2.1/docs/source/api/templates/module.rst_t
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-23 08:28:15.000000 apptools-5.2.1/docs/source/api/templates/package.rst_t
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-06-23 08:28:15.000000 apptools-5.2.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-23 08:28:15.000000 apptools-5.2.1/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:28:33.378400 apptools-5.2.1/docs/source/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-23 08:28:15.000000 apptools-5.2.1/docs/source/io/introduction.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:28:33.378400 apptools-5.2.1/docs/source/naming/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-23 08:28:15.000000 apptools-5.2.1/docs/source/naming/Introduction.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:28:33.378400 apptools-5.2.1/docs/source/preferences/
+-rw-r--r--   0 runner    (1001) docker     (123)    10398 2023-06-23 08:28:15.000000 apptools-5.2.1/docs/source/preferences/Preferences.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-23 08:28:15.000000 apptools-5.2.1/docs/source/preferences/PreferencesInEnvisage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:28:33.378400 apptools-5.2.1/docs/source/scripting/
+-rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-06-23 08:28:15.000000 apptools-5.2.1/docs/source/scripting/introduction.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:28:33.378400 apptools-5.2.1/docs/source/selection/
+-rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-06-23 08:28:15.000000 apptools-5.2.1/docs/source/selection/selection.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:28:33.378400 apptools-5.2.1/docs/source/undo/
+-rw-r--r--   0 runner    (1001) docker     (123)    10329 2023-06-23 08:28:15.000000 apptools-5.2.1/docs/source/undo/Introduction.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:28:33.346399 apptools-5.2.1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:28:33.382400 apptools-5.2.1/examples/naming/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:28:33.382400 apptools-5.2.1/examples/naming/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-23 08:28:15.000000 apptools-5.2.1/examples/naming/images/closed_folder.png
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-23 08:28:15.000000 apptools-5.2.1/examples/naming/images/document.png
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-23 08:28:15.000000 apptools-5.2.1/examples/naming/images/image_LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-23 08:28:15.000000 apptools-5.2.1/examples/naming/images/open_folder.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-06-23 08:28:15.000000 apptools-5.2.1/examples/naming/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:28:33.382400 apptools-5.2.1/examples/preferences/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-23 08:28:15.000000 apptools-5.2.1/examples/preferences/example.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-06-23 08:28:15.000000 apptools-5.2.1/examples/preferences/preferences_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:28:33.382400 apptools-5.2.1/examples/undo/
+-rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-06-23 08:28:15.000000 apptools-5.2.1/examples/undo/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-06-23 08:28:15.000000 apptools-5.2.1/examples/undo/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-06-23 08:28:15.000000 apptools-5.2.1/examples/undo/example_editor_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5158 2023-06-23 08:28:15.000000 apptools-5.2.1/examples/undo/example_undo_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-23 08:28:15.000000 apptools-5.2.1/examples/undo/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-23 08:28:15.000000 apptools-5.2.1/image_LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    19917 2023-06-23 08:28:15.000000 apptools-5.2.1/image_LICENSE_CP.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:28:33.346399 apptools-5.2.1/integrationtests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:28:33.382400 apptools-5.2.1/integrationtests/persistence/
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-06-23 08:28:15.000000 apptools-5.2.1/integrationtests/persistence/test_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-23 08:28:15.000000 apptools-5.2.1/integrationtests/persistence/update1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-23 08:28:15.000000 apptools-5.2.1/integrationtests/persistence/update2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-23 08:28:15.000000 apptools-5.2.1/integrationtests/persistence/update3.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-23 08:28:15.000000 apptools-5.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-23 08:28:33.382400 apptools-5.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    10140 2023-06-23 08:28:15.000000 apptools-5.2.1/setup.py
```

### Comparing `apptools-5.2.0/CHANGES.txt` & `apptools-5.2.1/CHANGES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,34 @@
 Apptools CHANGELOG
 ==================
 
+Released: 2023-05-25
+
+This is a bugfix release fixing a Python 3.11 compatibility issue in
+StatePickler.
+
+Thanks to the following contributors:
+
+* Mark Dickinson
+* Tony Ni
+* Rahul Poruri
+
+Version 5.2.0
+~~~~~~~~~~~~~
+
+Fixes
+-----
+* Fix StatePickler for Python 3.11. (#328)
+* Add encoding as an attribute for LogFileHandler initialization (#324)
+
+Build
+-----
+* Drop Python 3.6 and MacOS from EDM test matrix. (#332, #333)
+* Update Github workflows (#326)
+
 Version 5.2.0
 ~~~~~~~~~~~~~
 
 Released: 2022-08-16
 
 This is a minor release, focusing primarily on Python 3.8 support and updating
 of development workflows.
```

### Comparing `apptools-5.2.0/LICENSE.txt` & `apptools-5.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `apptools-5.2.0/PKG-INFO` & `apptools-5.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apptools
-Version: 5.2.0
+Version: 5.2.1
 Summary: application tools
 Home-page: https://docs.enthought.com/apptools
 Download-URL: https://www.github.com/enthought/apptools
 Author: Enthought, Inc.
 Author-email: info@enthought.com
 Maintainer: ETS Developers
 Maintainer-email: enthought-dev@enthought.com
```

### Comparing `apptools-5.2.0/README.rst` & `apptools-5.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `apptools-5.2.0/apptools/__init__.py` & `apptools-5.2.1/apptools/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/_testing/optional_dependencies.py` & `apptools-5.2.1/apptools/_testing/optional_dependencies.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2006-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2006-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/io/__init__.py` & `apptools-5.2.1/apptools/io/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/io/file.py` & `apptools-5.2.1/apptools/io/file.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/io/h5/dict_node.py` & `apptools-5.2.1/apptools/io/h5/dict_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/io/h5/file.py` & `apptools-5.2.1/apptools/io/h5/file.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/io/h5/table_node.py` & `apptools-5.2.1/apptools/io/h5/table_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/io/h5/tests/test_dict_node.py` & `apptools-5.2.1/apptools/io/h5/tests/test_dict_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/io/h5/tests/test_file.py` & `apptools-5.2.1/apptools/io/h5/tests/test_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/io/h5/tests/test_table_node.py` & `apptools-5.2.1/apptools/io/h5/tests/test_table_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/io/h5/tests/utils.py` & `apptools-5.2.1/apptools/io/h5/tests/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/io/h5/utils.py` & `apptools-5.2.1/apptools/io/h5/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/io/tests/test_file.py` & `apptools-5.2.1/apptools/io/tests/test_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/io/tests/test_folder.py` & `apptools-5.2.1/apptools/io/tests/test_folder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/logger/agent/attachments.py` & `apptools-5.2.1/apptools/logger/agent/attachments.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/logger/agent/quality_agent_mailer.py` & `apptools-5.2.1/apptools/logger/agent/quality_agent_mailer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/logger/agent/quality_agent_view.py` & `apptools-5.2.1/apptools/logger/agent/quality_agent_view.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/logger/agent/tests/test_attachments.py` & `apptools-5.2.1/apptools/logger/agent/tests/test_attachments.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/logger/api.py` & `apptools-5.2.1/apptools/logger/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/logger/custom_excepthook.py` & `apptools-5.2.1/apptools/logger/custom_excepthook.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/logger/log_point.py` & `apptools-5.2.1/apptools/logger/log_point.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/logger/log_queue_handler.py` & `apptools-5.2.1/apptools/logger/log_queue_handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/logger/logger.py` & `apptools-5.2.1/apptools/logger/logger.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
@@ -25,18 +25,32 @@
 FORMATTER = logging.Formatter("%(levelname)s|%(asctime)s|%(message)s")
 
 
 class LogFileHandler(RotatingFileHandler):
     """The default log file handler."""
 
     def __init__(
-        self, path, maxBytes=1000000, backupCount=3, level=None, formatter=None
+        self,
+        path,
+        mode="a",
+        maxBytes=1000000,
+        backupCount=3,
+        level=None,
+        formatter=None,
+        encoding=None,
+        delay=False,
     ):
         RotatingFileHandler.__init__(
-            self, path, maxBytes=maxBytes, backupCount=3
+            self,
+            filename=path,
+            mode=mode,
+            maxBytes=maxBytes,
+            backupCount=backupCount,
+            encoding=encoding,
+            delay=delay,
         )
 
         if level is None:
             level = LEVEL
         if formatter is None:
             formatter = FORMATTER
         # Set our default formatter and log level.
```

### Comparing `apptools-5.2.0/apptools/logger/plugin/logger_plugin.py` & `apptools-5.2.1/apptools/logger/plugin/logger_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/logger/plugin/logger_preferences.py` & `apptools-5.2.1/apptools/logger/plugin/logger_preferences.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/logger/plugin/logger_service.py` & `apptools-5.2.1/apptools/logger/plugin/logger_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/logger/plugin/tests/test_logger_service.py` & `apptools-5.2.1/apptools/logger/plugin/tests/test_logger_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/logger/plugin/view/images/crit_error.png` & `apptools-5.2.1/apptools/logger/plugin/view/images/crit_error.png`

 * *Files identical despite different names*

### Comparing `apptools-5.2.0/apptools/logger/plugin/view/images/debug.png` & `apptools-5.2.1/apptools/logger/plugin/view/images/debug.png`

 * *Files identical despite different names*

### Comparing `apptools-5.2.0/apptools/logger/plugin/view/images/error.png` & `apptools-5.2.1/apptools/logger/plugin/view/images/error.png`

 * *Files identical despite different names*

### Comparing `apptools-5.2.0/apptools/logger/plugin/view/images/info.png` & `apptools-5.2.1/apptools/logger/plugin/view/images/info.png`

 * *Files identical despite different names*

### Comparing `apptools-5.2.0/apptools/logger/plugin/view/images/warning.png` & `apptools-5.2.1/apptools/logger/plugin/view/images/warning.png`

 * *Files identical despite different names*

### Comparing `apptools-5.2.0/apptools/logger/plugin/view/logger_preferences_page.py` & `apptools-5.2.1/apptools/logger/plugin/view/logger_preferences_page.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/logger/plugin/view/logger_view.py` & `apptools-5.2.1/apptools/logger/plugin/view/logger_view.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/logger/ring_buffer.py` & `apptools-5.2.1/apptools/logger/ring_buffer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/naming/__init__.py` & `apptools-5.2.1/apptools/naming/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/naming/address.py` & `apptools-5.2.1/apptools/naming/address.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/naming/api.py` & `apptools-5.2.1/apptools/naming/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/naming/binding.py` & `apptools-5.2.1/apptools/naming/binding.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/naming/context.py` & `apptools-5.2.1/apptools/naming/context.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/naming/dir_context.py` & `apptools-5.2.1/apptools/naming/dir_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/naming/dynamic_context.py` & `apptools-5.2.1/apptools/naming/dynamic_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/naming/exception.py` & `apptools-5.2.1/apptools/naming/exception.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/naming/initial_context.py` & `apptools-5.2.1/apptools/naming/initial_context.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/naming/initial_context_factory.py` & `apptools-5.2.1/apptools/naming/initial_context_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/naming/naming_event.py` & `apptools-5.2.1/apptools/naming/naming_event.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/naming/naming_manager.py` & `apptools-5.2.1/apptools/naming/naming_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/naming/object_factory.py` & `apptools-5.2.1/apptools/naming/object_factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/naming/object_serializer.py` & `apptools-5.2.1/apptools/naming/object_serializer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/naming/py_context.py` & `apptools-5.2.1/apptools/naming/py_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/naming/py_object_factory.py` & `apptools-5.2.1/apptools/naming/py_object_factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/naming/pyfs_context.py` & `apptools-5.2.1/apptools/naming/pyfs_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/naming/pyfs_context_factory.py` & `apptools-5.2.1/apptools/naming/pyfs_object_factory.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,37 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
 # Thanks for using Enthought open source!
 """ Object factory for Python File System contexts. """
 
 
+# Enthought library imports.
+from apptools.io.api import File
+
 # Local imports.
 from .object_factory import ObjectFactory
 from .reference import Reference
 
 
-class PyFSContextFactory(ObjectFactory):
+class PyFSObjectFactory(ObjectFactory):
     """ Object factory for Python File System contexts. """
 
     ###########################################################################
     # 'ObjectFactory' interface.
     ###########################################################################
 
     def get_object_instance(self, state, name, context):
         """ Creates an object using the specified state information. """
 
         obj = None
 
         if isinstance(state, Reference):
-            if len(state.addresses) > 0:
-                if state.addresses[0].type == "pyfs_context":
-                    path = state.addresses[0].content
-                    obj = context._context_factory(name, path)
+            if state.class_name == "File" and len(state.addresses) > 0:
+                obj = File(state.addresses[0].content)
 
         return obj
```

### Comparing `apptools-5.2.0/apptools/naming/pyfs_initial_context_factory.py` & `apptools-5.2.1/apptools/naming/pyfs_initial_context_factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/naming/pyfs_object_factory.py` & `apptools-5.2.1/apptools/naming/pyfs_context_factory.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,36 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
 # Thanks for using Enthought open source!
 """ Object factory for Python File System contexts. """
 
 
-# Enthought library imports.
-from apptools.io.api import File
-
 # Local imports.
 from .object_factory import ObjectFactory
 from .reference import Reference
 
 
-class PyFSObjectFactory(ObjectFactory):
+class PyFSContextFactory(ObjectFactory):
     """ Object factory for Python File System contexts. """
 
     ###########################################################################
     # 'ObjectFactory' interface.
     ###########################################################################
 
     def get_object_instance(self, state, name, context):
         """ Creates an object using the specified state information. """
 
         obj = None
 
         if isinstance(state, Reference):
-            if state.class_name == "File" and len(state.addresses) > 0:
-                obj = File(state.addresses[0].content)
+            if len(state.addresses) > 0:
+                if state.addresses[0].type == "pyfs_context":
+                    path = state.addresses[0].content
+                    obj = context._context_factory(name, path)
 
         return obj
```

### Comparing `apptools-5.2.0/apptools/naming/pyfs_state_factory.py` & `apptools-5.2.1/apptools/naming/pyfs_state_factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/naming/reference.py` & `apptools-5.2.1/apptools/naming/reference.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/naming/referenceable.py` & `apptools-5.2.1/apptools/naming/referenceable.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/naming/referenceable_state_factory.py` & `apptools-5.2.1/apptools/naming/referenceable_state_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/naming/state_factory.py` & `apptools-5.2.1/apptools/naming/state_factory.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/naming/tests/test_context.py` & `apptools-5.2.1/apptools/naming/tests/test_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/naming/tests/test_dir_context.py` & `apptools-5.2.1/apptools/naming/tests/test_dir_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/naming/tests/test_object_serializer.py` & `apptools-5.2.1/apptools/naming/tests/test_object_serializer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/naming/tests/test_py_context.py` & `apptools-5.2.1/apptools/naming/tests/test_py_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/naming/tests/test_pyfs_context.py` & `apptools-5.2.1/apptools/naming/tests/test_pyfs_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/naming/trait_defs/__init__.py` & `apptools-5.2.1/apptools/naming/trait_defs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/naming/trait_defs/api.py` & `apptools-5.2.1/apptools/naming/trait_defs/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/naming/trait_defs/naming_traits.py` & `apptools-5.2.1/apptools/naming/trait_defs/naming_traits.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/naming/unique_name.py` & `apptools-5.2.1/apptools/naming/unique_name.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/persistence/__init__.py` & `apptools-5.2.1/apptools/persistence/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/persistence/file_path.py` & `apptools-5.2.1/apptools/persistence/file_path.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/persistence/project_loader.py` & `apptools-5.2.1/apptools/persistence/project_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/persistence/state_pickler.py` & `apptools-5.2.1/apptools/persistence/state_pickler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
@@ -389,19 +389,22 @@
 
         # Get the initargs.
         args = ()
         if hasattr(value, "__getinitargs__") and value.__getinitargs__:
             args = value.__getinitargs__()
 
         # Get the object state.
+        state = None
         if hasattr(value, "__get_pure_state__"):
             state = value.__get_pure_state__()
         elif hasattr(value, "__getstate__"):
+            # Note that __getstate__() may return None in Python >= 3.11
             state = value.__getstate__()
-        else:
+
+        if state is None:
             state = value.__dict__
 
         state.pop("__traits_version__", None)
 
         # Cache the args and state since they are likely to be gc'd.
         self._misc_cache.extend([args, state])
         # Register and process.
```

### Comparing `apptools-5.2.0/apptools/persistence/tests/state_function_classes.py` & `apptools-5.2.1/apptools/persistence/tests/state_function_classes.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/persistence/tests/test_class_mapping.py` & `apptools-5.2.1/apptools/persistence/tests/test_class_mapping.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/persistence/tests/test_file_path.py` & `apptools-5.2.1/apptools/persistence/tests/test_file_path.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/persistence/tests/test_state_function.py` & `apptools-5.2.1/apptools/persistence/tests/test_state_function.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/persistence/tests/test_state_pickler.py` & `apptools-5.2.1/apptools/persistence/tests/test_state_pickler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/persistence/tests/test_two_stage_unpickler.py` & `apptools-5.2.1/apptools/persistence/tests/test_two_stage_unpickler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/persistence/tests/test_version_registry.py` & `apptools-5.2.1/apptools/persistence/tests/test_version_registry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/persistence/updater.py` & `apptools-5.2.1/apptools/persistence/updater.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/persistence/version_registry.py` & `apptools-5.2.1/apptools/persistence/version_registry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/persistence/versioned_unpickler.py` & `apptools-5.2.1/apptools/persistence/versioned_unpickler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/preferences/api.py` & `apptools-5.2.1/apptools/preferences/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/preferences/i_preferences.py` & `apptools-5.2.1/apptools/preferences/i_preferences.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/preferences/package_globals.py` & `apptools-5.2.1/apptools/preferences/package_globals.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/preferences/preference_binding.py` & `apptools-5.2.1/apptools/preferences/preference_binding.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/preferences/preferences.py` & `apptools-5.2.1/apptools/preferences/preferences.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/preferences/preferences_helper.py` & `apptools-5.2.1/apptools/preferences/preferences_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/preferences/scoped_preferences.py` & `apptools-5.2.1/apptools/preferences/scoped_preferences.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/preferences/tests/py_config_example.ini` & `apptools-5.2.1/apptools/preferences/tests/py_config_example.ini`

 * *Files identical despite different names*

### Comparing `apptools-5.2.0/apptools/preferences/tests/py_config_file.py` & `apptools-5.2.1/apptools/preferences/tests/py_config_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/preferences/tests/test_preference_binding.py` & `apptools-5.2.1/apptools/preferences/tests/test_preference_binding.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/preferences/tests/test_preferences.py` & `apptools-5.2.1/apptools/preferences/tests/test_preferences.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/preferences/tests/test_preferences_helper.py` & `apptools-5.2.1/apptools/preferences/tests/test_preferences_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/preferences/tests/test_py_config_file.py` & `apptools-5.2.1/apptools/preferences/tests/test_py_config_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/preferences/tests/test_scoped_preferences.py` & `apptools-5.2.1/apptools/preferences/tests/test_scoped_preferences.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/preferences/ui/api.py` & `apptools-5.2.1/apptools/preferences/ui/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/preferences/ui/i_preferences_page.py` & `apptools-5.2.1/apptools/preferences/ui/i_preferences_page.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/preferences/ui/preferences_manager.py` & `apptools-5.2.1/apptools/preferences/ui/preferences_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/preferences/ui/preferences_node.py` & `apptools-5.2.1/apptools/preferences/ui/preferences_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/preferences/ui/preferences_page.py` & `apptools-5.2.1/apptools/preferences/ui/preferences_page.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/preferences/ui/tests/test_preferences_page.py` & `apptools-5.2.1/apptools/preferences/ui/tests/test_preferences_page.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/preferences/ui/tree_item.py` & `apptools-5.2.1/apptools/preferences/ui/tree_item.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/preferences/ui/widget_editor.py` & `apptools-5.2.1/apptools/preferences/ui/widget_editor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/scripting/__init__.py` & `apptools-5.2.1/apptools/scripting/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/scripting/api.py` & `apptools-5.2.1/apptools/scripting/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/scripting/package_globals.py` & `apptools-5.2.1/apptools/scripting/package_globals.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/scripting/recordable.py` & `apptools-5.2.1/apptools/scripting/recordable.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/scripting/recorder.py` & `apptools-5.2.1/apptools/scripting/recorder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/scripting/recorder_with_ui.py` & `apptools-5.2.1/apptools/scripting/recorder_with_ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/scripting/tests/test_recorder.py` & `apptools-5.2.1/apptools/scripting/tests/test_recorder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/scripting/util.py` & `apptools-5.2.1/apptools/scripting/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/selection/api.py` & `apptools-5.2.1/apptools/selection/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/selection/errors.py` & `apptools-5.2.1/apptools/selection/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/selection/i_selection.py` & `apptools-5.2.1/apptools/selection/i_selection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/selection/i_selection_provider.py` & `apptools-5.2.1/apptools/selection/i_selection_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/selection/list_selection.py` & `apptools-5.2.1/apptools/selection/list_selection.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/selection/selection_service.py` & `apptools-5.2.1/apptools/selection/selection_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/selection/tests/test_list_selection.py` & `apptools-5.2.1/apptools/selection/tests/test_list_selection.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/selection/tests/test_selection_service.py` & `apptools-5.2.1/apptools/selection/tests/test_selection_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/type_registry/api.py` & `apptools-5.2.1/apptools/undo/action/redo_action.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# ------------------------------------------------------------------------------
+# Copyright (c) 2007, Riverbank Computing Limited
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
-# license included in LICENSE.txt and may be redistributed only under
-# the conditions described in the aforementioned license. The license
+# license included in enthought/LICENSE.txt and may be redistributed only
+# under the conditions described in the aforementioned license.  The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
-#
 # Thanks for using Enthought open source!
+#
+# Author: Riverbank Computing Limited
+# Description: <Enthought undo package component>
+# ------------------------------------------------------------------------------
 
-""" API for the apptools.type_registry subpackage.
-
-- :class:`~.LazyRegistry`
-- :class:`~.TypeRegistry`
-"""
-
-from .type_registry import LazyRegistry, TypeRegistry
+from pyface.undo.action.api import RedoAction
```

### Comparing `apptools-5.2.0/apptools/type_registry/tests/dummies.py` & `apptools-5.2.1/apptools/type_registry/tests/dummies.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/type_registry/tests/test_lazy_registry.py` & `apptools-5.2.1/apptools/type_registry/tests/test_lazy_registry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/type_registry/tests/test_type_registry.py` & `apptools-5.2.1/apptools/type_registry/tests/test_type_registry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/type_registry/type_registry.py` & `apptools-5.2.1/apptools/type_registry/type_registry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/undo/__init__.py` & `apptools-5.2.1/apptools/undo/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/undo/abstract_command.py` & `apptools-5.2.1/apptools/undo/abstract_command.py`

 * *Files identical despite different names*

### Comparing `apptools-5.2.0/apptools/undo/action/__init__.py` & `apptools-5.2.1/apptools/undo/action/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/apptools/undo/action/abstract_command_stack_action.py` & `apptools-5.2.1/apptools/undo/action/abstract_command_stack_action.py`

 * *Files identical despite different names*

### Comparing `apptools-5.2.0/apptools/undo/action/api.py` & `apptools-5.2.1/apptools/undo/action/api.py`

 * *Files identical despite different names*

### Comparing `apptools-5.2.0/apptools/undo/action/command_action.py` & `apptools-5.2.1/apptools/undo/action/command_action.py`

 * *Files identical despite different names*

### Comparing `apptools-5.2.0/apptools/undo/action/redo_action.py` & `apptools-5.2.1/apptools/undo/action/undo_action.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 # Thanks for using Enthought open source!
 #
 # Author: Riverbank Computing Limited
 # Description: <Enthought undo package component>
 # ------------------------------------------------------------------------------
 
-from pyface.undo.action.api import RedoAction
+from pyface.undo.action.api import UndoAction
```

### Comparing `apptools-5.2.0/apptools/undo/action/undo_action.py` & `apptools-5.2.1/apptools/undo/i_command_stack.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 # Thanks for using Enthought open source!
 #
 # Author: Riverbank Computing Limited
 # Description: <Enthought undo package component>
 # ------------------------------------------------------------------------------
 
-from pyface.undo.action.api import UndoAction
+from pyface.undo.api import ICommandStack
```

### Comparing `apptools-5.2.0/apptools/undo/api.py` & `apptools-5.2.1/apptools/undo/api.py`

 * *Files identical despite different names*

### Comparing `apptools-5.2.0/apptools/undo/command_stack.py` & `apptools-5.2.1/apptools/undo/command_stack.py`

 * *Files identical despite different names*

### Comparing `apptools-5.2.0/apptools/undo/i_command.py` & `apptools-5.2.1/apptools/undo/i_command.py`

 * *Files identical despite different names*

### Comparing `apptools-5.2.0/apptools/undo/i_command_stack.py` & `apptools-5.2.1/apptools/undo/undo_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # ------------------------------------------------------------------------------
-# Copyright (c) 2007, Riverbank Computing Limited
+# Copyright (c) 2008, Riverbank Computing Limited
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in enthought/LICENSE.txt and may be redistributed only
 # under the conditions described in the aforementioned license.  The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 # Thanks for using Enthought open source!
 #
 # Author: Riverbank Computing Limited
 # Description: <Enthought undo package component>
 # ------------------------------------------------------------------------------
 
-from pyface.undo.api import ICommandStack
+from pyface.undo.api import UndoManager
```

### Comparing `apptools-5.2.0/apptools/undo/i_undo_manager.py` & `apptools-5.2.1/apptools/undo/i_undo_manager.py`

 * *Files identical despite different names*

### Comparing `apptools-5.2.0/apptools/undo/undo_manager.py` & `apptools-5.2.1/apptools/version.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,25 @@
-# ------------------------------------------------------------------------------
-# Copyright (c) 2008, Riverbank Computing Limited
+# (C) Copyright 2008-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
-# license included in enthought/LICENSE.txt and may be redistributed only
-# under the conditions described in the aforementioned license.  The license
+# license included in LICENSE.txt and may be redistributed only under
+# the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
-# Thanks for using Enthought open source!
 #
-# Author: Riverbank Computing Limited
-# Description: <Enthought undo package component>
-# ------------------------------------------------------------------------------
+# Thanks for using Enthought open source!
+
+"""
+Version information for this Apptools distribution.
+
+This file is autogenerated by the Apptools setup.py script.
+"""
+
+#: The full version of the package, including a development suffix
+#: for unreleased versions of the package.
+version = "5.2.1"
+
+#: The Git revision from which this release was made.
+git_revision = "237c3195f37631b709dbb66a2e9e5959f4521e01"
 
-from pyface.undo.api import UndoManager
+#: Flag whether this is a final release
+is_released = True
```

### Comparing `apptools-5.2.0/apptools.egg-info/PKG-INFO` & `apptools-5.2.1/apptools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apptools
-Version: 5.2.0
+Version: 5.2.1
 Summary: application tools
 Home-page: https://docs.enthought.com/apptools
 Download-URL: https://www.github.com/enthought/apptools
 Author: Enthought, Inc.
 Author-email: info@enthought.com
 Maintainer: ETS Developers
 Maintainer-email: enthought-dev@enthought.com
```

### Comparing `apptools-5.2.0/apptools.egg-info/SOURCES.txt` & `apptools-5.2.1/apptools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apptools-5.2.0/docs/Makefile` & `apptools-5.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `apptools-5.2.0/docs/releases/README.rst` & `apptools-5.2.1/docs/releases/README.rst`

 * *Files identical despite different names*

### Comparing `apptools-5.2.0/docs/source/_static/default.css` & `apptools-5.2.1/docs/source/_static/default.css`

 * *Files identical despite different names*

### Comparing `apptools-5.2.0/docs/source/_static/e-logo-rev.png` & `apptools-5.2.1/docs/source/_static/e-logo-rev.png`

 * *Files identical despite different names*

### Comparing `apptools-5.2.0/docs/source/_static/et.ico` & `apptools-5.2.1/docs/source/_static/et.ico`

 * *Files identical despite different names*

### Comparing `apptools-5.2.0/docs/source/api/templates/module.rst_t` & `apptools-5.2.1/docs/source/api/templates/module.rst_t`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ..
-   (C) Copyright 2006-2022 Enthought, Inc., Austin, TX
+   (C) Copyright 2006-2023 Enthought, Inc., Austin, TX
    All rights reserved.
 
    This software is provided without warranty under the terms of the BSD
    license included in LICENSE.txt and may be redistributed only under
    the conditions described in the aforementioned license. The license
    is also available online at http://www.enthought.com/licenses/BSD.txt
```

### Comparing `apptools-5.2.0/docs/source/api/templates/package.rst_t` & `apptools-5.2.1/docs/source/api/templates/package.rst_t`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ..
-   (C) Copyright 2006-2022 Enthought, Inc., Austin, TX
+   (C) Copyright 2006-2023 Enthought, Inc., Austin, TX
    All rights reserved.
 
    This software is provided without warranty under the terms of the BSD
    license included in LICENSE.txt and may be redistributed only under
    the conditions described in the aforementioned license. The license
    is also available online at http://www.enthought.com/licenses/BSD.txt
```

### Comparing `apptools-5.2.0/docs/source/conf.py` & `apptools-5.2.1/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
@@ -45,15 +45,15 @@
 source_suffix = '.rst'
 
 # The master toctree document.
 master_doc = 'index'
 
 # General substitutions.
 project = 'apptools'
-copyright = '2008-2022, Enthought'
+copyright = '2008-2023, Enthought'
 
 # The default replacements for |version| and |release|, also used in various
 # other places throughout the built documents.
 version = release = apptools.__version__
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
```

### Comparing `apptools-5.2.0/docs/source/io/introduction.rst` & `apptools-5.2.1/docs/source/io/introduction.rst`

 * *Files identical despite different names*

### Comparing `apptools-5.2.0/docs/source/preferences/Preferences.rst` & `apptools-5.2.1/docs/source/preferences/Preferences.rst`

 * *Files identical despite different names*

### Comparing `apptools-5.2.0/docs/source/preferences/PreferencesInEnvisage.rst` & `apptools-5.2.1/docs/source/preferences/PreferencesInEnvisage.rst`

 * *Files identical despite different names*

### Comparing `apptools-5.2.0/docs/source/scripting/introduction.rst` & `apptools-5.2.1/docs/source/scripting/introduction.rst`

 * *Files identical despite different names*

### Comparing `apptools-5.2.0/docs/source/selection/selection.rst` & `apptools-5.2.1/docs/source/selection/selection.rst`

 * *Files identical despite different names*

### Comparing `apptools-5.2.0/docs/source/undo/Introduction.rst` & `apptools-5.2.1/docs/source/undo/Introduction.rst`

 * *Files identical despite different names*

### Comparing `apptools-5.2.0/examples/naming/images/closed_folder.png` & `apptools-5.2.1/examples/naming/images/closed_folder.png`

 * *Files identical despite different names*

### Comparing `apptools-5.2.0/examples/naming/images/open_folder.png` & `apptools-5.2.1/examples/naming/images/open_folder.png`

 * *Files identical despite different names*

### Comparing `apptools-5.2.0/examples/naming/simple.py` & `apptools-5.2.1/examples/naming/simple.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/examples/preferences/preferences_manager.py` & `apptools-5.2.1/examples/preferences/preferences_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/examples/undo/commands.py` & `apptools-5.2.1/examples/undo/commands.py`

 * *Files identical despite different names*

### Comparing `apptools-5.2.0/examples/undo/example.py` & `apptools-5.2.1/examples/undo/example.py`

 * *Files identical despite different names*

### Comparing `apptools-5.2.0/examples/undo/example_editor_manager.py` & `apptools-5.2.1/examples/undo/example_editor_manager.py`

 * *Files identical despite different names*

### Comparing `apptools-5.2.0/examples/undo/example_undo_window.py` & `apptools-5.2.1/examples/undo/example_undo_window.py`

 * *Files identical despite different names*

### Comparing `apptools-5.2.0/examples/undo/model.py` & `apptools-5.2.1/examples/undo/model.py`

 * *Files identical despite different names*

### Comparing `apptools-5.2.0/image_LICENSE.txt` & `apptools-5.2.1/image_LICENSE.txt`

 * *Files identical despite different names*

### Comparing `apptools-5.2.0/image_LICENSE_CP.txt` & `apptools-5.2.1/image_LICENSE_CP.txt`

 * *Files identical despite different names*

### Comparing `apptools-5.2.0/integrationtests/persistence/test_persistence.py` & `apptools-5.2.1/integrationtests/persistence/test_persistence.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/integrationtests/persistence/update1.py` & `apptools-5.2.1/integrationtests/persistence/update1.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/integrationtests/persistence/update2.py` & `apptools-5.2.1/integrationtests/persistence/update2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/integrationtests/persistence/update3.py` & `apptools-5.2.1/integrationtests/persistence/update3.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `apptools-5.2.0/setup.py` & `apptools-5.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2008-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2008-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
@@ -16,15 +16,15 @@
 
 # Version information; update this by hand when making a new bugfix or feature
 # release. The actual package version is autogenerated from this information
 # together with information from the version control system, and then injected
 # into the package source.
 MAJOR = 5
 MINOR = 2
-MICRO = 0
+MICRO = 1
 PRERELEASE = ""
 IS_RELEASED = True
 
 # If this file is part of a Git export (for example created with "git archive",
 # or downloaded from GitHub), ARCHIVE_COMMIT_HASH gives the full hash of the
 # commit that was exported.
 ARCHIVE_COMMIT_HASH = "$Format:%H$"
@@ -36,15 +36,15 @@
 # Paths to the autogenerated version file and the Git directory.
 HERE = os.path.abspath(os.path.dirname(__file__))
 VERSION_FILE = os.path.join(HERE, "apptools", "version.py")
 GIT_DIRECTORY = os.path.join(HERE, ".git")
 
 # Template for the autogenerated version file.
 VERSION_FILE_TEMPLATE = '''\
-# (C) Copyright 2008-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2008-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

