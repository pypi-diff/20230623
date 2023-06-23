# Comparing `tmp/taipy-gui-2.3.0.dev6.tar.gz` & `tmp/taipy-gui-3.0.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taipy-gui-2.3.0.dev6.tar", last modified: Tue Jun 13 17:34:24 2023, max compression
+gzip compressed data, was "taipy-gui-3.0.0.dev0.tar", last modified: Fri Jun 23 10:28:46 2023, max compression
```

## Comparing `taipy-gui-2.3.0.dev6.tar` & `taipy-gui-3.0.0.dev0.tar`

### file list

```diff
@@ -1,159 +1,160 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:34:24.657065 taipy-gui-2.3.0.dev6/
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-06-13 17:34:24.657065 taipy-gui-2.3.0.dev6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 17:34:24.657065 taipy-gui-2.3.0.dev6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-06-13 17:29:30.000000 taipy-gui-2.3.0.dev6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:34:24.625065 taipy-gui-2.3.0.dev6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:34:24.629065 taipy-gui-2.3.0.dev6/src/taipy/
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:34:24.629065 taipy-gui-2.3.0.dev6/src/taipy/gui/
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/_default_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/_gui_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/_gui_section.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/_page.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/_warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)    12148 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:34:24.633065 taipy-gui-2.3.0.dev6/src/taipy/gui/data/
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/data/array_dict_data_accessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/data/content_accessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/data/data_accessor.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/data/data_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/data/data_scope.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:34:24.633065 taipy-gui-2.3.0.dev6/src/taipy/gui/data/decimator/
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/data/decimator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/data/decimator/lttb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/data/decimator/minmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/data/decimator/rdp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/data/decimator/scatter_decimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/data/numpy_data_accessor.py
--rw-r--r--   0 runner    (1001) docker     (123)    16809 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/data/pandas_data_accessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:34:24.633065 taipy-gui-2.3.0.dev6/src/taipy/gui/extension/
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17246 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/extension/library.py
--rw-r--r--   0 runner    (1001) docker     (123)    91973 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)    15069 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/gui_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/icon.py
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/page.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/partial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:34:24.633065 taipy-gui-2.3.0.dev6/src/taipy/gui/renderers/
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/renderers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:34:24.633065 taipy-gui-2.3.0.dev6/src/taipy/gui/renderers/_html/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/renderers/_html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/renderers/_html/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/renderers/_html/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:34:24.633065 taipy-gui-2.3.0.dev6/src/taipy/gui/renderers/_markdown/
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/renderers/_markdown/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/renderers/_markdown/blocproc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/renderers/_markdown/control.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/renderers/_markdown/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/renderers/_markdown/postproc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10471 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/renderers/_markdown/preproc.py
--rw-r--r--   0 runner    (1001) docker     (123)    41559 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/renderers/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    23376 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/renderers/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/renderers/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/renderers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13085 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:34:24.637065 taipy-gui-2.3.0.dev6/src/taipy/gui/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/utils/_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/utils/_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/utils/_bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)    14942 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/utils/_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/utils/_locals_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/utils/_map_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/utils/_runtime_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/utils/_variable_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/utils/boolean.py
--rw-r--r--   0 runner    (1001) docker     (123)    10793 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/utils/chart_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/utils/clientvarname.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/utils/datatype.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/utils/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/utils/expr_var_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/utils/filename.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/utils/filter_locals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/utils/get_imported_var.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/utils/get_module_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/utils/getdatecolstrname.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/utils/html.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/utils/is_debugging.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/utils/isnotebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/utils/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/utils/singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/utils/table_col_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/utils/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/utils/varnamefromcontent.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/version.json
--rw-r--r--   0 runner    (1001) docker     (123)    56258 2023-06-13 17:28:46.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/viselements.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:34:24.653065 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-13 17:33:24.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/227.taipy-gui.js
--rw-r--r--   0 runner    (1001) docker     (123)   204350 2023-06-13 17:33:24.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/499.taipy-gui.js
--rw-r--r--   0 runner    (1001) docker     (123)  3591394 2023-06-13 17:33:24.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/660.taipy-gui.js
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-13 17:33:24.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/660.taipy-gui.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    11708 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/favicon.png
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/package.json
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:34:24.653065 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:34:24.653065 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/base/
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/base/base.css
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/base/fontfaces.css
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/base/typography.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:34:24.653065 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/blocks/
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/blocks/layout.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:34:24.657065 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/controls/
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/controls/button.css
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/controls/chart.css
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/controls/date.css
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/controls/expandable.css
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/controls/image.css
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/controls/input.css
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/controls/navbar.css
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/controls/number.css
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/controls/selector.css
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/controls/slider.css
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/controls/table.css
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/controls/toggle.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:34:24.657065 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/elements/
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/elements/card.css
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/elements/container.css
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/elements/header.css
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/elements/sidebar.css
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/stylekit.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:34:24.657065 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/utilities/colors.css
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/utilities/misc.css
--rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/utilities/spacing.css
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/utilities/typography.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:34:24.657065 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/variables/
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/variables/colors.css
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/variables/elements.css
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/variables/misc.css
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/variables/shapes.css
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/variables/spacing.css
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/variables/typography.css
--rw-r--r--   0 runner    (1001) docker     (123)   218114 2023-06-13 17:30:57.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/taipy-gui-deps-manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)  5259716 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/taipy-gui-deps.dll.js
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-13 17:30:57.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/taipy-gui-deps.dll.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/taipy-gui-dom.js
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/taipy-gui-dom.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10984 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/taipy-gui.d.ts
--rw-r--r--   0 runner    (1001) docker     (123)  1085147 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/taipy-gui.js
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-13 17:33:24.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/taipy-gui.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-13 17:34:13.000000 taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/taipy.status.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:34:24.657065 taipy-gui-2.3.0.dev6/src/taipy_gui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-06-13 17:34:24.000000 taipy-gui-2.3.0.dev6/src/taipy_gui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-06-13 17:34:24.000000 taipy-gui-2.3.0.dev6/src/taipy_gui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 17:34:24.000000 taipy-gui-2.3.0.dev6/src/taipy_gui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 17:34:14.000000 taipy-gui-2.3.0.dev6/src/taipy_gui.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-13 17:34:24.000000 taipy-gui-2.3.0.dev6/src/taipy_gui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-13 17:34:24.000000 taipy-gui-2.3.0.dev6/src/taipy_gui.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:46.955158 taipy-gui-3.0.0.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-06-23 10:28:46.955158 taipy-gui-3.0.0.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 10:28:46.955158 taipy-gui-3.0.0.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-06-23 10:24:33.000000 taipy-gui-3.0.0.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:46.927158 taipy-gui-3.0.0.dev0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:46.927158 taipy-gui-3.0.0.dev0/src/taipy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:46.927158 taipy-gui-3.0.0.dev0/src/taipy/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/_default_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/_gui_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/_gui_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12148 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:46.931158 taipy-gui-3.0.0.dev0/src/taipy/gui/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/data/array_dict_data_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/data/content_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/data/data_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/data/data_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/data/data_scope.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:46.931158 taipy-gui-3.0.0.dev0/src/taipy/gui/data/decimator/
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/data/decimator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/data/decimator/lttb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/data/decimator/minmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/data/decimator/rdp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/data/decimator/scatter_decimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/data/numpy_data_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16809 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/data/pandas_data_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:46.931158 taipy-gui-3.0.0.dev0/src/taipy/gui/extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17246 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/extension/library.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92173 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15529 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/gui_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/icon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/partial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:46.931158 taipy-gui-3.0.0.dev0/src/taipy/gui/renderers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/renderers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:46.931158 taipy-gui-3.0.0.dev0/src/taipy/gui/renderers/_html/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/renderers/_html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/renderers/_html/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/renderers/_html/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:46.931158 taipy-gui-3.0.0.dev0/src/taipy/gui/renderers/_markdown/
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/renderers/_markdown/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/renderers/_markdown/blocproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/renderers/_markdown/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/renderers/_markdown/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/renderers/_markdown/postproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10471 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/renderers/_markdown/preproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41961 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/renderers/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23376 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/renderers/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/renderers/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/renderers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13085 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:46.935158 taipy-gui-3.0.0.dev0/src/taipy/gui/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/utils/_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/utils/_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/utils/_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14942 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/utils/_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/utils/_locals_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/utils/_map_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/utils/_runtime_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/utils/_variable_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/utils/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10793 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/utils/chart_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/utils/clientvarname.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/utils/datatype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/utils/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/utils/expr_var_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/utils/filename.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/utils/filter_locals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/utils/get_imported_var.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/utils/get_module_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/utils/getdatecolstrname.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/utils/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/utils/is_debugging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/utils/isnotebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/utils/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/utils/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/utils/table_col_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/utils/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/utils/varnamefromcontent.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/version.json
+-rw-r--r--   0 runner    (1001) docker     (123)    56267 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/viselements.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:46.947158 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-23 10:27:57.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/227.taipy-gui.js
+-rw-r--r--   0 runner    (1001) docker     (123)   204350 2023-06-23 10:27:57.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/499.taipy-gui.js
+-rw-r--r--   0 runner    (1001) docker     (123)  3591394 2023-06-23 10:27:57.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/660.taipy-gui.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-23 10:27:57.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/660.taipy-gui.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    11708 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:46.947158 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:46.951158 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/base/
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/base/base.css
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/base/fontfaces.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/base/typography.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:46.951158 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/blocks/layout.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:46.951158 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/controls/
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/controls/button.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/controls/chart.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/controls/date.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/controls/expandable.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/controls/image.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/controls/input.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/controls/navbar.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/controls/number.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/controls/selector.css
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/controls/slider.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/controls/table.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/controls/toggle.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:46.951158 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/elements/
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/elements/card.css
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/elements/container.css
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/elements/header.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/elements/sidebar.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/stylekit.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:46.951158 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/utilities/colors.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/utilities/misc.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/utilities/spacing.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/utilities/typography.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:46.951158 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/variables/colors.css
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/variables/elements.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/variables/misc.css
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/variables/shapes.css
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/variables/spacing.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/variables/typography.css
+-rw-r--r--   0 runner    (1001) docker     (123)   218114 2023-06-23 10:25:50.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/taipy-gui-deps-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)  5259716 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/taipy-gui-deps.dll.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-23 10:25:50.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/taipy-gui-deps.dll.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/taipy-gui-dom.js
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/taipy-gui-dom.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10984 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/taipy-gui.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)  1085146 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/taipy-gui.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-23 10:27:57.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/taipy-gui.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/taipy.status.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:46.955158 taipy-gui-3.0.0.dev0/src/taipy_gui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-06-23 10:28:46.000000 taipy-gui-3.0.0.dev0/src/taipy_gui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-06-23 10:28:46.000000 taipy-gui-3.0.0.dev0/src/taipy_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 10:28:46.000000 taipy-gui-3.0.0.dev0/src/taipy_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 10:28:40.000000 taipy-gui-3.0.0.dev0/src/taipy_gui.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-23 10:28:46.000000 taipy-gui-3.0.0.dev0/src/taipy_gui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-23 10:28:46.000000 taipy-gui-3.0.0.dev0/src/taipy_gui.egg-info/top_level.txt
```

### Comparing `taipy-gui-2.3.0.dev6/LICENSE` & `taipy-gui-3.0.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/PKG-INFO` & `taipy-gui-3.0.0.dev0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipy-gui
-Version: 2.3.0.dev6
+Version: 3.0.0.dev0
 Summary: Low-code library to create graphical user interfaces on the Web for your Python applications.
 Home-page: https://github.com/avaiga/taipy-gui
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy-gui
 Classifier: Intended Audience :: Developers
@@ -43,44 +43,44 @@
 - [Contributing](#contributing)
 - [Code of conduct](#code-of-conduct)
 - [Directory Structure](#directory-structure)
 
 ## What is Taipy GUI
 
 Taipy is a Python library for creating Business Applications. More information on our
-[website](https://www.taipy.io). Taipy is split into multiple repositories including _taipy-gui_ to let users
+[website](https://www.taipy.io). Taipy is split into multiple repositories including `taipy-gui` to let users
 install the minimum they need.
 
-[Taipy GUI](https://github.com/Avaiga/taipy-gui) provides Python classes that make it easy to create powerful Web apps in minutes.
+[Taipy GUI](https://github.com/Avaiga/taipy-gui) provides Python classes that make it easy to create powerful web apps in minutes.
 
-A more in depth documentation of taipy can be found [here](https://docs.taipy.io/).
+A more in depth documentation of Taipy can be found [here](https://docs.taipy.io/).
 
 ## Installation
 
-Want to install and try _Taipy GUI_? Check out our [`INSTALLATION.md`](INSTALLATION.md) file.
+Want to install and try *Taipy GUI*? Check out our [`INSTALLATION.md`](INSTALLATION.md) file.
 
 ## Contributing
 
-Want to help build _Taipy GUI_? Check out our [`CONTRIBUTING.md`](CONTRIBUTING.md) file.
+Want to help build *Taipy GUI*? Check out our [`CONTRIBUTING.md`](CONTRIBUTING.md) file.
 
 ## Code of conduct
 
-Want to be part of the _Taipy GUI_ community? Check out our [`CODE_OF_CONDUCT.md`](CODE_OF_CONDUCT.md) file.
+Want to be part of the *Taipy GUI* community? Check out our [`CODE_OF_CONDUCT.md`](CODE_OF_CONDUCT.md) file.
 
 ## Directory Structure
 
 - `gui`: Graphical user interface related files;
 - `src/taipy/gui`: Python source files;
 - `tests/taipy/gui`: Unit tests;
-- `tools`: Files used to document _taipy-gui_;
-- `CODE_OF_CONDUCT.md`: Code of conduct for members and contributors of _taipy-gui_;
-- `CONTRIBUTING.md`: Instructions to contribute to _taipy-gui_;
-- `INSTALLATION.md`: Instructions to install _taipy-gui_;
+- `tools`: Files used to document `taipy-gui`;
+- `CODE_OF_CONDUCT.md`: Code of conduct for members and contributors of `taipy-gui`;
+- `CONTRIBUTING.md`: Instructions to contribute to `taipy-gui`;
+- `INSTALLATION.md`: Instructions to build and install `taipy-gui`;
 - `LICENSE`: The Apache 2.0 License;
 - `MANIFEST.in`: Build configuration file;
 - `mypy.ini`: [mypy](http://mypy-lang.org/) linter configuration file;
 - `Pipfile`: File used by the Pipenv virtual environment to manage project dependencies;
 - `pyproject.toml`: Python build configuration file use for linters here;
 - `pytest.ini`: [pytest](https://pytest.org/) configuration file;
 - `README.md`: Current file;
-- `setup.py`: The setup script managing building, distributing, and installing _taipy-gui_;
+- `setup.py`: The setup script managing building, distributing, and installing `taipy-gui`;
 - `tox.ini`: Contains test scenarios to be run.
```

### Comparing `taipy-gui-2.3.0.dev6/README.md` & `taipy-gui-3.0.0.dev0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -19,44 +19,44 @@
 - [Contributing](#contributing)
 - [Code of conduct](#code-of-conduct)
 - [Directory Structure](#directory-structure)
 
 ## What is Taipy GUI
 
 Taipy is a Python library for creating Business Applications. More information on our
-[website](https://www.taipy.io). Taipy is split into multiple repositories including _taipy-gui_ to let users
+[website](https://www.taipy.io). Taipy is split into multiple repositories including `taipy-gui` to let users
 install the minimum they need.
 
-[Taipy GUI](https://github.com/Avaiga/taipy-gui) provides Python classes that make it easy to create powerful Web apps in minutes.
+[Taipy GUI](https://github.com/Avaiga/taipy-gui) provides Python classes that make it easy to create powerful web apps in minutes.
 
-A more in depth documentation of taipy can be found [here](https://docs.taipy.io/).
+A more in depth documentation of Taipy can be found [here](https://docs.taipy.io/).
 
 ## Installation
 
-Want to install and try _Taipy GUI_? Check out our [`INSTALLATION.md`](INSTALLATION.md) file.
+Want to install and try *Taipy GUI*? Check out our [`INSTALLATION.md`](INSTALLATION.md) file.
 
 ## Contributing
 
-Want to help build _Taipy GUI_? Check out our [`CONTRIBUTING.md`](CONTRIBUTING.md) file.
+Want to help build *Taipy GUI*? Check out our [`CONTRIBUTING.md`](CONTRIBUTING.md) file.
 
 ## Code of conduct
 
-Want to be part of the _Taipy GUI_ community? Check out our [`CODE_OF_CONDUCT.md`](CODE_OF_CONDUCT.md) file.
+Want to be part of the *Taipy GUI* community? Check out our [`CODE_OF_CONDUCT.md`](CODE_OF_CONDUCT.md) file.
 
 ## Directory Structure
 
 - `gui`: Graphical user interface related files;
 - `src/taipy/gui`: Python source files;
 - `tests/taipy/gui`: Unit tests;
-- `tools`: Files used to document _taipy-gui_;
-- `CODE_OF_CONDUCT.md`: Code of conduct for members and contributors of _taipy-gui_;
-- `CONTRIBUTING.md`: Instructions to contribute to _taipy-gui_;
-- `INSTALLATION.md`: Instructions to install _taipy-gui_;
+- `tools`: Files used to document `taipy-gui`;
+- `CODE_OF_CONDUCT.md`: Code of conduct for members and contributors of `taipy-gui`;
+- `CONTRIBUTING.md`: Instructions to contribute to `taipy-gui`;
+- `INSTALLATION.md`: Instructions to build and install `taipy-gui`;
 - `LICENSE`: The Apache 2.0 License;
 - `MANIFEST.in`: Build configuration file;
 - `mypy.ini`: [mypy](http://mypy-lang.org/) linter configuration file;
 - `Pipfile`: File used by the Pipenv virtual environment to manage project dependencies;
 - `pyproject.toml`: Python build configuration file use for linters here;
 - `pytest.ini`: [pytest](https://pytest.org/) configuration file;
 - `README.md`: Current file;
-- `setup.py`: The setup script managing building, distributing, and installing _taipy-gui_;
+- `setup.py`: The setup script managing building, distributing, and installing `taipy-gui`;
 - `tox.ini`: Contains test scenarios to be run.
```

### Comparing `taipy-gui-2.3.0.dev6/setup.py` & `taipy-gui-3.0.0.dev0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     "python-dotenv>=0.19,<0.21",
     "pytz>=2021.3,<2022.2",
     "tzlocal>=3.0,<5.0",
     "backports.zoneinfo>=0.2.1,<0.3;python_version<'3.9'",
     "gevent>=22.10.2,<23.0",
     "gevent-websocket>=0.10.1,<0.11",
     "kthread>=0.2.3,<0.3",
-    "taipy-config==2.3.0.dev3",
+    "taipy-config==3.0.0.dev0",
     "gitignore-parser>=0.1,<0.2",
     "simple-websocket>=0.9,<1.0",
     "twisted>=22.10",
 ]
 
 test_requirements = ["pytest>=3.8"]
```

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/__init__.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 # an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
 
 """# Taipy Graphical User Interface generator
 
 The Taipy GUI package provides User Interface generation based on page templates. It can
-run a Web server that a Web browser can connect to.
+run a web server that a web browser can connect to.
 
-The pages are generated by a Web server that allows Web clients to connect, display and
+The pages are generated by a web server that allows web clients to connect, display and
 interact with the page content through visual elements.
 
 Each page can contain regular text and images, as well as Taipy controls that are
 typically linked to some value that is managed by the whole Taipy application.
 
 Here is how you can create your first Taipy User Interface:
 
@@ -49,15 +49,15 @@
       from byte buffers so the [`image`](../../gui/viselements/image.md) control can
       display them, and so that [`file_download`](../../gui/viselements/file_download.md)
       can request the browser to display the image content when relevant.<br/>
       You can install that package with the regular `pip install python-magic` command
       (then potentially `pip install python-magic` on Windows),
       or install Taipy GUI using: `pip install taipy-gui[image]`.
     - [`pyarrow`](https://pypi.org/project/pyarrow/): can improve the performance of your
-      application by reducing the volume of data transferred between the Web server and the
+      application by reducing the volume of data transferred between the web server and the
       clients. This is relevant if your application uses large tabular data.<br/>
       You can install that package with the regular `pip install pyarrow` command,
       or install Taipy GUI using: `pip install taipy-gui[arrow]`.
     - [`simple-websocket`](https://pypi.org/project/simple-websocket/): enables the
       debugging of the WebSocket part of the server execution.<br/>
       You can install that package with the regular `pip install simple-websocket` command,
       or install Taipy GUI using: `pip install taipy-gui[simple-websocket]`.
@@ -66,15 +66,15 @@
       You can install that package with the regular `pip install pyngrok` command,
       or install Taipy GUI using: `pip install taipy-gui[pyngrok]`.
 
 """
 
 from importlib.util import find_spec
 
-from .gui import Gui
+from ._init import *
 from .gui_actions import (
     download,
     get_module_context,
     get_module_name_from_state,
     get_state_id,
     get_user_content_url,
     hold_control,
```

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/_default_config.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/_default_config.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/_gui_cli.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/_gui_cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
         gui_parser.add_argument("--ngrok-token", nargs="?", default="", const="", help="Specify NGROK Authtoken")
         gui_parser.add_argument(
             "--webapp-path",
             nargs="?",
             default="",
             const="",
-            help="The path to the WebApp to be used. The default is the webapp directory under gui in the Taipy GUI package directory.",
+            help="The path to the web app to be used. The default is the webapp directory under gui in the Taipy GUI package directory.",
         )
 
         debug_group = gui_parser.add_mutually_exclusive_group()
         debug_group.add_argument("--debug", help="Turn on debug", action="store_true")
         debug_group.add_argument("--no-debug", help="Turn off debug", action="store_true")
 
         reloader_group = gui_parser.add_mutually_exclusive_group()
```

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/_gui_section.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/_gui_section.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
     def _update(self, as_dict: t.Dict[str, t.Any]):
         if self._property_list:
             as_dict = {k: v for k, v in as_dict.items() if k in self._property_list}
         self._properties.update(as_dict)
 
     @staticmethod
-    def _configure(**properties):
+    def _configure(**properties) -> "_GuiSection":
         """NOT DOCUMENTED
         Configure the Graphical User Interface.
 
         Parameters:
             **properties (dict[str, any]): Keyword arguments that configure the behavior of the `Gui^` instances.<br/>
                 Please refer to the
                 [Configuration section](../gui/configuration.md#configuring-the-gui-instance)
```

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/_page.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/_page.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/config.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/config.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/data/__init__.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/data/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/data/array_dict_data_accessor.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/data/array_dict_data_accessor.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/data/content_accessor.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/data/content_accessor.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/data/data_accessor.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/data/data_accessor.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/data/data_format.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/data/data_format.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/data/data_scope.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/data/data_scope.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,20 +55,20 @@
                 if hasattr(v, name):
                     setattr(v, name, value)
 
     def create_scope(self, id: str) -> None:
         if self.__single_client:
             return
         if id is None:
-            _warn("Empty session id, might be due to unestablished Web Socket connection.")
+            _warn("Empty session id, might be due to unestablished WebSocket connection.")
             return
         if id not in self.__scopes:
             self.__scopes[id] = SimpleNamespace()
 
     def delete_scope(self, id: str) -> None:  # pragma: no cover
         if self.__single_client:
             return
         if id is None:
-            _warn("Empty session id, might be due to unestablished Web Socket connection.")
+            _warn("Empty session id, might be due to unestablished WebSocket connection.")
             return
         if id in self.__scopes:
             del self.__scopes[id]
```

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/data/decimator/__init__.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/data/decimator/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/data/decimator/lttb.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/data/decimator/lttb.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/data/decimator/minmax.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/data/decimator/minmax.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/data/decimator/rdp.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/data/decimator/rdp.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/data/decimator/scatter_decimator.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/data/decimator/scatter_decimator.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/data/numpy_data_accessor.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/data/numpy_data_accessor.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/data/pandas_data_accessor.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/data/pandas_data_accessor.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,21 +174,21 @@
             # Create sink buffer stream
             sink = pa.BufferOutputStream()
             # Create Stream writer
             writer = pa.ipc.new_stream(sink, table.schema)
             # Write data to table
             writer.write_table(table)
             writer.close()
-            # end buffer stream
+            # End buffer stream
             buf = sink.getvalue()
-            # convert buffer to python bytes and return
+            # Convert buffer to Python bytes and return
             ret["data"] = buf.to_pybytes()
             ret["orient"] = orient
         else:
-            # workaround for python built in json encoder that does not yet support ignore_nan
+            # Workaround for Python built in JSON encoder that does not yet support ignore_nan
             ret["data"] = data.replace([np.nan], ["NaN" if handle_nan else None]).to_dict(orient=orient)  # type: ignore
         return ret
 
     def get_col_types(self, var_name: str, value: t.Any) -> t.Union[None, t.Dict[str, str]]:  # type: ignore
         if isinstance(value, _PandasDataAccessor.__types):  # type: ignore
             return {str(k): v for k, v in value.dtypes.apply(lambda x: x.name).items()}
         elif isinstance(value, list):
```

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/data/utils.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/data/utils.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/extension/__init__.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/extension/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/extension/library.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/extension/library.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/gui.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,26 +155,30 @@
             application. If there is no such function, status page content shows only the status of the
             server.<br/>
             The signature of the *on_status* callback function must be:
 
             - *state*: the `State^` instance of the caller.
 
             It must return raw and valid HTML content as a string.
-        on_user_content (Callable): The function that is called when a specific URL (generated by `get_user_content_url()^`) is requested.<br/>
-            It defaults to the `on_user_content()` global function defined in the Python
-            application. If there is no such function, those specific URL will not trigger
+        on_user_content (Callable): The function that is called when a specific URL (generated by
+            `get_user_content_url()^`) is requested.<br/>
+            This callback function must return the raw HTML content of the page to be displayed on
+            the browser.
+
+            This attribute defaults to the `on_user_content()` global function defined in the Python
+            application. If there is no such function, those specific URLs will not trigger
             anything.<br/>
             The signature of the *on_user_content* callback function must be:
 
             - *state*: the `State^` instance of the caller.
             - *path*: the path provided to the `get_user_content_url()^` to build the URL.
-            - *query_args*: An optional dictionnary as defined in the `get_user_content_url()^` call.
-
-            The *on_user_content* callback function must return the raw HTML content of the page to be displayed by the browser.
+            - *parameters*: An optional dictionary as defined in the `get_user_content_url()^` call.
 
+            The returned HTML content can therefore use both the variables stored in the *state*
+            and the parameters provided in the call to `get_user_content_url()^`.
         state (State^): **Only defined when running in an IPython notebook context.**<br/>
             The unique instance of `State^` that you can use to change bound variables
             directly, potentially impacting the user interface in real-time.
 
     !!! note
         This class belongs to and is documented in the `taipy.gui` package but it is
         accessible from the top `taipy` package to simplify its access, allowing to
@@ -250,16 +254,16 @@
             path_mapping (Optional[dict]): A dictionary that associates a URL prefix to
                 a path in the server file system.<br/>
                 If the assets of your application are located in _/home/me/app_assets_ and
                 you want to access them using only '_assets_' in your application, you can
                 set _path_mapping={"assets": "/home/me/app_assets"}_. If your application
                 then requests the file _"/assets/images/logo.png"_, the server searches
                 for the file  _"/home/me/app_assets/images/logo.png"_.<br/>
-                If empty or not defined, access through the browser to all resources under the directory of the main python file
-                is allowed.
+                If empty or not defined, access through the browser to all resources under the directory
+                of the main Python file is allowed.
             env_filename (Optional[str]): An optional file from which to load application
                 configuration variables (see the
                 [Configuration](../gui/configuration.md#configuring-the-gui-instance) section
                 of the User Manual for details.)<br/>
                 The default value is "taipy.gui.env"
             libraries (Optional[List[ElementLibrary]]): An optional list of extension library
                 instances that pages can reference.<br/>
@@ -354,17 +358,17 @@
         """Add a custom visual element library.
 
         This application will be able to use custom visual elements defined in this library.
 
         Arguments:
             library: The custom visual element library to add to this application.
 
-        Multiple libraries with the same name can be added. This allows to split multiple custom visual elements
-        in several `ElementLibrary^` instances, but still refer to these elements with the same prefix in the page
-        definitions.
+        Multiple libraries with the same name can be added. This allows to split multiple custom visual
+        elements in several `ElementLibrary^` instances, but still refer to these elements with the same
+        prefix in the page definitions.
         """
         if isinstance(library, ElementLibrary):
             _Factory.set_library(library)
             library_name = library.get_name()
             if library_name.isidentifier():
                 libs = Gui.__extensions.get(library_name)
                 if libs is None:
@@ -874,36 +878,36 @@
                 self._server._ws.emit(
                     "message",
                     payload,
                     to=self.__get_ws_receiver(),
                 )
                 time.sleep(0.001)
             except Exception as e:  # pragma: no cover
-                _warn(f"Exception raised in Web Socket communication in '{self.__frame.f_code.co_name}':\n{e}")
+                _warn(f"Exception raised in WebSocket communication in '{self.__frame.f_code.co_name}':\n{e}")
         else:
             grouping_message.append(payload)
 
     def __broadcast_ws(self, payload: dict):
         try:
             self._server._ws.emit(
                 "message",
                 payload,
             )
             time.sleep(0.001)
         except Exception as e:  # pragma: no cover
-            _warn(f"Exception raised in Web Socket communication in '{self.__frame.f_code.co_name}':\n{e}")
+            _warn(f"Exception raised in WebSocket communication in '{self.__frame.f_code.co_name}':\n{e}")
 
     def __send_ack(self, ack_id: t.Optional[str]) -> None:
         if ack_id:
             try:
                 self._server._ws.emit("message", {"type": _WsType.ACKNOWLEDGEMENT.value, "id": ack_id})
                 time.sleep(0.001)
             except Exception as e:  # pragma: no cover
                 _warn(
-                    f"Exception raised in Web Socket communication (send ack) in '{self.__frame.f_code.co_name}':\n{e}"
+                    f"Exception raised in WebSocket communication (send ack) in '{self.__frame.f_code.co_name}':\n{e}"
                 )
 
     def _send_ws_id(self, id: str) -> None:
         self.__send_ws(
             {
                 "type": _WsType.CLIENT_ID.value,
                 "id": id,
@@ -1336,45 +1340,45 @@
         if name == Gui.__root_page_name:
             self._config.root_page = new_page
         # Update locals context
         self.__locals_context.add(page._get_module_name(), page._get_locals())
         # Update variable directory
         self.__var_dir.add_frame(page._frame)
 
-    def add_pages(self, pages: t.Optional[t.Union[t.Dict[str, t.Union[str, Page]], str]] = None) -> None:
+    def add_pages(self, pages: t.Optional[t.Union[t.Mapping[str, t.Union[str, Page]], str]] = None) -> None:
         """Add several pages to the Graphical User Interface.
 
         Arguments:
             pages (Union[dict[str, Union[str, Page^]], str]): The pages to add.<br/>
-                If _pages_ is a dictionnary, a page is added to this `Gui` instance
-                for each of the entries in _pages_:
+                If *pages* is a dictionary, a page is added to this `Gui` instance
+                for each of the entries in *pages*:
 
                 - The entry key is used as the page name.
                 - The entry value is used as the page content:
                     - The value can can be an instance of `Markdown^` or `Html^`, then
                       it is used as the page definition.
                     - If entry value is a string, then:
                         - If it is set to the pathname of a readable file, the page
                           content is read as Markdown input text.
                         - If it is not, the page content is read from this string as
                           Markdown text.
 
         !!! note "Reading pages from a directory"
-            If _pages_ is a string that holds the path to a readable directory, then
+            If *pages* is a string that holds the path to a readable directory, then
             this directory is traversed, recursively, to find files that Taipy can build
             pages from.
 
             For every new directory that is traversed, a new hierarchical level
             for pages is created.
 
             For every file that is found:
 
-            - If the filename extention is _.md_, it is read as Markdown content and
+            - If the filename extension is *.md*, it is read as Markdown content and
               a new page is created with the base name of this filename.
-            - If the filename extention is _.html_, it is read as HTML content and
+            - If the filename extension is *.html*, it is read as HTML content and
               a new page is created with the base name of this filename.
 
             For example, say you have the following directory structure:
             ```
             reports
             ├── home.html
             ├── budget/
@@ -1525,19 +1529,19 @@
                 _warn(f"{name}: {func} should be a function.")
 
     def load_config(self, config: Config) -> None:
         self._config._load(config)
 
     def broadcast(self, name: str, value: t.Any):
         """
-        Send a new value for a variable to all connected clients.
+        Send the new value of a variable to all connected clients.
 
         Arguments:
             name: The name of the variable to update or create.
-            value: The value (must be serializable to json format)
+            value: The value (must be serializable to the JSON format).
         """
         self.__send_ws_broadcast(name, value)
 
     def _download(self, content: t.Any, name: t.Optional[str] = "", on_action: t.Optional[str] = ""):
         content_str = self._get_content("Gui.download", content, False)
         self.__send_ws_download(content_str, str(name), str(on_action))
 
@@ -1636,15 +1640,15 @@
                         _warn(f"on_navigate() returned an invalid page name '{nav_page}'.")
                     nav_page = page_name
             except Exception as e:  # pragma: no cover
                 if not self._call_on_exception("on_navigate", e):
                     _warn(f"Exception raised in on_navigate():\n{e}")
         page = next((page_i for page_i in self._config.pages if page_i._route == nav_page), None)
 
-        # try partials
+        # Try partials
         if page is None:
             page = self._get_partial(nav_page)
         # Make sure that there is a page instance found
         if page is None:
             return (
                 jsonify({"error": f"Page '{nav_page}' doesn't exist."}),
                 400,
@@ -1871,30 +1875,30 @@
         self,
         run_server: bool = True,
         run_in_thread: bool = False,
         async_mode: str = "gevent",
         **kwargs,
     ) -> t.Optional[Flask]:
         """
-        Starts the server that delivers pages to Web clients.
+        Start the server that delivers pages to web clients.
 
-        Once you enter `run()`, users can run Web browsers and point to the Web server
-        URL that `Gui` serves. The default is to listen to the _localhost_ address
+        Once you enter `run()`, users can run web browsers and point to the web server
+        URL that `Gui` serves. The default is to listen to the *localhost* address
         (127.0.0.1) on the port number 5000. However, the configuration of this `Gui`
         object may impact that (see the
         [Configuration](../gui/configuration.md#configuring-the-gui-instance)
         section of the User Manual for details).
 
         Arguments:
-            run_server (bool): Whether or not to run a Web server locally.
-                If set to _False_, a Web server is _not_ created and started.
-            run_in_thread (bool): Whether or not to run a Web server in a separated thread.
-                If set to _True_, the Web server is run is a separated thread.
-                Note that if you are running in an IPython notebook context, the Web
-                server is always run in a separate thread.
+            run_server (bool): Whether or not to run a web server locally.
+                If set to *False*, a web server is *not* created and started.
+            run_in_thread (bool): Whether or not to run a web server in a separated thread.
+                If set to *True*, the web server runs is a separated thread.<br/>
+                Note that if you are running in an IPython notebook context, the web
+                server always runs in a separate thread.
             async_mode (str): The asynchronous model to use for the Flask-SocketIO.
                 Valid values are:<br/>
 
                 - "gevent": Use a [gevent](https://www.gevent.org/servers.html) server.
                 - "threading": Use the Flask Development Server. This allows the application to use
                   the Flask reloader (the *use_reloader* option) and Debug mode (the *debug* option).
                 - "eventlet": Use an [*eventlet*](https://flask.palletsprojects.com/en/2.2.x/deploying/eventlet/)
@@ -1957,25 +1961,25 @@
 
         self.__var_dir.set_default(self.__frame)
 
         if self.__state is None:
             self.__state = State(self, self.__locals_context.get_all_keys(), self.__locals_context.get_all_context())
 
         if _is_in_notebook():
-            # to allow gui.state.x in notebook mode
+            # Allow gui.state.x in notebook mode
             self.state = self.__state
 
         self.__bind_default_function()
 
-        # base global ctx is TaipyHolder classes + script modules and callables
+        # Base global ctx is TaipyHolder classes + script modules and callables
         glob_ctx: t.Dict[str, t.Any] = {t.__name__: t for t in _TaipyBase.__subclasses__()}
         glob_ctx.update({k: v for k, v in locals_bind.items() if inspect.ismodule(v) or callable(v)})
         glob_ctx[Gui.__SELF_VAR] = self
 
-        # call on_init on each library
+        # Call on_init on each library
         for name, libs in self.__extensions.items():
             for lib in libs:
                 if not isinstance(lib, ElementLibrary):
                     continue
                 try:
                     lib_context = lib.on_init(self)
                     if (
@@ -1997,15 +2001,15 @@
                         _warn(f"Method {name}.on_init() raised an exception:\n{e}")
 
         # Initiate the Evaluator with the right context
         self.__evaluator = _Evaluator(glob_ctx)
 
         self.__register_blueprint()
 
-        # Register data accessor communicaiton data format (JSON, Apache Arrow)
+        # Register data accessor communication data format (JSON, Apache Arrow)
         self._accessors._set_data_format(_DataFormat.APACHE_ARROW if app_config["use_arrow"] else _DataFormat.JSON)
 
         # Use multi user or not
         self._bindings()._set_single_client(bool(app_config["single_client"]))
 
         # Start Flask Server
         if not run_server:
@@ -2020,31 +2024,31 @@
             run_in_thread=app_config["run_in_thread"],
             allow_unsafe_werkzeug=app_config["allow_unsafe_werkzeug"],
             notebook_proxy=app_config["notebook_proxy"],
         )
 
     def reload(self):  # pragma: no cover
         """
-        Reload the Web server.
+        Reload the web server.
 
-        This function reloads the underlying Web server only in the situation where
-        it was run in a separated thread: the _run_in_thread_ parameter to the
+        This function reloads the underlying web server only in the situation where
+        it was run in a separated thread: the *run_in_thread* parameter to the
         `(Gui.)run^` method was set to True, or you are running in an IPython notebook
         context.
         """
         if hasattr(self, "_server") and hasattr(self._server, "_thread") and self._server._is_running:
             self._server.stop_thread()
             self.run(**self.__run_kwargs)
             _TaipyLogger._get_logger().info("Gui server has been reloaded.")
 
     def stop(self):
         """
-        Stop the Web server.
+        Stop the web server.
 
-        This function stops the underlying Web server only in the situation where
-        it was run in a separated thread: the _run_in_thread_ parameter to the
+        This function stops the underlying web server only in the situation where
+        it was run in a separated thread: the *run_in_thread* parameter to the
         `(Gui.)run^` method was set to True, or you are running in an IPython notebook
         context.
         """
         if hasattr(self, "_server") and hasattr(self._server, "_thread") and self._server._is_running:
             self._server.stop_thread()
             _TaipyLogger._get_logger().info("Gui server has been stopped.")
```

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/gui_actions.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/gui_actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 
 def download(state: State, content: t.Any, name: t.Optional[str] = "", on_action: t.Optional[str] = ""):
     """Download content to the client.
 
     Arguments:
         state (State^): The current user state as received in any callback.
         content: File path or file content.
-        name: File name for the content on the client browser (default to content name).
-        on_action: Function called when the download starts.
+        name: File name for the content on the client browser (defaults to content name).
+        on_action: Name of the callback function to call when the download starts.
     """
     if state and isinstance(state._gui, Gui):
         state._gui._download(content, name, on_action)
     else:
         _warn("'download()' must be called in the context of a callback.")
 
 
@@ -39,30 +39,30 @@
     system_notification: t.Optional[bool] = None,
     duration: t.Optional[int] = None,
 ):
     """Send a notification to the user interface.
 
     Arguments:
         state (State^): The current user state as received in any callback.
-        notification_type: The notification type. This can be one of _"success"_, _"info"_,
-            _"warning"_, or _"error"_.<br/>
+        notification_type: The notification type. This can be one of "success", "info",
+            "warning", or "error".<br/>
             To remove the last notification, set this parameter to the empty string.
         message: The text message to display.
-        system_notification: If True, the system will also show the notification.
+        system_notification: If True, the system will also show the notification.<br/>
             If not specified or set to None, this parameter will use the value of
-            _configuration[system_notification]_.
+            *configuration[system_notification]*.
         duration: The time, in milliseconds, during which the notification is shown.
             If not specified or set to None, this parameter will use the value of
-            _configuration[notification_duration]_.
+            *configuration[notification_duration]*.
 
-    Note that you can also call this function with _notification_type_ set to the first letter
-    or the alert type (ie setting _notification_type_ to "i" is equivalent to setting it to
+    Note that you can also call this function with *notification_type* set to the first letter
+    or the alert type (i.e. setting *notification_type* to "i" is equivalent to setting it to
     "info").
 
-    If _system_notification_ is set to True, then the browser requests the system
+    If *system_notification* is set to True, then the browser requests the system
     to display a notification as well. They usually appear in small windows that
     fly out of the system tray.<br/>
     The first time your browser is requested to show such a system notification for
     Taipy applications, you may be prompted to authorize the browser to do so. Please
     refer to your browser documentation for details on how to allow or prevent this
     feature.
     """
@@ -112,41 +112,49 @@
 
 
 def navigate(state: State, to: t.Optional[str] = "", tab: t.Optional[str] = None, force: t.Optional[bool] = False):
     """Navigate to a page.
 
     Arguments:
         state (State^): The current user state as received in any callback.
-        to: The name of the page to navigate to. This can be a page identifier (as created by `Gui.add_page()^` with no leading /) or an URL.
-            If ommitted, the application navigates to the root page.
-        tab: When navigating to a page that is not a known page, the page is opened in a tab identified by this (as in [window.open](https://developer.mozilla.org/en-US/docs/Web/API/Window/open)).
-            The default value creates a new tab for the page (which is equivalent to setting tab to "_blank").
+        to: The name of the page to navigate to. This can be a page identifier (as created by
+            `Gui.add_page()^` with no leading '/') or an URL.<br/>
+            If omitted, the application navigates to the root page.
+        tab: When navigating to a page that is not a known page, the page is opened in a tab identified by
+            *tab* (as in [window.open](https://developer.mozilla.org/en-US/docs/Web/API/Window/open)).<br/>
+            The default value creates a new tab for the page (which is equivalent to setting *tab* to "_blank").
         force: When navigating to a known page, the content is refreshed even it the page is already shown.
     """
     if state and isinstance(state._gui, Gui):
         state._gui._navigate(to, tab, force)
     else:
         _warn("'navigate()' must be called in the context of a callback.")
 
 
 def get_user_content_url(
-    state: State, path: t.Optional[str] = None, query_args: t.Optional[t.Dict[str, str]] = None
+    state: State, path: t.Optional[str] = None, params: t.Optional[t.Dict[str, str]] = None
 ) -> t.Optional[str]:
     """Get a user content URL.
 
+    This function can be used if you need to deliver dynamic content to your page: you can create
+    a path at run-time that, when queried, will deliver some user-defined content defined in the
+    *on_user_content* callback (see the description of the `Gui^` class for more information).
+
     Arguments:
         state (State^): The current user state as received in any callback.
-        path: An optional additional path to the URL
-        query_args: An optional dict that will be adding to the arguments of the query string.
+        path: An optional additional path to the URL.
+        params: An optional dictionary sent to the *on_user_content* callback.<br/>
+           These arguments are added as query parameters to the generated URL and converted into
+           strings.
 
     Returns:
-        An URL that will allow the `on_user_content()^` to be fired.
+        An URL that, when queried, triggers the `on_user_content()^` callback.
     """
     if state and isinstance(state._gui, Gui):
-        return state._gui._get_user_content_url(path, query_args)
+        return state._gui._get_user_content_url(path, params)
     _warn("'get_user_content_url()' must be called in the context of a callback.")
     return None
 
 
 def get_state_id(state: State) -> t.Optional[str]:
     """Get the identifier of a state.
```

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/icon.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/icon.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/page.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/page.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,29 +18,29 @@
 from .utils import _filter_locals, _get_module_name_from_frame, _is_in_notebook, _varname_from_content
 
 
 class Page(ABC):
     """Generic page generator.
 
     The `Page` class transforms template text into actual pages that can be displayed
-    on a Web browser.
+    on a web browser.
 
     When a page is requested to be displayed, it is converted into HTML
     code that can be sent to the client. All control placeholders are
     replaced by their respective graphical component so you can show
     your application variables and interact with them.
     """
 
     def __init__(self, content: str, **kwargs) -> None:
         """Initialize a new Page with the indicated content.
 
         Arguments:
             content (str): The text content or the path to the file holding the text to be transformed.
 
-        If _content_ is a path to a readable file, the file is read entirely as the text template.
+        If *content* is a path to a readable file, the file is read entirely as the text template.
         """
         self._content = ""
         self._filepath = ""
         self._frame: t.Optional[FrameType] = None
         if "frame" in kwargs:
             self._frame = kwargs.get("frame")
         else:
@@ -48,30 +48,30 @@
             self._frame = t.cast(FrameType, t.cast(FrameType, inspect.stack()[2].frame))
         self.__process_content(content)
 
     def __process_content(self, content: str) -> None:
         if path.exists(content) and path.isfile(content):
             with open(t.cast(str, content), "r") as f:
                 self._content = f.read()
-                # save file path for error handling
+                # Save file path for error handling
                 self._filepath = content
         else:
             self._content = content
 
     def set_content(self, content: str) -> None:
         """Set a new page content.
 
         Reads the new page content and reinitializes the page to reflect the change.
 
         !!! important
             This function can only be used an IPython notebook context.
 
         Arguments:
             content (str): The text content or the path to the file holding the text to be transformed.
-                If _content_ is a path to a readable file, the file is read entirely as the text
+                If *content* is a path to a readable file, the file is read entirely as the text
                 template.
 
         Exceptions:
             RuntimeError: If this method is called outside an IPython notebook context.
         """
         if not _is_in_notebook():
             raise RuntimeError("'set_content()' must be used in an IPython notebook context")
```

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/partial.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/partial.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/renderers/__init__.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/renderers/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/renderers/_html/__init__.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/renderers/_html/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/renderers/_html/factory.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/renderers/_html/factory.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/renderers/_html/parser.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/renderers/_html/parser.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/renderers/_markdown/__init__.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/renderers/_markdown/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/renderers/_markdown/blocproc.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/renderers/_markdown/blocproc.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/renderers/_markdown/control.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/renderers/_markdown/control.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/renderers/_markdown/factory.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/renderers/_markdown/factory.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/renderers/_markdown/postproc.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/renderers/_markdown/postproc.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/renderers/_markdown/preproc.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/renderers/_markdown/preproc.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/renderers/builder.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/renderers/builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -661,29 +661,39 @@
             _warn(f"{self.__element_name}: {var_name} value is not valid ({numVal}).")
         if hash_name:
             hash_name = self.__get_typed_hash_name(hash_name, PropertyType.number)
             self.__update_vars.append(f"{var_name}={hash_name}")
             self.__set_react_attribute(var_name, hash_name)
         return self
 
-    def __set_default_value(self, var_name: str, value: t.Optional[t.Any] = None, native_type: bool = False):
+    def __set_default_value(
+        self,
+        var_name: str,
+        value: t.Optional[t.Any] = None,
+        native_type: bool = False,
+        var_type: t.Optional[PropertyType] = None,
+    ):
         if value is None:
             value = self.__attributes.get(var_name)
         default_var_name = _to_camel_case(f"default_{var_name}")
         if isinstance(value, (datetime, date, time)):
-            self.set_attribute(default_var_name, _date_to_ISO(value))
+            return self.set_attribute(default_var_name, _date_to_ISO(value))
         elif isinstance(value, str):
-            self.set_attribute(default_var_name, value)
+            return self.set_attribute(default_var_name, value)
         elif native_type and isinstance(value, numbers.Number):
-            self.__set_react_attribute(default_var_name, value)
+            return self.__set_react_attribute(default_var_name, value)
         elif value is None:
-            self.__set_react_attribute(default_var_name, "null")
+            return self.__set_react_attribute(default_var_name, "null")
+        elif var_type == PropertyType.lov_value:
+            # Done by _get_adapter
+            return self
+        elif isclass(var_type) and issubclass(var_type, _TaipyBase):
+            return self.__set_default_value(var_name, t.cast(t.Callable, var_type)(value, "").get())
         else:
-            self.__set_json_attribute(default_var_name, value)
-        return self
+            return self.__set_json_attribute(default_var_name, value)
 
     def __set_update_var_name(self, hash_name: str):
         return self.set_attribute("updateVarName", hash_name)
 
     def set_value_and_default(
         self,
         var_name: t.Optional[str] = None,
@@ -724,15 +734,15 @@
                 if native_type:
                     val = self.__attributes.get(var_name)
                     if native_type and isinstance(val, str):
                         with contextlib.suppress(Exception):
                             val = float(val)
                     self.__set_default_value(var_name, val, native_type=native_type)
                 else:
-                    self.__set_default_value(var_name)
+                    self.__set_default_value(var_name, var_type=var_type)
         else:
             value = self.__attributes.get(var_name)
             if value is not None:
                 if native_type:
                     if isinstance(value, str):
                         with contextlib.suppress(Exception):
                             value = float(value)
```

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/renderers/factory.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/renderers/factory.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/renderers/json.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/renderers/json.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/renderers/utils.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/renderers/utils.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/server.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/server.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/state.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/state.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/types.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/types.py`

 * *Files 16% similar despite different names*

```diff
@@ -124,17 +124,43 @@
     decimator = Decimator
     """
     The property holds an inner attributes that is defined by a library and cannot be overridden by the user.
     """
     inner = "inner"
 
 
-def _get_taipy_type(a_type: t.Optional[PropertyType]) -> t.Optional[t.Type[_TaipyBase]]:
+@t.overload
+def _get_taipy_type(a_type: None) -> None:
+    ...
+
+
+@t.overload
+def _get_taipy_type(a_type: t.Type[_TaipyBase]) -> t.Type[_TaipyBase]:
+    ...
+
+
+@t.overload
+def _get_taipy_type(a_type: PropertyType) -> t.Type[_TaipyBase]:
+    ...
+
+
+@t.overload
+def _get_taipy_type(
+    a_type: t.Optional[t.Union[t.Type[_TaipyBase], t.Type[Decimator], PropertyType]]
+) -> t.Optional[t.Union[t.Type[_TaipyBase], t.Type[Decimator], PropertyType]]:
+    ...
+
+
+def _get_taipy_type(
+    a_type: t.Optional[t.Union[t.Type[_TaipyBase], t.Type[Decimator], PropertyType]]
+) -> t.Optional[t.Union[t.Type[_TaipyBase], t.Type[Decimator], PropertyType]]:
+    if a_type is None:
+        return None
     if isinstance(a_type, PropertyType) and not isinstance(a_type.value, str):
         return a_type.value
-    if isclass(a_type) and issubclass(a_type, _TaipyBase):
+    if isclass(a_type) and not isinstance(a_type, PropertyType) and issubclass(a_type, _TaipyBase):
         return a_type
     if a_type == PropertyType.boolean:
         return _TaipyBool
     elif a_type == PropertyType.number:
         return _TaipyNumber
     return None
```

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/utils/__init__.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/utils/_adapter.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/utils/_adapter.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/utils/_attributes.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/utils/_attributes.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/utils/_bindings.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/utils/_bindings.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/utils/_evaluator.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/utils/_evaluator.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/utils/_locals_context.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/utils/_locals_context.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/utils/_map_dict.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/utils/_map_dict.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/utils/_runtime_manager.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/utils/_runtime_manager.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/utils/_variable_directory.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/utils/_variable_directory.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/utils/boolean.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/utils/boolean.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/utils/chart_config_builder.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/utils/chart_config_builder.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/utils/clientvarname.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/utils/clientvarname.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/utils/datatype.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/utils/datatype.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/utils/date.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/utils/date.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/utils/expr_var_name.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/utils/expr_var_name.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/utils/filename.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/utils/filename.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/utils/filter_locals.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/utils/filter_locals.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/utils/get_imported_var.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/utils/get_imported_var.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/utils/get_module_name.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/utils/get_module_name.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/utils/getdatecolstrname.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/utils/getdatecolstrname.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/utils/html.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/utils/html.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/utils/is_debugging.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/utils/is_debugging.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/utils/isnotebook.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/utils/isnotebook.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/utils/proxy.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/utils/proxy.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/utils/singleton.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/utils/table_col_builder.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/utils/table_col_builder.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/utils/types.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/utils/types.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/utils/varnamefromcontent.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/utils/varnamefromcontent.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/viselements.json` & `taipy-gui-3.0.0.dev0/src/taipy/gui/viselements.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999964629315223%*

 * *Differences: {"'controls'": "{16: {1: {'properties': {0: {'type': 'dynamic(any)'}}}}}"}*

```diff
@@ -1075,15 +1075,15 @@
                 ],
                 "properties": [
                     {
                         "default_property": true,
                         "doc": "The data to be represented in this table.",
                         "name": "data",
                         "required": true,
-                        "type": "any"
+                        "type": "dynamic(any)"
                     },
                     {
                         "default_value": "100",
                         "doc": "For a paginated table, the number of visible rows.",
                         "name": "page_size",
                         "type": "int"
                     },
```

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/227.taipy-gui.js` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/227.taipy-gui.js`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/499.taipy-gui.js` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/499.taipy-gui.js`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/660.taipy-gui.js` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/660.taipy-gui.js`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/660.taipy-gui.js.LICENSE.txt` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/660.taipy-gui.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/favicon.ico` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/favicon.ico`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/favicon.png` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/favicon.png`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/index.html` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/index.html`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/base/base.css` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/base/base.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/base/fontfaces.css` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/base/fontfaces.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/base/typography.css` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/base/typography.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/blocks/layout.css` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/blocks/layout.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/controls/button.css` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/controls/button.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/controls/chart.css` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/controls/chart.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/controls/date.css` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/controls/date.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/controls/expandable.css` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/controls/expandable.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/controls/image.css` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/controls/image.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/controls/input.css` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/controls/input.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/controls/navbar.css` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/controls/navbar.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/controls/number.css` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/controls/number.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/controls/selector.css` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/controls/selector.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/controls/slider.css` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/controls/slider.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/controls/table.css` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/controls/table.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/controls/toggle.css` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/controls/toggle.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/elements/card.css` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/elements/card.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/elements/container.css` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/elements/container.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/elements/header.css` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/elements/header.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/elements/sidebar.css` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/elements/sidebar.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/stylekit.css` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/stylekit.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/utilities/colors.css` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/utilities/colors.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/utilities/misc.css` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/utilities/misc.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/utilities/spacing.css` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/utilities/spacing.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/utilities/typography.css` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/utilities/typography.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/variables/colors.css` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/variables/colors.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/variables/elements.css` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/variables/elements.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/variables/misc.css` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/variables/misc.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/variables/shapes.css` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/variables/shapes.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/variables/spacing.css` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/variables/spacing.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/stylekit/variables/typography.css` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/variables/typography.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/taipy-gui-deps-manifest.json` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/taipy-gui-deps-manifest.json`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/taipy-gui-deps.dll.js` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/taipy-gui-deps.dll.js`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/taipy-gui-deps.dll.js.LICENSE.txt` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/taipy-gui-deps.dll.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/taipy-gui-dom.js` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/taipy-gui-dom.js`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/taipy-gui.d.ts` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/taipy-gui.d.ts`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/taipy-gui.js` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/taipy-gui.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -21149,15 +21149,15 @@
                     R = (0, n.useMemo)((() => {
                         let t = {};
                         if (e.plotConfig) {
                             try {
                                 t = JSON.parse(e.plotConfig)
                             } catch (e) {
                                 console.info(`Error while parsing Chart.plot_config\n${e.message||e}`)
-                            }("object" != typeof t || null === t || Array.isArray(t)) && (console.info("Error Chart.plot_config is not a dictionnary"), t = {})
+                            }("object" != typeof t || null === t || Array.isArray(t)) && (console.info("Error Chart.plot_config is not a dictionary"), t = {})
                         }
                         return k ? t : Object.assign(Object.assign({}, t), {
                             staticPlot: !0
                         })
                     }), [k, e.plotConfig]),
                     A = (0, n.useCallback)((e => {
                         if (Object.keys(e).some((e => e.startsWith("xaxis."))) && (u && p(Ts(l, y, Object.assign({
```

### Comparing `taipy-gui-2.3.0.dev6/src/taipy/gui/webapp/taipy-gui.js.LICENSE.txt` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/taipy-gui.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.3.0.dev6/src/taipy_gui.egg-info/PKG-INFO` & `taipy-gui-3.0.0.dev0/src/taipy_gui.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipy-gui
-Version: 2.3.0.dev6
+Version: 3.0.0.dev0
 Summary: Low-code library to create graphical user interfaces on the Web for your Python applications.
 Home-page: https://github.com/avaiga/taipy-gui
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy-gui
 Classifier: Intended Audience :: Developers
@@ -43,44 +43,44 @@
 - [Contributing](#contributing)
 - [Code of conduct](#code-of-conduct)
 - [Directory Structure](#directory-structure)
 
 ## What is Taipy GUI
 
 Taipy is a Python library for creating Business Applications. More information on our
-[website](https://www.taipy.io). Taipy is split into multiple repositories including _taipy-gui_ to let users
+[website](https://www.taipy.io). Taipy is split into multiple repositories including `taipy-gui` to let users
 install the minimum they need.
 
-[Taipy GUI](https://github.com/Avaiga/taipy-gui) provides Python classes that make it easy to create powerful Web apps in minutes.
+[Taipy GUI](https://github.com/Avaiga/taipy-gui) provides Python classes that make it easy to create powerful web apps in minutes.
 
-A more in depth documentation of taipy can be found [here](https://docs.taipy.io/).
+A more in depth documentation of Taipy can be found [here](https://docs.taipy.io/).
 
 ## Installation
 
-Want to install and try _Taipy GUI_? Check out our [`INSTALLATION.md`](INSTALLATION.md) file.
+Want to install and try *Taipy GUI*? Check out our [`INSTALLATION.md`](INSTALLATION.md) file.
 
 ## Contributing
 
-Want to help build _Taipy GUI_? Check out our [`CONTRIBUTING.md`](CONTRIBUTING.md) file.
+Want to help build *Taipy GUI*? Check out our [`CONTRIBUTING.md`](CONTRIBUTING.md) file.
 
 ## Code of conduct
 
-Want to be part of the _Taipy GUI_ community? Check out our [`CODE_OF_CONDUCT.md`](CODE_OF_CONDUCT.md) file.
+Want to be part of the *Taipy GUI* community? Check out our [`CODE_OF_CONDUCT.md`](CODE_OF_CONDUCT.md) file.
 
 ## Directory Structure
 
 - `gui`: Graphical user interface related files;
 - `src/taipy/gui`: Python source files;
 - `tests/taipy/gui`: Unit tests;
-- `tools`: Files used to document _taipy-gui_;
-- `CODE_OF_CONDUCT.md`: Code of conduct for members and contributors of _taipy-gui_;
-- `CONTRIBUTING.md`: Instructions to contribute to _taipy-gui_;
-- `INSTALLATION.md`: Instructions to install _taipy-gui_;
+- `tools`: Files used to document `taipy-gui`;
+- `CODE_OF_CONDUCT.md`: Code of conduct for members and contributors of `taipy-gui`;
+- `CONTRIBUTING.md`: Instructions to contribute to `taipy-gui`;
+- `INSTALLATION.md`: Instructions to build and install `taipy-gui`;
 - `LICENSE`: The Apache 2.0 License;
 - `MANIFEST.in`: Build configuration file;
 - `mypy.ini`: [mypy](http://mypy-lang.org/) linter configuration file;
 - `Pipfile`: File used by the Pipenv virtual environment to manage project dependencies;
 - `pyproject.toml`: Python build configuration file use for linters here;
 - `pytest.ini`: [pytest](https://pytest.org/) configuration file;
 - `README.md`: Current file;
-- `setup.py`: The setup script managing building, distributing, and installing _taipy-gui_;
+- `setup.py`: The setup script managing building, distributing, and installing `taipy-gui`;
 - `tox.ini`: Contains test scenarios to be run.
```

### Comparing `taipy-gui-2.3.0.dev6/src/taipy_gui.egg-info/SOURCES.txt` & `taipy-gui-3.0.0.dev0/src/taipy_gui.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 pyproject.toml
 setup.py
 src/taipy/__init__.py
 src/taipy/gui/__init__.py
 src/taipy/gui/_default_config.py
 src/taipy/gui/_gui_cli.py
 src/taipy/gui/_gui_section.py
+src/taipy/gui/_init.py
 src/taipy/gui/_page.py
 src/taipy/gui/_warnings.py
 src/taipy/gui/config.py
 src/taipy/gui/gui.py
 src/taipy/gui/gui_actions.py
 src/taipy/gui/icon.py
 src/taipy/gui/page.py
```

### Comparing `taipy-gui-2.3.0.dev6/src/taipy_gui.egg-info/requires.txt` & `taipy-gui-3.0.0.dev0/src/taipy_gui.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 pandas<2.0,>=1.5.1
 python-dotenv<0.21,>=0.19
 pytz<2022.2,>=2021.3
 tzlocal<5.0,>=3.0
 gevent<23.0,>=22.10.2
 gevent-websocket<0.11,>=0.10.1
 kthread<0.3,>=0.2.3
-taipy-config==2.3.0.dev3
+taipy-config==3.0.0.dev0
 gitignore-parser<0.2,>=0.1
 simple-websocket<1.0,>=0.9
 twisted>=22.10
 
 [:python_version < "3.9"]
 backports.zoneinfo<0.3,>=0.2.1
```

