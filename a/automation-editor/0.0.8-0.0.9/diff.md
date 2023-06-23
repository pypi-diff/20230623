# Comparing `tmp/automation_editor-0.0.8.tar.gz` & `tmp/automation_editor-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automation_editor-0.0.8.tar", last modified: Mon May 22 09:26:56 2023, max compression
+gzip compressed data, was "automation_editor-0.0.9.tar", last modified: Wed May 24 10:01:06 2023, max compression
```

## Comparing `automation_editor-0.0.8.tar` & `automation_editor-0.0.9.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 09:26:56.764515 automation_editor-0.0.8/
--rw-rw-rw-   0        0        0     1085 2023-04-19 01:59:04.000000 automation_editor-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     5885 2023-05-22 09:26:56.763515 automation_editor-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     5065 2023-05-02 01:28:19.000000 automation_editor-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 09:26:56.566005 automation_editor-0.0.8/automation_editor/
--rw-rw-rw-   0        0        0      130 2023-05-02 01:28:19.000000 automation_editor-0.0.8/automation_editor/__init__.py
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.8/automation_editor/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 09:26:56.599372 automation_editor-0.0.8/automation_editor/automation_editor_ui/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.8/automation_editor/automation_editor_ui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 09:26:56.607406 automation_editor-0.0.8/automation_editor/automation_editor_ui/editor_main/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.8/automation_editor/automation_editor_ui/editor_main/__init__.py
--rw-rw-rw-   0        0        0     2087 2023-05-22 09:17:26.000000 automation_editor-0.0.8/automation_editor/automation_editor_ui/editor_main/main_ui.py
-drwxrwxrwx   0        0        0        0 2023-05-22 09:26:56.610412 automation_editor-0.0.8/automation_editor/automation_editor_ui/menu/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.8/automation_editor/automation_editor_ui/menu/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 09:26:56.616419 automation_editor-0.0.8/automation_editor/automation_editor_ui/menu/api_testka_menu/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.8/automation_editor/automation_editor_ui/menu/api_testka_menu/__init__.py
--rw-rw-rw-   0        0        0     4016 2023-05-22 01:10:45.000000 automation_editor-0.0.8/automation_editor/automation_editor_ui/menu/api_testka_menu/build_api_testka_menu.py
-drwxrwxrwx   0        0        0        0 2023-05-22 09:26:56.625511 automation_editor-0.0.8/automation_editor/automation_editor_ui/menu/auto_control_menu/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.8/automation_editor/automation_editor_ui/menu/auto_control_menu/__init__.py
--rw-rw-rw-   0        0        0     4145 2023-05-22 01:10:45.000000 automation_editor-0.0.8/automation_editor/automation_editor_ui/menu/auto_control_menu/build_autocontrol_menu.py
-drwxrwxrwx   0        0        0        0 2023-05-22 09:26:56.633068 automation_editor-0.0.8/automation_editor/automation_editor_ui/menu/install_menu/
--rw-rw-rw-   0        0        0        0 2023-05-03 02:30:10.000000 automation_editor-0.0.8/automation_editor/automation_editor_ui/menu/install_menu/__init__.py
--rw-rw-rw-   0        0        0     3604 2023-05-22 01:10:45.000000 automation_editor-0.0.8/automation_editor/automation_editor_ui/menu/install_menu/build_install_menu.py
-drwxrwxrwx   0        0        0        0 2023-05-22 09:26:56.640621 automation_editor-0.0.8/automation_editor/automation_editor_ui/menu/load_density_menu/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.8/automation_editor/automation_editor_ui/menu/load_density_menu/__init__.py
--rw-rw-rw-   0        0        0     4179 2023-05-22 01:10:45.000000 automation_editor-0.0.8/automation_editor/automation_editor_ui/menu/load_density_menu/build_load_density_menu.py
-drwxrwxrwx   0        0        0        0 2023-05-22 09:26:56.647659 automation_editor-0.0.8/automation_editor/automation_editor_ui/menu/web_runner_menu/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.8/automation_editor/automation_editor_ui/menu/web_runner_menu/__init__.py
--rw-rw-rw-   0        0        0     4056 2023-05-22 01:10:45.000000 automation_editor-0.0.8/automation_editor/automation_editor_ui/menu/web_runner_menu/build_webrunner_menu.py
-drwxrwxrwx   0        0        0        0 2023-05-22 09:26:56.653664 automation_editor-0.0.8/automation_editor/automation_editor_ui/show_code_window/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.8/automation_editor/automation_editor_ui/show_code_window/__init__.py
--rw-rw-rw-   0        0        0      791 2023-05-02 01:28:19.000000 automation_editor-0.0.8/automation_editor/automation_editor_ui/show_code_window/code_window.py
-drwxrwxrwx   0        0        0        0 2023-05-22 09:26:56.666218 automation_editor-0.0.8/automation_editor/automation_editor_ui/syntax/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.8/automation_editor/automation_editor_ui/syntax/__init__.py
--rw-rw-rw-   0        0        0      785 2023-05-22 01:10:45.000000 automation_editor-0.0.8/automation_editor/automation_editor_ui/syntax/syntax_extend.py
--rw-rw-rw-   0        0        0     3257 2023-05-19 03:00:53.000000 automation_editor-0.0.8/automation_editor/automation_editor_ui/syntax/syntax_keyword.py
-drwxrwxrwx   0        0        0        0 2023-05-22 09:26:56.669737 automation_editor-0.0.8/automation_editor/extend/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.8/automation_editor/extend/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 09:26:56.677166 automation_editor-0.0.8/automation_editor/extend/mail_thunder_extend/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.8/automation_editor/extend/mail_thunder_extend/__init__.py
--rw-rw-rw-   0        0        0     1704 2023-05-22 01:10:45.000000 automation_editor-0.0.8/automation_editor/extend/mail_thunder_extend/mail_thunder_setting.py
-drwxrwxrwx   0        0        0        0 2023-05-22 09:26:56.680191 automation_editor-0.0.8/automation_editor/utils/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.8/automation_editor/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 09:26:56.691202 automation_editor-0.0.8/automation_editor/utils/exception/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.8/automation_editor/utils/exception/__init__.py
--rw-rw-rw-   0        0        0     1513 2023-05-19 03:12:11.000000 automation_editor-0.0.8/automation_editor/utils/exception/exception_tags.py
--rw-rw-rw-   0        0        0      608 2023-05-02 01:28:19.000000 automation_editor-0.0.8/automation_editor/utils/exception/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-22 09:26:56.698271 automation_editor-0.0.8/automation_editor/utils/file_process/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.8/automation_editor/utils/file_process/__init__.py
--rw-rw-rw-   0        0        0     1171 2023-05-02 09:53:50.000000 automation_editor-0.0.8/automation_editor/utils/file_process/get_dir_file_list.py
-drwxrwxrwx   0        0        0        0 2023-05-22 09:26:56.712296 automation_editor-0.0.8/automation_editor/utils/json_format/
--rw-rw-rw-   0        0        0        2 2023-05-02 01:28:19.000000 automation_editor-0.0.8/automation_editor/utils/json_format/__init__.py
--rw-rw-rw-   0        0        0     1005 2023-05-22 01:10:45.000000 automation_editor-0.0.8/automation_editor/utils/json_format/json_process.py
-drwxrwxrwx   0        0        0        0 2023-05-22 09:26:56.716314 automation_editor-0.0.8/automation_editor/utils/manager/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.8/automation_editor/utils/manager/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 09:26:56.723797 automation_editor-0.0.8/automation_editor/utils/manager/package_manager/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.8/automation_editor/utils/manager/package_manager/__init__.py
--rw-rw-rw-   0        0        0      558 2023-05-03 02:11:15.000000 automation_editor-0.0.8/automation_editor/utils/manager/package_manager/package_manager_class.py
-drwxrwxrwx   0        0        0        0 2023-05-22 09:26:56.732476 automation_editor-0.0.8/automation_editor/utils/test_executor/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.8/automation_editor/utils/test_executor/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 09:26:56.741532 automation_editor-0.0.8/automation_editor/utils/test_executor/api_testka/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.8/automation_editor/utils/test_executor/api_testka/__init__.py
--rw-rw-rw-   0        0        0     3935 2023-05-02 01:28:19.000000 automation_editor-0.0.8/automation_editor/utils/test_executor/api_testka/api_testka_process.py
-drwxrwxrwx   0        0        0        0 2023-05-22 09:26:56.748053 automation_editor-0.0.8/automation_editor/utils/test_executor/auto_control/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.8/automation_editor/utils/test_executor/auto_control/__init__.py
--rw-rw-rw-   0        0        0     3939 2023-05-02 01:28:19.000000 automation_editor-0.0.8/automation_editor/utils/test_executor/auto_control/auto_control_process.py
--rw-rw-rw-   0        0        0      498 2023-05-02 01:28:19.000000 automation_editor-0.0.8/automation_editor/utils/test_executor/check_mail_thunder.py
-drwxrwxrwx   0        0        0        0 2023-05-22 09:26:56.754053 automation_editor-0.0.8/automation_editor/utils/test_executor/load_density/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.8/automation_editor/utils/test_executor/load_density/__init__.py
--rw-rw-rw-   0        0        0     3949 2023-05-02 01:28:19.000000 automation_editor-0.0.8/automation_editor/utils/test_executor/load_density/load_density_process.py
--rw-rw-rw-   0        0        0     7109 2023-05-03 08:50:31.000000 automation_editor-0.0.8/automation_editor/utils/test_executor/task_process_manager.py
-drwxrwxrwx   0        0        0        0 2023-05-22 09:26:56.760512 automation_editor-0.0.8/automation_editor/utils/test_executor/web_runner/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.8/automation_editor/utils/test_executor/web_runner/__init__.py
--rw-rw-rw-   0        0        0     3897 2023-05-02 01:28:19.000000 automation_editor-0.0.8/automation_editor/utils/test_executor/web_runner/web_runner_process.py
-drwxrwxrwx   0        0        0        0 2023-05-22 09:26:56.596363 automation_editor-0.0.8/automation_editor.egg-info/
--rw-rw-rw-   0        0        0     5885 2023-05-22 09:26:56.000000 automation_editor-0.0.8/automation_editor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3079 2023-05-22 09:26:56.000000 automation_editor-0.0.8/automation_editor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 09:26:56.000000 automation_editor-0.0.8/automation_editor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      104 2023-05-22 09:26:56.000000 automation_editor-0.0.8/automation_editor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-05-22 09:26:56.000000 automation_editor-0.0.8/automation_editor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1280 2023-05-22 09:26:39.000000 automation_editor-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-22 09:26:56.766047 automation_editor-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-24 10:01:06.932906 automation_editor-0.0.9/
+-rw-rw-rw-   0        0        0     1085 2023-04-19 01:59:04.000000 automation_editor-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     5917 2023-05-24 10:01:06.931904 automation_editor-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     5097 2023-05-24 10:00:49.000000 automation_editor-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-24 10:01:06.747451 automation_editor-0.0.9/automation_editor/
+-rw-rw-rw-   0        0        0      130 2023-05-02 01:28:19.000000 automation_editor-0.0.9/automation_editor/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.9/automation_editor/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 10:01:06.785696 automation_editor-0.0.9/automation_editor/automation_editor_ui/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.9/automation_editor/automation_editor_ui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 10:01:06.791702 automation_editor-0.0.9/automation_editor/automation_editor_ui/editor_main/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.9/automation_editor/automation_editor_ui/editor_main/__init__.py
+-rw-rw-rw-   0        0        0     2087 2023-05-22 09:17:26.000000 automation_editor-0.0.9/automation_editor/automation_editor_ui/editor_main/main_ui.py
+drwxrwxrwx   0        0        0        0 2023-05-24 10:01:06.794728 automation_editor-0.0.9/automation_editor/automation_editor_ui/menu/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.9/automation_editor/automation_editor_ui/menu/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 10:01:06.800742 automation_editor-0.0.9/automation_editor/automation_editor_ui/menu/api_testka_menu/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.9/automation_editor/automation_editor_ui/menu/api_testka_menu/__init__.py
+-rw-rw-rw-   0        0        0     4016 2023-05-22 01:10:45.000000 automation_editor-0.0.9/automation_editor/automation_editor_ui/menu/api_testka_menu/build_api_testka_menu.py
+drwxrwxrwx   0        0        0        0 2023-05-24 10:01:06.807696 automation_editor-0.0.9/automation_editor/automation_editor_ui/menu/auto_control_menu/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.9/automation_editor/automation_editor_ui/menu/auto_control_menu/__init__.py
+-rw-rw-rw-   0        0        0     4145 2023-05-22 01:10:45.000000 automation_editor-0.0.9/automation_editor/automation_editor_ui/menu/auto_control_menu/build_autocontrol_menu.py
+drwxrwxrwx   0        0        0        0 2023-05-24 10:01:06.812696 automation_editor-0.0.9/automation_editor/automation_editor_ui/menu/install_menu/
+-rw-rw-rw-   0        0        0        0 2023-05-03 02:30:10.000000 automation_editor-0.0.9/automation_editor/automation_editor_ui/menu/install_menu/__init__.py
+-rw-rw-rw-   0        0        0     3604 2023-05-22 01:10:45.000000 automation_editor-0.0.9/automation_editor/automation_editor_ui/menu/install_menu/build_install_menu.py
+drwxrwxrwx   0        0        0        0 2023-05-24 10:01:06.820526 automation_editor-0.0.9/automation_editor/automation_editor_ui/menu/load_density_menu/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.9/automation_editor/automation_editor_ui/menu/load_density_menu/__init__.py
+-rw-rw-rw-   0        0        0     4179 2023-05-22 01:10:45.000000 automation_editor-0.0.9/automation_editor/automation_editor_ui/menu/load_density_menu/build_load_density_menu.py
+drwxrwxrwx   0        0        0        0 2023-05-24 10:01:06.827567 automation_editor-0.0.9/automation_editor/automation_editor_ui/menu/web_runner_menu/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.9/automation_editor/automation_editor_ui/menu/web_runner_menu/__init__.py
+-rw-rw-rw-   0        0        0     4056 2023-05-22 01:10:45.000000 automation_editor-0.0.9/automation_editor/automation_editor_ui/menu/web_runner_menu/build_webrunner_menu.py
+drwxrwxrwx   0        0        0        0 2023-05-24 10:01:06.834525 automation_editor-0.0.9/automation_editor/automation_editor_ui/show_code_window/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.9/automation_editor/automation_editor_ui/show_code_window/__init__.py
+-rw-rw-rw-   0        0        0      791 2023-05-02 01:28:19.000000 automation_editor-0.0.9/automation_editor/automation_editor_ui/show_code_window/code_window.py
+drwxrwxrwx   0        0        0        0 2023-05-24 10:01:06.843527 automation_editor-0.0.9/automation_editor/automation_editor_ui/syntax/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.9/automation_editor/automation_editor_ui/syntax/__init__.py
+-rw-rw-rw-   0        0        0      785 2023-05-22 01:10:45.000000 automation_editor-0.0.9/automation_editor/automation_editor_ui/syntax/syntax_extend.py
+-rw-rw-rw-   0        0        0     3257 2023-05-19 03:00:53.000000 automation_editor-0.0.9/automation_editor/automation_editor_ui/syntax/syntax_keyword.py
+drwxrwxrwx   0        0        0        0 2023-05-24 10:01:06.846544 automation_editor-0.0.9/automation_editor/extend/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.9/automation_editor/extend/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 10:01:06.852551 automation_editor-0.0.9/automation_editor/extend/mail_thunder_extend/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.9/automation_editor/extend/mail_thunder_extend/__init__.py
+-rw-rw-rw-   0        0        0     1704 2023-05-22 01:10:45.000000 automation_editor-0.0.9/automation_editor/extend/mail_thunder_extend/mail_thunder_setting.py
+drwxrwxrwx   0        0        0        0 2023-05-24 10:01:06.855800 automation_editor-0.0.9/automation_editor/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.9/automation_editor/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 10:01:06.865556 automation_editor-0.0.9/automation_editor/utils/exception/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.9/automation_editor/utils/exception/__init__.py
+-rw-rw-rw-   0        0        0     1513 2023-05-19 03:12:11.000000 automation_editor-0.0.9/automation_editor/utils/exception/exception_tags.py
+-rw-rw-rw-   0        0        0      608 2023-05-02 01:28:19.000000 automation_editor-0.0.9/automation_editor/utils/exception/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-24 10:01:06.871555 automation_editor-0.0.9/automation_editor/utils/file_process/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.9/automation_editor/utils/file_process/__init__.py
+-rw-rw-rw-   0        0        0     1171 2023-05-02 09:53:50.000000 automation_editor-0.0.9/automation_editor/utils/file_process/get_dir_file_list.py
+drwxrwxrwx   0        0        0        0 2023-05-24 10:01:06.879054 automation_editor-0.0.9/automation_editor/utils/json_format/
+-rw-rw-rw-   0        0        0        2 2023-05-02 01:28:19.000000 automation_editor-0.0.9/automation_editor/utils/json_format/__init__.py
+-rw-rw-rw-   0        0        0     1005 2023-05-22 01:10:45.000000 automation_editor-0.0.9/automation_editor/utils/json_format/json_process.py
+drwxrwxrwx   0        0        0        0 2023-05-24 10:01:06.884056 automation_editor-0.0.9/automation_editor/utils/manager/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.9/automation_editor/utils/manager/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 10:01:06.891167 automation_editor-0.0.9/automation_editor/utils/manager/package_manager/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.9/automation_editor/utils/manager/package_manager/__init__.py
+-rw-rw-rw-   0        0        0      558 2023-05-03 02:11:15.000000 automation_editor-0.0.9/automation_editor/utils/manager/package_manager/package_manager_class.py
+drwxrwxrwx   0        0        0        0 2023-05-24 10:01:06.901660 automation_editor-0.0.9/automation_editor/utils/test_executor/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.9/automation_editor/utils/test_executor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 10:01:06.909609 automation_editor-0.0.9/automation_editor/utils/test_executor/api_testka/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.9/automation_editor/utils/test_executor/api_testka/__init__.py
+-rw-rw-rw-   0        0        0     3935 2023-05-02 01:28:19.000000 automation_editor-0.0.9/automation_editor/utils/test_executor/api_testka/api_testka_process.py
+drwxrwxrwx   0        0        0        0 2023-05-24 10:01:06.915619 automation_editor-0.0.9/automation_editor/utils/test_executor/auto_control/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.9/automation_editor/utils/test_executor/auto_control/__init__.py
+-rw-rw-rw-   0        0        0     3939 2023-05-02 01:28:19.000000 automation_editor-0.0.9/automation_editor/utils/test_executor/auto_control/auto_control_process.py
+-rw-rw-rw-   0        0        0      498 2023-05-02 01:28:19.000000 automation_editor-0.0.9/automation_editor/utils/test_executor/check_mail_thunder.py
+drwxrwxrwx   0        0        0        0 2023-05-24 10:01:06.921621 automation_editor-0.0.9/automation_editor/utils/test_executor/load_density/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.9/automation_editor/utils/test_executor/load_density/__init__.py
+-rw-rw-rw-   0        0        0     3949 2023-05-02 01:28:19.000000 automation_editor-0.0.9/automation_editor/utils/test_executor/load_density/load_density_process.py
+-rw-rw-rw-   0        0        0     7109 2023-05-03 08:50:31.000000 automation_editor-0.0.9/automation_editor/utils/test_executor/task_process_manager.py
+drwxrwxrwx   0        0        0        0 2023-05-24 10:01:06.928619 automation_editor-0.0.9/automation_editor/utils/test_executor/web_runner/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.9/automation_editor/utils/test_executor/web_runner/__init__.py
+-rw-rw-rw-   0        0        0     3897 2023-05-02 01:28:19.000000 automation_editor-0.0.9/automation_editor/utils/test_executor/web_runner/web_runner_process.py
+drwxrwxrwx   0        0        0        0 2023-05-24 10:01:06.782711 automation_editor-0.0.9/automation_editor.egg-info/
+-rw-rw-rw-   0        0        0     5917 2023-05-24 10:01:06.000000 automation_editor-0.0.9/automation_editor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3079 2023-05-24 10:01:06.000000 automation_editor-0.0.9/automation_editor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 10:01:06.000000 automation_editor-0.0.9/automation_editor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      104 2023-05-24 10:01:06.000000 automation_editor-0.0.9/automation_editor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-24 10:01:06.000000 automation_editor-0.0.9/automation_editor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1280 2023-05-24 10:00:53.000000 automation_editor-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-24 10:01:06.933905 automation_editor-0.0.9/setup.cfg
```

### Comparing `automation_editor-0.0.8/LICENSE` & `automation_editor-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.8/PKG-INFO` & `automation_editor-0.0.9/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automation_editor
-Version: 0.0.8
+Version: 0.0.9
 Summary: Automation Editor for GUI, WEB, API, Load Automation
 Author-email: JE-Chen <jechenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Intergration-Automation-Testing/AutomationEditor
 Project-URL: Code, https://github.com/Intergration-Automation-Testing/AutomationEditor
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -107,18 +107,18 @@
 > * open log window to check automation result
 > * Send mail when automation failure (need to setting mail)
 
 ---
 
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/b7d32ed8600b4bd2a2f3e960f46f2ad0)](https://www.codacy.com/gh/JE-Chen/Integration-testing-environment/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=JE-Chen/Integration-testing-environment&amp;utm_campaign=Badge_Grade)
 
-[![CircleCI](https://dl.circleci.com/status-badge/img/gh/Integrated-Testing-Environment/Integration-testing-environment/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/Integrated-Testing-Environment/Integration-testing-environment/tree/main)
+[![AutomationEditor Stable Python3.8](https://github.com/Intergration-Automation-Testing/AutomationEditor/actions/workflows/stable_python3_8.yml/badge.svg)](https://github.com/Intergration-Automation-Testing/AutomationEditor/actions/workflows/stable_python3_8.yml)
 
-[![GitHub Actions Dev](https://github.com/JE-Chen/Integration-testing-environment/actions/workflows/ITE-github-actions_dev.yml/badge.svg)](https://github.com/JE-Chen/Integration-testing-environment/actions/workflows/ITE-github-actions_dev.yml)
+[![AutomationEditor Stable Python3.9](https://github.com/Intergration-Automation-Testing/AutomationEditor/actions/workflows/stable_python3_9.yml/badge.svg)](https://github.com/Intergration-Automation-Testing/AutomationEditor/actions/workflows/stable_python3_9.yml)
 
-[![GitHub Actions Stable](https://github.com/JE-Chen/Integration-testing-environment/actions/workflows/ITE-github-actions_stable.yml/badge.svg)](https://github.com/JE-Chen/Integration-testing-environment/actions/workflows/ITE-github-actions_stable.yml)
+[![AutomationEditor Stable Python3.10](https://github.com/Intergration-Automation-Testing/AutomationEditor/actions/workflows/stable_python3_10.yml/badge.svg)](https://github.com/Intergration-Automation-Testing/AutomationEditor/actions/workflows/stable_python3_10.yml)
 
 ### install
 #### we suggest install full package
 * pip install automation_editor[full_extension]
 #### if we don't want to use send after test
 * pip install automation_editor
```

### Comparing `automation_editor-0.0.8/README.md` & `automation_editor-0.0.9/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -87,18 +87,18 @@
 > * open log window to check automation result
 > * Send mail when automation failure (need to setting mail)
 
 ---
 
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/b7d32ed8600b4bd2a2f3e960f46f2ad0)](https://www.codacy.com/gh/JE-Chen/Integration-testing-environment/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=JE-Chen/Integration-testing-environment&amp;utm_campaign=Badge_Grade)
 
-[![CircleCI](https://dl.circleci.com/status-badge/img/gh/Integrated-Testing-Environment/Integration-testing-environment/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/Integrated-Testing-Environment/Integration-testing-environment/tree/main)
+[![AutomationEditor Stable Python3.8](https://github.com/Intergration-Automation-Testing/AutomationEditor/actions/workflows/stable_python3_8.yml/badge.svg)](https://github.com/Intergration-Automation-Testing/AutomationEditor/actions/workflows/stable_python3_8.yml)
 
-[![GitHub Actions Dev](https://github.com/JE-Chen/Integration-testing-environment/actions/workflows/ITE-github-actions_dev.yml/badge.svg)](https://github.com/JE-Chen/Integration-testing-environment/actions/workflows/ITE-github-actions_dev.yml)
+[![AutomationEditor Stable Python3.9](https://github.com/Intergration-Automation-Testing/AutomationEditor/actions/workflows/stable_python3_9.yml/badge.svg)](https://github.com/Intergration-Automation-Testing/AutomationEditor/actions/workflows/stable_python3_9.yml)
 
-[![GitHub Actions Stable](https://github.com/JE-Chen/Integration-testing-environment/actions/workflows/ITE-github-actions_stable.yml/badge.svg)](https://github.com/JE-Chen/Integration-testing-environment/actions/workflows/ITE-github-actions_stable.yml)
+[![AutomationEditor Stable Python3.10](https://github.com/Intergration-Automation-Testing/AutomationEditor/actions/workflows/stable_python3_10.yml/badge.svg)](https://github.com/Intergration-Automation-Testing/AutomationEditor/actions/workflows/stable_python3_10.yml)
 
 ### install
 #### we suggest install full package
 * pip install automation_editor[full_extension]
 #### if we don't want to use send after test
 * pip install automation_editor
```

### Comparing `automation_editor-0.0.8/automation_editor/automation_editor_ui/editor_main/main_ui.py` & `automation_editor-0.0.9/automation_editor/automation_editor_ui/editor_main/main_ui.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.8/automation_editor/automation_editor_ui/menu/api_testka_menu/build_api_testka_menu.py` & `automation_editor-0.0.9/automation_editor/automation_editor_ui/menu/api_testka_menu/build_api_testka_menu.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.8/automation_editor/automation_editor_ui/menu/auto_control_menu/build_autocontrol_menu.py` & `automation_editor-0.0.9/automation_editor/automation_editor_ui/menu/auto_control_menu/build_autocontrol_menu.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.8/automation_editor/automation_editor_ui/menu/install_menu/build_install_menu.py` & `automation_editor-0.0.9/automation_editor/automation_editor_ui/menu/install_menu/build_install_menu.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.8/automation_editor/automation_editor_ui/menu/load_density_menu/build_load_density_menu.py` & `automation_editor-0.0.9/automation_editor/automation_editor_ui/menu/load_density_menu/build_load_density_menu.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.8/automation_editor/automation_editor_ui/menu/web_runner_menu/build_webrunner_menu.py` & `automation_editor-0.0.9/automation_editor/automation_editor_ui/menu/web_runner_menu/build_webrunner_menu.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.8/automation_editor/automation_editor_ui/show_code_window/code_window.py` & `automation_editor-0.0.9/automation_editor/automation_editor_ui/show_code_window/code_window.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.8/automation_editor/automation_editor_ui/syntax/syntax_extend.py` & `automation_editor-0.0.9/automation_editor/automation_editor_ui/syntax/syntax_extend.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.8/automation_editor/automation_editor_ui/syntax/syntax_keyword.py` & `automation_editor-0.0.9/automation_editor/automation_editor_ui/syntax/syntax_keyword.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.8/automation_editor/extend/mail_thunder_extend/mail_thunder_setting.py` & `automation_editor-0.0.9/automation_editor/extend/mail_thunder_extend/mail_thunder_setting.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.8/automation_editor/utils/exception/exception_tags.py` & `automation_editor-0.0.9/automation_editor/utils/exception/exception_tags.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.8/automation_editor/utils/exception/exceptions.py` & `automation_editor-0.0.9/automation_editor/utils/exception/exceptions.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.8/automation_editor/utils/file_process/get_dir_file_list.py` & `automation_editor-0.0.9/automation_editor/utils/file_process/get_dir_file_list.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.8/automation_editor/utils/json_format/json_process.py` & `automation_editor-0.0.9/automation_editor/utils/json_format/json_process.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.8/automation_editor/utils/manager/package_manager/package_manager_class.py` & `automation_editor-0.0.9/automation_editor/utils/manager/package_manager/package_manager_class.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.8/automation_editor/utils/test_executor/api_testka/api_testka_process.py` & `automation_editor-0.0.9/automation_editor/utils/test_executor/api_testka/api_testka_process.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.8/automation_editor/utils/test_executor/auto_control/auto_control_process.py` & `automation_editor-0.0.9/automation_editor/utils/test_executor/auto_control/auto_control_process.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.8/automation_editor/utils/test_executor/load_density/load_density_process.py` & `automation_editor-0.0.9/automation_editor/utils/test_executor/load_density/load_density_process.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.8/automation_editor/utils/test_executor/task_process_manager.py` & `automation_editor-0.0.9/automation_editor/utils/test_executor/task_process_manager.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.8/automation_editor/utils/test_executor/web_runner/web_runner_process.py` & `automation_editor-0.0.9/automation_editor/utils/test_executor/web_runner/web_runner_process.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.8/automation_editor.egg-info/SOURCES.txt` & `automation_editor-0.0.9/automation_editor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.8/pyproject.toml` & `automation_editor-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # This is stable version
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "automation_editor"
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

