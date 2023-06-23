# Comparing `tmp/automation_editor_dev-0.0.8.tar.gz` & `tmp/automation_editor_dev-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automation_editor_dev-0.0.8.tar", last modified: Mon May 22 09:27:44 2023, max compression
+gzip compressed data, was "automation_editor_dev-0.0.9.tar", last modified: Wed May 24 09:59:21 2023, max compression
```

## Comparing `automation_editor_dev-0.0.8.tar` & `automation_editor_dev-0.0.9.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 09:27:44.075374 automation_editor_dev-0.0.8/
--rw-rw-rw-   0        0        0     1085 2023-04-19 01:59:04.000000 automation_editor_dev-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     5889 2023-05-22 09:27:44.073867 automation_editor_dev-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     5065 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 09:27:43.878141 automation_editor_dev-0.0.8/automation_editor/
--rw-rw-rw-   0        0        0      130 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.8/automation_editor/__init__.py
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.8/automation_editor/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 09:27:43.881272 automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 09:27:43.888288 automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/editor_main/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/editor_main/__init__.py
--rw-rw-rw-   0        0        0     2087 2023-05-22 09:17:26.000000 automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/editor_main/main_ui.py
-drwxrwxrwx   0        0        0        0 2023-05-22 09:27:43.890286 automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/menu/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/menu/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 09:27:43.896297 automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/menu/api_testka_menu/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/menu/api_testka_menu/__init__.py
--rw-rw-rw-   0        0        0     4016 2023-05-22 01:10:45.000000 automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/menu/api_testka_menu/build_api_testka_menu.py
-drwxrwxrwx   0        0        0        0 2023-05-22 09:27:43.902770 automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/menu/auto_control_menu/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/menu/auto_control_menu/__init__.py
--rw-rw-rw-   0        0        0     4145 2023-05-22 01:10:45.000000 automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/menu/auto_control_menu/build_autocontrol_menu.py
-drwxrwxrwx   0        0        0        0 2023-05-22 09:27:43.908825 automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/menu/install_menu/
--rw-rw-rw-   0        0        0        0 2023-05-03 02:30:10.000000 automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/menu/install_menu/__init__.py
--rw-rw-rw-   0        0        0     3604 2023-05-22 01:10:45.000000 automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/menu/install_menu/build_install_menu.py
-drwxrwxrwx   0        0        0        0 2023-05-22 09:27:43.915331 automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/menu/load_density_menu/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/menu/load_density_menu/__init__.py
--rw-rw-rw-   0        0        0     4179 2023-05-22 01:10:45.000000 automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/menu/load_density_menu/build_load_density_menu.py
-drwxrwxrwx   0        0        0        0 2023-05-22 09:27:43.923862 automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/menu/web_runner_menu/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/menu/web_runner_menu/__init__.py
--rw-rw-rw-   0        0        0     4056 2023-05-22 01:10:45.000000 automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/menu/web_runner_menu/build_webrunner_menu.py
-drwxrwxrwx   0        0        0        0 2023-05-22 09:27:43.931263 automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/show_code_window/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/show_code_window/__init__.py
--rw-rw-rw-   0        0        0      791 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/show_code_window/code_window.py
-drwxrwxrwx   0        0        0        0 2023-05-22 09:27:43.942280 automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/syntax/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/syntax/__init__.py
--rw-rw-rw-   0        0        0      785 2023-05-22 01:10:45.000000 automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/syntax/syntax_extend.py
--rw-rw-rw-   0        0        0     3257 2023-05-19 03:00:53.000000 automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/syntax/syntax_keyword.py
-drwxrwxrwx   0        0        0        0 2023-05-22 09:27:43.946289 automation_editor_dev-0.0.8/automation_editor/extend/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.8/automation_editor/extend/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 09:27:43.952828 automation_editor_dev-0.0.8/automation_editor/extend/mail_thunder_extend/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.8/automation_editor/extend/mail_thunder_extend/__init__.py
--rw-rw-rw-   0        0        0     1704 2023-05-22 01:10:45.000000 automation_editor_dev-0.0.8/automation_editor/extend/mail_thunder_extend/mail_thunder_setting.py
-drwxrwxrwx   0        0        0        0 2023-05-22 09:27:43.956022 automation_editor_dev-0.0.8/automation_editor/utils/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.8/automation_editor/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 09:27:43.968093 automation_editor_dev-0.0.8/automation_editor/utils/exception/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.8/automation_editor/utils/exception/__init__.py
--rw-rw-rw-   0        0        0     1513 2023-05-19 03:12:11.000000 automation_editor_dev-0.0.8/automation_editor/utils/exception/exception_tags.py
--rw-rw-rw-   0        0        0      608 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.8/automation_editor/utils/exception/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-22 09:27:43.974096 automation_editor_dev-0.0.8/automation_editor/utils/file_process/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.8/automation_editor/utils/file_process/__init__.py
--rw-rw-rw-   0        0        0     1171 2023-05-02 09:53:50.000000 automation_editor_dev-0.0.8/automation_editor/utils/file_process/get_dir_file_list.py
-drwxrwxrwx   0        0        0        0 2023-05-22 09:27:43.983027 automation_editor_dev-0.0.8/automation_editor/utils/json_format/
--rw-rw-rw-   0        0        0        2 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.8/automation_editor/utils/json_format/__init__.py
--rw-rw-rw-   0        0        0     1005 2023-05-22 01:10:45.000000 automation_editor_dev-0.0.8/automation_editor/utils/json_format/json_process.py
-drwxrwxrwx   0        0        0        0 2023-05-22 09:27:43.986052 automation_editor_dev-0.0.8/automation_editor/utils/manager/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.8/automation_editor/utils/manager/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 09:27:43.992581 automation_editor_dev-0.0.8/automation_editor/utils/manager/package_manager/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.8/automation_editor/utils/manager/package_manager/__init__.py
--rw-rw-rw-   0        0        0      558 2023-05-03 02:11:15.000000 automation_editor_dev-0.0.8/automation_editor/utils/manager/package_manager/package_manager_class.py
-drwxrwxrwx   0        0        0        0 2023-05-22 09:27:44.003096 automation_editor_dev-0.0.8/automation_editor/utils/test_executor/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.8/automation_editor/utils/test_executor/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 09:27:44.010002 automation_editor_dev-0.0.8/automation_editor/utils/test_executor/api_testka/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.8/automation_editor/utils/test_executor/api_testka/__init__.py
--rw-rw-rw-   0        0        0     3935 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.8/automation_editor/utils/test_executor/api_testka/api_testka_process.py
-drwxrwxrwx   0        0        0        0 2023-05-22 09:27:44.017038 automation_editor_dev-0.0.8/automation_editor/utils/test_executor/auto_control/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.8/automation_editor/utils/test_executor/auto_control/__init__.py
--rw-rw-rw-   0        0        0     3939 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.8/automation_editor/utils/test_executor/auto_control/auto_control_process.py
--rw-rw-rw-   0        0        0      498 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.8/automation_editor/utils/test_executor/check_mail_thunder.py
-drwxrwxrwx   0        0        0        0 2023-05-22 09:27:44.025216 automation_editor_dev-0.0.8/automation_editor/utils/test_executor/load_density/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.8/automation_editor/utils/test_executor/load_density/__init__.py
--rw-rw-rw-   0        0        0     3949 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.8/automation_editor/utils/test_executor/load_density/load_density_process.py
--rw-rw-rw-   0        0        0     7109 2023-05-03 08:50:31.000000 automation_editor_dev-0.0.8/automation_editor/utils/test_executor/task_process_manager.py
-drwxrwxrwx   0        0        0        0 2023-05-22 09:27:44.033421 automation_editor_dev-0.0.8/automation_editor/utils/test_executor/web_runner/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.8/automation_editor/utils/test_executor/web_runner/__init__.py
--rw-rw-rw-   0        0        0     3897 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.8/automation_editor/utils/test_executor/web_runner/web_runner_process.py
-drwxrwxrwx   0        0        0        0 2023-05-22 09:27:44.070373 automation_editor_dev-0.0.8/automation_editor_dev.egg-info/
--rw-rw-rw-   0        0        0     5889 2023-05-22 09:27:43.000000 automation_editor_dev-0.0.8/automation_editor_dev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3099 2023-05-22 09:27:43.000000 automation_editor_dev-0.0.8/automation_editor_dev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 09:27:43.000000 automation_editor_dev-0.0.8/automation_editor_dev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      104 2023-05-22 09:27:43.000000 automation_editor_dev-0.0.8/automation_editor_dev.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-05-22 09:27:43.000000 automation_editor_dev-0.0.8/automation_editor_dev.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1272 2023-05-22 09:27:28.000000 automation_editor_dev-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-22 09:27:44.075374 automation_editor_dev-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-24 09:59:21.837050 automation_editor_dev-0.0.9/
+-rw-rw-rw-   0        0        0     1085 2023-04-19 01:59:04.000000 automation_editor_dev-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     5116 2023-05-24 09:59:21.836053 automation_editor_dev-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4292 2023-05-22 10:04:41.000000 automation_editor_dev-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-24 09:59:21.451814 automation_editor_dev-0.0.9/automation_editor/
+-rw-rw-rw-   0        0        0      130 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.9/automation_editor/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.9/automation_editor/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:59:21.456218 automation_editor_dev-0.0.9/automation_editor/automation_editor_ui/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.9/automation_editor/automation_editor_ui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:59:21.474094 automation_editor_dev-0.0.9/automation_editor/automation_editor_ui/editor_main/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.9/automation_editor/automation_editor_ui/editor_main/__init__.py
+-rw-rw-rw-   0        0        0     2087 2023-05-22 09:17:26.000000 automation_editor_dev-0.0.9/automation_editor/automation_editor_ui/editor_main/main_ui.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:59:21.482122 automation_editor_dev-0.0.9/automation_editor/automation_editor_ui/menu/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.9/automation_editor/automation_editor_ui/menu/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:59:21.501361 automation_editor_dev-0.0.9/automation_editor/automation_editor_ui/menu/api_testka_menu/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.9/automation_editor/automation_editor_ui/menu/api_testka_menu/__init__.py
+-rw-rw-rw-   0        0        0     4016 2023-05-22 01:10:45.000000 automation_editor_dev-0.0.9/automation_editor/automation_editor_ui/menu/api_testka_menu/build_api_testka_menu.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:59:21.526088 automation_editor_dev-0.0.9/automation_editor/automation_editor_ui/menu/auto_control_menu/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.9/automation_editor/automation_editor_ui/menu/auto_control_menu/__init__.py
+-rw-rw-rw-   0        0        0     4145 2023-05-22 01:10:45.000000 automation_editor_dev-0.0.9/automation_editor/automation_editor_ui/menu/auto_control_menu/build_autocontrol_menu.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:59:21.543175 automation_editor_dev-0.0.9/automation_editor/automation_editor_ui/menu/install_menu/
+-rw-rw-rw-   0        0        0        0 2023-05-03 02:30:10.000000 automation_editor_dev-0.0.9/automation_editor/automation_editor_ui/menu/install_menu/__init__.py
+-rw-rw-rw-   0        0        0     3604 2023-05-22 01:10:45.000000 automation_editor_dev-0.0.9/automation_editor/automation_editor_ui/menu/install_menu/build_install_menu.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:59:21.561442 automation_editor_dev-0.0.9/automation_editor/automation_editor_ui/menu/load_density_menu/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.9/automation_editor/automation_editor_ui/menu/load_density_menu/__init__.py
+-rw-rw-rw-   0        0        0     4179 2023-05-22 01:10:45.000000 automation_editor_dev-0.0.9/automation_editor/automation_editor_ui/menu/load_density_menu/build_load_density_menu.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:59:21.583150 automation_editor_dev-0.0.9/automation_editor/automation_editor_ui/menu/web_runner_menu/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.9/automation_editor/automation_editor_ui/menu/web_runner_menu/__init__.py
+-rw-rw-rw-   0        0        0     4056 2023-05-22 01:10:45.000000 automation_editor_dev-0.0.9/automation_editor/automation_editor_ui/menu/web_runner_menu/build_webrunner_menu.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:59:21.602711 automation_editor_dev-0.0.9/automation_editor/automation_editor_ui/show_code_window/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.9/automation_editor/automation_editor_ui/show_code_window/__init__.py
+-rw-rw-rw-   0        0        0      791 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.9/automation_editor/automation_editor_ui/show_code_window/code_window.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:59:21.625877 automation_editor_dev-0.0.9/automation_editor/automation_editor_ui/syntax/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.9/automation_editor/automation_editor_ui/syntax/__init__.py
+-rw-rw-rw-   0        0        0      785 2023-05-22 01:10:45.000000 automation_editor_dev-0.0.9/automation_editor/automation_editor_ui/syntax/syntax_extend.py
+-rw-rw-rw-   0        0        0     3257 2023-05-19 03:00:53.000000 automation_editor_dev-0.0.9/automation_editor/automation_editor_ui/syntax/syntax_keyword.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:59:21.631881 automation_editor_dev-0.0.9/automation_editor/extend/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.9/automation_editor/extend/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:59:21.647920 automation_editor_dev-0.0.9/automation_editor/extend/mail_thunder_extend/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.9/automation_editor/extend/mail_thunder_extend/__init__.py
+-rw-rw-rw-   0        0        0     1704 2023-05-22 01:10:45.000000 automation_editor_dev-0.0.9/automation_editor/extend/mail_thunder_extend/mail_thunder_setting.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:59:21.652229 automation_editor_dev-0.0.9/automation_editor/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.9/automation_editor/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:59:21.672954 automation_editor_dev-0.0.9/automation_editor/utils/exception/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.9/automation_editor/utils/exception/__init__.py
+-rw-rw-rw-   0        0        0     1513 2023-05-19 03:12:11.000000 automation_editor_dev-0.0.9/automation_editor/utils/exception/exception_tags.py
+-rw-rw-rw-   0        0        0      608 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.9/automation_editor/utils/exception/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:59:21.685928 automation_editor_dev-0.0.9/automation_editor/utils/file_process/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.9/automation_editor/utils/file_process/__init__.py
+-rw-rw-rw-   0        0        0     1171 2023-05-02 09:53:50.000000 automation_editor_dev-0.0.9/automation_editor/utils/file_process/get_dir_file_list.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:59:21.705764 automation_editor_dev-0.0.9/automation_editor/utils/json_format/
+-rw-rw-rw-   0        0        0        2 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.9/automation_editor/utils/json_format/__init__.py
+-rw-rw-rw-   0        0        0     1005 2023-05-22 01:10:45.000000 automation_editor_dev-0.0.9/automation_editor/utils/json_format/json_process.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:59:21.711183 automation_editor_dev-0.0.9/automation_editor/utils/manager/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.9/automation_editor/utils/manager/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:59:21.724608 automation_editor_dev-0.0.9/automation_editor/utils/manager/package_manager/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.9/automation_editor/utils/manager/package_manager/__init__.py
+-rw-rw-rw-   0        0        0      558 2023-05-03 02:11:15.000000 automation_editor_dev-0.0.9/automation_editor/utils/manager/package_manager/package_manager_class.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:59:21.745032 automation_editor_dev-0.0.9/automation_editor/utils/test_executor/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.9/automation_editor/utils/test_executor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:59:21.757061 automation_editor_dev-0.0.9/automation_editor/utils/test_executor/api_testka/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.9/automation_editor/utils/test_executor/api_testka/__init__.py
+-rw-rw-rw-   0        0        0     3935 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.9/automation_editor/utils/test_executor/api_testka/api_testka_process.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:59:21.770585 automation_editor_dev-0.0.9/automation_editor/utils/test_executor/auto_control/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.9/automation_editor/utils/test_executor/auto_control/__init__.py
+-rw-rw-rw-   0        0        0     3939 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.9/automation_editor/utils/test_executor/auto_control/auto_control_process.py
+-rw-rw-rw-   0        0        0      498 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.9/automation_editor/utils/test_executor/check_mail_thunder.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:59:21.783104 automation_editor_dev-0.0.9/automation_editor/utils/test_executor/load_density/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.9/automation_editor/utils/test_executor/load_density/__init__.py
+-rw-rw-rw-   0        0        0     3949 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.9/automation_editor/utils/test_executor/load_density/load_density_process.py
+-rw-rw-rw-   0        0        0     7109 2023-05-03 08:50:31.000000 automation_editor_dev-0.0.9/automation_editor/utils/test_executor/task_process_manager.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:59:21.796455 automation_editor_dev-0.0.9/automation_editor/utils/test_executor/web_runner/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.9/automation_editor/utils/test_executor/web_runner/__init__.py
+-rw-rw-rw-   0        0        0     3897 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.9/automation_editor/utils/test_executor/web_runner/web_runner_process.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:59:21.832050 automation_editor_dev-0.0.9/automation_editor_dev.egg-info/
+-rw-rw-rw-   0        0        0     5116 2023-05-24 09:59:21.000000 automation_editor_dev-0.0.9/automation_editor_dev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3099 2023-05-24 09:59:21.000000 automation_editor_dev-0.0.9/automation_editor_dev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 09:59:21.000000 automation_editor_dev-0.0.9/automation_editor_dev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      104 2023-05-24 09:59:21.000000 automation_editor_dev-0.0.9/automation_editor_dev.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-24 09:59:21.000000 automation_editor_dev-0.0.9/automation_editor_dev.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1272 2023-05-24 09:59:01.000000 automation_editor_dev-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-24 09:59:21.837050 automation_editor_dev-0.0.9/setup.cfg
```

### Comparing `automation_editor_dev-0.0.8/LICENSE` & `automation_editor_dev-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.8/PKG-INFO` & `automation_editor_dev-0.0.9/automation_editor_dev.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: automation_editor_dev
-Version: 0.0.8
+Name: automation-editor-dev
+Version: 0.0.9
 Summary: Automation Editor for GUI, WEB, API, Load Automation
 Author-email: JE-Chen <jechenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Intergration-Automation-Testing/AutomationEditor
 Project-URL: Code, https://github.com/Intergration-Automation-Testing/AutomationEditor
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -107,18 +107,13 @@
 > * open log window to check automation result
 > * Send mail when automation failure (need to setting mail)
 
 ---
 
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/b7d32ed8600b4bd2a2f3e960f46f2ad0)](https://www.codacy.com/gh/JE-Chen/Integration-testing-environment/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=JE-Chen/Integration-testing-environment&amp;utm_campaign=Badge_Grade)
 
-[![CircleCI](https://dl.circleci.com/status-badge/img/gh/Integrated-Testing-Environment/Integration-testing-environment/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/Integrated-Testing-Environment/Integration-testing-environment/tree/main)
-
-[![GitHub Actions Dev](https://github.com/JE-Chen/Integration-testing-environment/actions/workflows/ITE-github-actions_dev.yml/badge.svg)](https://github.com/JE-Chen/Integration-testing-environment/actions/workflows/ITE-github-actions_dev.yml)
-
-[![GitHub Actions Stable](https://github.com/JE-Chen/Integration-testing-environment/actions/workflows/ITE-github-actions_stable.yml/badge.svg)](https://github.com/JE-Chen/Integration-testing-environment/actions/workflows/ITE-github-actions_stable.yml)
 
 ### install
 #### we suggest install full package
 * pip install automation_editor[full_extension]
 #### if we don't want to use send after test
 * pip install automation_editor
```

### Comparing `automation_editor_dev-0.0.8/README.md` & `automation_editor_dev-0.0.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+Metadata-Version: 2.1
+Name: automation_editor_dev
+Version: 0.0.9
+Summary: Automation Editor for GUI, WEB, API, Load Automation
+Author-email: JE-Chen <jechenmailman@gmail.com>
+License: MIT
+Project-URL: Homepage, https://github.com/Intergration-Automation-Testing/AutomationEditor
+Project-URL: Code, https://github.com/Intergration-Automation-Testing/AutomationEditor
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Environment :: Win32 (MS Windows)
+Classifier: Environment :: MacOS X
+Classifier: Environment :: X11 Applications
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: full_extension
+License-File: LICENSE
+
 # Table of contents
 > Editor components \
 > GUI components \
 > WEB components \
 > API components \
 > Load components
 ---
@@ -87,18 +107,13 @@
 > * open log window to check automation result
 > * Send mail when automation failure (need to setting mail)
 
 ---
 
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/b7d32ed8600b4bd2a2f3e960f46f2ad0)](https://www.codacy.com/gh/JE-Chen/Integration-testing-environment/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=JE-Chen/Integration-testing-environment&amp;utm_campaign=Badge_Grade)
 
-[![CircleCI](https://dl.circleci.com/status-badge/img/gh/Integrated-Testing-Environment/Integration-testing-environment/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/Integrated-Testing-Environment/Integration-testing-environment/tree/main)
-
-[![GitHub Actions Dev](https://github.com/JE-Chen/Integration-testing-environment/actions/workflows/ITE-github-actions_dev.yml/badge.svg)](https://github.com/JE-Chen/Integration-testing-environment/actions/workflows/ITE-github-actions_dev.yml)
-
-[![GitHub Actions Stable](https://github.com/JE-Chen/Integration-testing-environment/actions/workflows/ITE-github-actions_stable.yml/badge.svg)](https://github.com/JE-Chen/Integration-testing-environment/actions/workflows/ITE-github-actions_stable.yml)
 
 ### install
 #### we suggest install full package
 * pip install automation_editor[full_extension]
 #### if we don't want to use send after test
 * pip install automation_editor
```

### Comparing `automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/editor_main/main_ui.py` & `automation_editor_dev-0.0.9/automation_editor/automation_editor_ui/editor_main/main_ui.py`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/menu/api_testka_menu/build_api_testka_menu.py` & `automation_editor_dev-0.0.9/automation_editor/automation_editor_ui/menu/api_testka_menu/build_api_testka_menu.py`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/menu/auto_control_menu/build_autocontrol_menu.py` & `automation_editor_dev-0.0.9/automation_editor/automation_editor_ui/menu/auto_control_menu/build_autocontrol_menu.py`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/menu/install_menu/build_install_menu.py` & `automation_editor_dev-0.0.9/automation_editor/automation_editor_ui/menu/install_menu/build_install_menu.py`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/menu/load_density_menu/build_load_density_menu.py` & `automation_editor_dev-0.0.9/automation_editor/automation_editor_ui/menu/load_density_menu/build_load_density_menu.py`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/menu/web_runner_menu/build_webrunner_menu.py` & `automation_editor_dev-0.0.9/automation_editor/automation_editor_ui/menu/web_runner_menu/build_webrunner_menu.py`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/show_code_window/code_window.py` & `automation_editor_dev-0.0.9/automation_editor/automation_editor_ui/show_code_window/code_window.py`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/syntax/syntax_extend.py` & `automation_editor_dev-0.0.9/automation_editor/automation_editor_ui/syntax/syntax_extend.py`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/syntax/syntax_keyword.py` & `automation_editor_dev-0.0.9/automation_editor/automation_editor_ui/syntax/syntax_keyword.py`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.8/automation_editor/extend/mail_thunder_extend/mail_thunder_setting.py` & `automation_editor_dev-0.0.9/automation_editor/extend/mail_thunder_extend/mail_thunder_setting.py`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.8/automation_editor/utils/exception/exception_tags.py` & `automation_editor_dev-0.0.9/automation_editor/utils/exception/exception_tags.py`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.8/automation_editor/utils/exception/exceptions.py` & `automation_editor_dev-0.0.9/automation_editor/utils/exception/exceptions.py`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.8/automation_editor/utils/file_process/get_dir_file_list.py` & `automation_editor_dev-0.0.9/automation_editor/utils/file_process/get_dir_file_list.py`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.8/automation_editor/utils/json_format/json_process.py` & `automation_editor_dev-0.0.9/automation_editor/utils/json_format/json_process.py`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.8/automation_editor/utils/manager/package_manager/package_manager_class.py` & `automation_editor_dev-0.0.9/automation_editor/utils/manager/package_manager/package_manager_class.py`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.8/automation_editor/utils/test_executor/api_testka/api_testka_process.py` & `automation_editor_dev-0.0.9/automation_editor/utils/test_executor/api_testka/api_testka_process.py`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.8/automation_editor/utils/test_executor/auto_control/auto_control_process.py` & `automation_editor_dev-0.0.9/automation_editor/utils/test_executor/auto_control/auto_control_process.py`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.8/automation_editor/utils/test_executor/load_density/load_density_process.py` & `automation_editor_dev-0.0.9/automation_editor/utils/test_executor/load_density/load_density_process.py`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.8/automation_editor/utils/test_executor/task_process_manager.py` & `automation_editor_dev-0.0.9/automation_editor/utils/test_executor/task_process_manager.py`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.8/automation_editor/utils/test_executor/web_runner/web_runner_process.py` & `automation_editor_dev-0.0.9/automation_editor/utils/test_executor/web_runner/web_runner_process.py`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.8/automation_editor_dev.egg-info/SOURCES.txt` & `automation_editor_dev-0.0.9/automation_editor_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.8/pyproject.toml` & `automation_editor_dev-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # This is dev version
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "automation_editor_dev"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
     { name = "JE-Chen", email = "jechenmailman@gmail.com" },
 ]
 description = "Automation Editor for GUI, WEB, API, Load Automation"
 requires-python = ">=3.8"
 license = { text = "MIT" }
 dependencies = [
```

