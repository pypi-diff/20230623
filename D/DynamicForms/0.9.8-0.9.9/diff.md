# Comparing `tmp/DynamicForms-0.9.8.tar.gz` & `tmp/DynamicForms-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/DynamicForms-0.9.8.tar", last modified: Tue Mar 24 09:30:13 2020, max compression
+gzip compressed data, was "dist/DynamicForms-0.9.9.tar", last modified: Fri Apr 17 08:04:14 2020, max compression
```

## Comparing `DynamicForms-0.9.8.tar` & `DynamicForms-0.9.9.tar`

### file list

```diff
@@ -1,228 +1,236 @@
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2020-03-24 09:30:13.000000 DynamicForms-0.9.8/
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2020-03-24 09:30:13.000000 DynamicForms-0.9.8/DynamicForms.egg-info/
--rw-r--r--   0 jure      (1000) jure      (1000)     8173 2020-03-24 09:30:13.000000 DynamicForms-0.9.8/DynamicForms.egg-info/PKG-INFO
--rw-r--r--   0 jure      (1000) jure      (1000)    11296 2020-03-24 09:30:13.000000 DynamicForms-0.9.8/DynamicForms.egg-info/SOURCES.txt
--rw-r--r--   0 jure      (1000) jure      (1000)        1 2020-03-24 09:30:13.000000 DynamicForms-0.9.8/DynamicForms.egg-info/dependency_links.txt
--rw-r--r--   0 jure      (1000) jure      (1000)      107 2020-03-24 09:30:13.000000 DynamicForms-0.9.8/DynamicForms.egg-info/requires.txt
--rw-r--r--   0 jure      (1000) jure      (1000)       13 2020-03-24 09:30:13.000000 DynamicForms-0.9.8/DynamicForms.egg-info/top_level.txt
--rw-rw-r--   0 jure      (1000) jure      (1000)     1499 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/LICENSE.rst
--rw-rw-r--   0 jure      (1000) jure      (1000)      189 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/MANIFEST.in
--rw-r--r--   0 jure      (1000) jure      (1000)     8173 2020-03-24 09:30:13.000000 DynamicForms-0.9.8/PKG-INFO
--rw-rw-r--   0 jure      (1000) jure      (1000)     5868 2020-01-23 08:59:43.000000 DynamicForms-0.9.8/README.rst
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2020-03-24 09:30:13.000000 DynamicForms-0.9.8/dynamicforms/
--rw-rw-r--   0 jure      (1000) jure      (1000)      228 2020-03-24 09:29:47.000000 DynamicForms-0.9.8/dynamicforms/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)    20638 2020-03-03 07:27:29.000000 DynamicForms-0.9.8/dynamicforms/action.py
--rw-rw-r--   0 jure      (1000) jure      (1000)       99 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/apps.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1002 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/context_processors.py
--rw-r--r--   0 jure      (1000) jure      (1000)     1561 2020-02-25 12:32:14.000000 DynamicForms-0.9.8/dynamicforms/dynamicforms_migration_mixin.py
--rw-r--r--   0 jure      (1000) jure      (1000)    28721 2020-03-24 09:28:35.000000 DynamicForms-0.9.8/dynamicforms/fields.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2020-03-24 09:30:13.000000 DynamicForms-0.9.8/dynamicforms/migrations/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/migrations/__init__.py
--rw-r--r--   0 jure      (1000) jure      (1000)    12549 2020-03-24 09:28:22.000000 DynamicForms-0.9.8/dynamicforms/mixins.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      110 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/models.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1885 2019-07-26 10:41:59.000000 DynamicForms-0.9.8/dynamicforms/progress.py
--rw-r--r--   0 jure      (1000) jure      (1000)     6766 2020-02-20 09:31:54.000000 DynamicForms-0.9.8/dynamicforms/renderers.py
--rw-rw-r--   0 jure      (1000) jure      (1000)    10271 2020-03-04 09:59:35.000000 DynamicForms-0.9.8/dynamicforms/serializers.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     6935 2020-02-25 08:08:58.000000 DynamicForms-0.9.8/dynamicforms/settings.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2020-03-24 09:30:13.000000 DynamicForms-0.9.8/dynamicforms/static/
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2020-03-24 09:30:13.000000 DynamicForms-0.9.8/dynamicforms/static/bootstrap-3.4.1-dist/
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2020-03-24 09:30:13.000000 DynamicForms-0.9.8/dynamicforms/static/bootstrap-3.4.1-dist/css/
--rw-rw-r--   0 jure      (1000) jure      (1000)    25682 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/bootstrap-3.4.1-dist/css/bootstrap-theme.css
--rw-rw-r--   0 jure      (1000) jure      (1000)    48005 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/bootstrap-3.4.1-dist/css/bootstrap-theme.css.map
--rw-rw-r--   0 jure      (1000) jure      (1000)    23411 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/bootstrap-3.4.1-dist/css/bootstrap-theme.min.css
--rw-rw-r--   0 jure      (1000) jure      (1000)    75600 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/bootstrap-3.4.1-dist/css/bootstrap-theme.min.css.map
--rw-rw-r--   0 jure      (1000) jure      (1000)   145933 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/bootstrap-3.4.1-dist/css/bootstrap.css
--rw-rw-r--   0 jure      (1000) jure      (1000)   390887 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/bootstrap-3.4.1-dist/css/bootstrap.css.map
--rw-rw-r--   0 jure      (1000) jure      (1000)   121457 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/bootstrap-3.4.1-dist/css/bootstrap.min.css
--rw-rw-r--   0 jure      (1000) jure      (1000)   540434 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/bootstrap-3.4.1-dist/css/bootstrap.min.css.map
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2020-03-24 09:30:13.000000 DynamicForms-0.9.8/dynamicforms/static/bootstrap-3.4.1-dist/fonts/
--rw-rw-r--   0 jure      (1000) jure      (1000)    20127 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/bootstrap-3.4.1-dist/fonts/glyphicons-halflings-regular.eot
--rw-rw-r--   0 jure      (1000) jure      (1000)   108738 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/bootstrap-3.4.1-dist/fonts/glyphicons-halflings-regular.svg
--rw-rw-r--   0 jure      (1000) jure      (1000)    45404 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/bootstrap-3.4.1-dist/fonts/glyphicons-halflings-regular.ttf
--rw-rw-r--   0 jure      (1000) jure      (1000)    23424 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/bootstrap-3.4.1-dist/fonts/glyphicons-halflings-regular.woff
--rw-rw-r--   0 jure      (1000) jure      (1000)    18028 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/bootstrap-3.4.1-dist/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2020-03-24 09:30:13.000000 DynamicForms-0.9.8/dynamicforms/static/bootstrap-3.4.1-dist/js/
--rw-rw-r--   0 jure      (1000) jure      (1000)    75484 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/bootstrap-3.4.1-dist/js/bootstrap.js
--rw-rw-r--   0 jure      (1000) jure      (1000)    39680 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/bootstrap-3.4.1-dist/js/bootstrap.min.js
--rw-rw-r--   0 jure      (1000) jure      (1000)      484 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/bootstrap-3.4.1-dist/js/npm.js
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2020-03-24 09:30:13.000000 DynamicForms-0.9.8/dynamicforms/static/bootstrap-4.3.1-dist/
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2020-03-24 09:30:13.000000 DynamicForms-0.9.8/dynamicforms/static/bootstrap-4.3.1-dist/css/
--rw-rw-r--   0 jure      (1000) jure      (1000)    64548 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/bootstrap-4.3.1-dist/css/bootstrap-grid.css
--rw-rw-r--   0 jure      (1000) jure      (1000)   151749 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/bootstrap-4.3.1-dist/css/bootstrap-grid.css.map
--rw-rw-r--   0 jure      (1000) jure      (1000)    48488 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/bootstrap-4.3.1-dist/css/bootstrap-grid.min.css
--rw-rw-r--   0 jure      (1000) jure      (1000)   108539 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/bootstrap-4.3.1-dist/css/bootstrap-grid.min.css.map
--rw-rw-r--   0 jure      (1000) jure      (1000)     4897 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/bootstrap-4.3.1-dist/css/bootstrap-reboot.css
--rw-rw-r--   0 jure      (1000) jure      (1000)    76483 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/bootstrap-4.3.1-dist/css/bootstrap-reboot.css.map
--rw-rw-r--   0 jure      (1000) jure      (1000)     4021 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/bootstrap-4.3.1-dist/css/bootstrap-reboot.min.css
--rw-rw-r--   0 jure      (1000) jure      (1000)    32461 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/bootstrap-4.3.1-dist/css/bootstrap-reboot.min.css.map
--rw-rw-r--   0 jure      (1000) jure      (1000)   192348 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/bootstrap-4.3.1-dist/css/bootstrap.css
--rw-rw-r--   0 jure      (1000) jure      (1000)   492048 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/bootstrap-4.3.1-dist/css/bootstrap.css.map
--rw-rw-r--   0 jure      (1000) jure      (1000)   155758 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/bootstrap-4.3.1-dist/css/bootstrap.min.css
--rw-rw-r--   0 jure      (1000) jure      (1000)   625953 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/bootstrap-4.3.1-dist/css/bootstrap.min.css.map
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2020-03-24 09:30:13.000000 DynamicForms-0.9.8/dynamicforms/static/bootstrap-4.3.1-dist/js/
--rw-rw-r--   0 jure      (1000) jure      (1000)   222911 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/bootstrap-4.3.1-dist/js/bootstrap.bundle.js
--rw-rw-r--   0 jure      (1000) jure      (1000)   402249 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/bootstrap-4.3.1-dist/js/bootstrap.bundle.js.map
--rw-rw-r--   0 jure      (1000) jure      (1000)    78635 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/bootstrap-4.3.1-dist/js/bootstrap.bundle.min.js
--rw-rw-r--   0 jure      (1000) jure      (1000)   311949 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/bootstrap-4.3.1-dist/js/bootstrap.bundle.min.js.map
--rw-rw-r--   0 jure      (1000) jure      (1000)   131637 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/bootstrap-4.3.1-dist/js/bootstrap.js
--rw-rw-r--   0 jure      (1000) jure      (1000)   250568 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/bootstrap-4.3.1-dist/js/bootstrap.js.map
--rw-rw-r--   0 jure      (1000) jure      (1000)    58072 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/bootstrap-4.3.1-dist/js/bootstrap.min.js
--rw-rw-r--   0 jure      (1000) jure      (1000)   190253 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/bootstrap-4.3.1-dist/js/bootstrap.min.js.map
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2020-03-24 09:30:13.000000 DynamicForms-0.9.8/dynamicforms/static/dynamicforms/
--rw-rw-r--   0 jure      (1000) jure      (1000)    51604 2020-01-23 08:59:43.000000 DynamicForms-0.9.8/dynamicforms/static/dynamicforms/dynamicforms.js
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2020-03-24 09:30:13.000000 DynamicForms-0.9.8/dynamicforms/static/jquery_ui/
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2020-03-24 09:30:13.000000 DynamicForms-0.9.8/dynamicforms/static/jquery_ui/css/
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2020-03-24 09:30:13.000000 DynamicForms-0.9.8/dynamicforms/static/jquery_ui/css/images/
--rw-rw-r--   0 jure      (1000) jure      (1000)      418 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/jquery_ui/css/images/ui-bg_diagonals-thick_18_b81900_40x40.png
--rw-rw-r--   0 jure      (1000) jure      (1000)      312 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/jquery_ui/css/images/ui-bg_diagonals-thick_20_666666_40x40.png
--rw-rw-r--   0 jure      (1000) jure      (1000)      262 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/jquery_ui/css/images/ui-bg_glass_100_f6f6f6_1x400.png
--rw-rw-r--   0 jure      (1000) jure      (1000)      348 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/jquery_ui/css/images/ui-bg_glass_100_fdf5ce_1x400.png
--rw-rw-r--   0 jure      (1000) jure      (1000)      207 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/jquery_ui/css/images/ui-bg_glass_65_ffffff_1x400.png
--rw-rw-r--   0 jure      (1000) jure      (1000)     5815 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/jquery_ui/css/images/ui-bg_gloss-wave_35_f6a828_500x100.png
--rw-rw-r--   0 jure      (1000) jure      (1000)      278 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/jquery_ui/css/images/ui-bg_highlight-soft_100_eeeeee_1x100.png
--rw-rw-r--   0 jure      (1000) jure      (1000)      328 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/jquery_ui/css/images/ui-bg_highlight-soft_75_ffe45c_1x100.png
--rw-rw-r--   0 jure      (1000) jure      (1000)     6922 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/jquery_ui/css/images/ui-icons_222222_256x240.png
--rw-rw-r--   0 jure      (1000) jure      (1000)     4549 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/jquery_ui/css/images/ui-icons_228ef1_256x240.png
--rw-rw-r--   0 jure      (1000) jure      (1000)     4549 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/jquery_ui/css/images/ui-icons_ef8c08_256x240.png
--rw-rw-r--   0 jure      (1000) jure      (1000)     4549 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/jquery_ui/css/images/ui-icons_ffd27a_256x240.png
--rw-rw-r--   0 jure      (1000) jure      (1000)     6299 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/jquery_ui/css/images/ui-icons_ffffff_256x240.png
--rw-rw-r--   0 jure      (1000) jure      (1000)    31583 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/jquery_ui/css/jquery-ui.min.css
--rw-rw-r--   0 jure      (1000) jure      (1000)    15548 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/jquery_ui/css/jquery-ui.structure.min.css
--rw-rw-r--   0 jure      (1000) jure      (1000)    14436 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/jquery_ui/css/jquery-ui.theme.min.css
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2020-03-24 09:30:13.000000 DynamicForms-0.9.8/dynamicforms/static/jquery_ui/js/
--rw-rw-r--   0 jure      (1000) jure      (1000)    86927 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/jquery_ui/js/jquery-3.3.1.min.js
--rw-rw-r--   0 jure      (1000) jure      (1000)   253669 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/jquery_ui/js/jquery-ui.min.js
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2020-03-24 09:30:13.000000 DynamicForms-0.9.8/dynamicforms/static/select2/
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2020-03-24 09:30:13.000000 DynamicForms-0.9.8/dynamicforms/static/select2/css/
--rw-rw-r--   0 jure      (1000) jure      (1000)    16792 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/select2/css/select2-bootstrap3.min.css
--rw-rw-r--   0 jure      (1000) jure      (1000)    19533 2019-05-31 14:28:35.000000 DynamicForms-0.9.8/dynamicforms/static/select2/css/select2-bootstrap4.min.css
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2020-03-24 09:30:13.000000 DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2020-03-24 09:30:13.000000 DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/css/
--rw-rw-r--   0 jure      (1000) jure      (1000)    15196 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/css/select2.min.css
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2020-03-24 09:30:13.000000 DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2020-03-24 09:30:13.000000 DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/
--rw-rw-r--   0 jure      (1000) jure      (1000)      846 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/af.js
--rw-rw-r--   0 jure      (1000) jure      (1000)      868 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/ar.js
--rw-rw-r--   0 jure      (1000) jure      (1000)      701 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/az.js
--rw-rw-r--   0 jure      (1000) jure      (1000)      906 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/bg.js
--rw-rw-r--   0 jure      (1000) jure      (1000)      940 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/bs.js
--rw-rw-r--   0 jure      (1000) jure      (1000)      876 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/ca.js
--rw-rw-r--   0 jure      (1000) jure      (1000)     1252 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/cs.js
--rw-rw-r--   0 jure      (1000) jure      (1000)      808 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/da.js
--rw-rw-r--   0 jure      (1000) jure      (1000)      853 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/de.js
--rw-rw-r--   0 jure      (1000) jure      (1000)     1015 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/dsb.js
--rw-rw-r--   0 jure      (1000) jure      (1000)     1132 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/el.js
--rw-rw-r--   0 jure      (1000) jure      (1000)      827 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/en.js
--rw-rw-r--   0 jure      (1000) jure      (1000)      892 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/es.js
--rw-rw-r--   0 jure      (1000) jure      (1000)      775 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/et.js
--rw-rw-r--   0 jure      (1000) jure      (1000)      844 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/eu.js
--rw-rw-r--   0 jure      (1000) jure      (1000)     1004 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/fa.js
--rw-rw-r--   0 jure      (1000) jure      (1000)      782 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/fi.js
--rw-rw-r--   0 jure      (1000) jure      (1000)      883 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/fr.js
--rw-rw-r--   0 jure      (1000) jure      (1000)      886 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/gl.js
--rw-rw-r--   0 jure      (1000) jure      (1000)      951 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/he.js
--rw-rw-r--   0 jure      (1000) jure      (1000)     1125 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/hi.js
--rw-rw-r--   0 jure      (1000) jure      (1000)      839 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/hr.js
--rw-rw-r--   0 jure      (1000) jure      (1000)     1016 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/hsb.js
--rw-rw-r--   0 jure      (1000) jure      (1000)      802 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/hu.js
--rw-rw-r--   0 jure      (1000) jure      (1000)     1005 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/hy.js
--rw-rw-r--   0 jure      (1000) jure      (1000)      752 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/id.js
--rw-rw-r--   0 jure      (1000) jure      (1000)      773 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/is.js
--rw-rw-r--   0 jure      (1000) jure      (1000)      876 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/it.js
--rw-rw-r--   0 jure      (1000) jure      (1000)      848 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/ja.js
--rw-rw-r--   0 jure      (1000) jure      (1000)     1065 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/km.js
--rw-rw-r--   0 jure      (1000) jure      (1000)      854 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/ko.js
--rw-rw-r--   0 jure      (1000) jure      (1000)      913 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/lt.js
--rw-rw-r--   0 jure      (1000) jure      (1000)      872 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/lv.js
--rw-rw-r--   0 jure      (1000) jure      (1000)      979 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/mk.js
--rw-rw-r--   0 jure      (1000) jure      (1000)      791 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/ms.js
--rw-rw-r--   0 jure      (1000) jure      (1000)      775 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/nb.js
--rw-rw-r--   0 jure      (1000) jure      (1000)      896 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/nl.js
--rw-rw-r--   0 jure      (1000) jure      (1000)      925 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/pl.js
--rw-rw-r--   0 jure      (1000) jure      (1000)     1019 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/ps.js
--rw-rw-r--   0 jure      (1000) jure      (1000)      853 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/pt-BR.js
--rw-rw-r--   0 jure      (1000) jure      (1000)      859 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/pt.js
--rw-rw-r--   0 jure      (1000) jure      (1000)      910 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/ro.js
--rw-rw-r--   0 jure      (1000) jure      (1000)     1127 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/ru.js
--rw-rw-r--   0 jure      (1000) jure      (1000)     1266 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/sk.js
--rw-rw-r--   0 jure      (1000) jure      (1000)      890 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/sl.js
--rw-rw-r--   0 jure      (1000) jure      (1000)     1067 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/sr-Cyrl.js
--rw-rw-r--   0 jure      (1000) jure      (1000)      938 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/sr.js
--rw-rw-r--   0 jure      (1000) jure      (1000)      786 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/sv.js
--rw-rw-r--   0 jure      (1000) jure      (1000)     1048 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/th.js
--rw-rw-r--   0 jure      (1000) jure      (1000)      773 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/tr.js
--rw-rw-r--   0 jure      (1000) jure      (1000)     1117 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/uk.js
--rw-rw-r--   0 jure      (1000) jure      (1000)      800 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/vi.js
--rw-rw-r--   0 jure      (1000) jure      (1000)      769 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/zh-CN.js
--rw-rw-r--   0 jure      (1000) jure      (1000)      708 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/zh-TW.js
--rw-rw-r--   0 jure      (1000) jure      (1000)   162676 2019-11-04 14:15:16.000000 DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/select2.full.js
--rw-rw-r--   0 jure      (1000) jure      (1000)    74931 2019-11-04 14:15:16.000000 DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/select2.full.min.js
--rw-rw-r--   0 jure      (1000) jure      (1000)   142778 2019-11-04 14:15:16.000000 DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/select2.js
--rw-rw-r--   0 jure      (1000) jure      (1000)    66615 2019-11-04 14:15:16.000000 DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/select2.min.js
--rw-rw-r--   0 jure      (1000) jure      (1000)     1260 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/struct.py
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2020-03-24 09:30:13.000000 DynamicForms-0.9.8/dynamicforms/templates/
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2020-03-24 09:30:13.000000 DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2020-03-24 09:30:13.000000 DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/bootstrap/
--rw-rw-r--   0 jure      (1000) jure      (1000)      327 2019-07-09 09:00:49.000000 DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/bootstrap/base.html
--rw-rw-r--   0 jure      (1000) jure      (1000)     1411 2019-11-15 08:08:56.000000 DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/bootstrap/base_form.html
--rw-rw-r--   0 jure      (1000) jure      (1000)      257 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/bootstrap/base_includes_select2.html
--rw-rw-r--   0 jure      (1000) jure      (1000)     2374 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/bootstrap/base_includes_v3.html
--rw-rw-r--   0 jure      (1000) jure      (1000)     1519 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/bootstrap/base_includes_v4.html
--rw-rw-r--   0 jure      (1000) jure      (1000)     1957 2019-07-09 09:00:49.000000 DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/bootstrap/base_list.html
--rw-rw-r--   0 jure      (1000) jure      (1000)     1497 2019-06-28 12:42:14.000000 DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/bootstrap/base_table_body.html
--rw-rw-r--   0 jure      (1000) jure      (1000)     1190 2019-12-06 13:40:15.000000 DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/bootstrap/base_table_filter.html
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2020-03-24 09:30:13.000000 DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/bootstrap/field/
--rw-rw-r--   0 jure      (1000) jure      (1000)     2184 2019-05-22 07:53:00.000000 DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/bootstrap/field/base_field_v3.html
--rw-rw-r--   0 jure      (1000) jure      (1000)     2191 2019-05-22 07:53:00.000000 DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/bootstrap/field/base_field_v4.html
--rw-rw-r--   0 jure      (1000) jure      (1000)      674 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/bootstrap/field/checkbox.html
--rw-rw-r--   0 jure      (1000) jure      (1000)      515 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/bootstrap/field/checkbox_multiple.html
--rw-rw-r--   0 jure      (1000) jure      (1000)      179 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/bootstrap/field/dict_field.html
--rw-rw-r--   0 jure      (1000) jure      (1000)      620 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/bootstrap/field/fieldset.html
--rw-rw-r--   0 jure      (1000) jure      (1000)      304 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/bootstrap/field/form.html
--rw-rw-r--   0 jure      (1000) jure      (1000)      788 2019-11-04 14:15:16.000000 DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/bootstrap/field/input.html
--rw-rw-r--   0 jure      (1000) jure      (1000)      172 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/bootstrap/field/list_field.html
--rw-rw-r--   0 jure      (1000) jure      (1000)      668 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/bootstrap/field/list_fieldset.html
--rw-rw-r--   0 jure      (1000) jure      (1000)      863 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/bootstrap/field/radio.html
--rw-rw-r--   0 jure      (1000) jure      (1000)     2738 2019-12-20 09:07:53.000000 DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/bootstrap/field/select.html
--rw-rw-r--   0 jure      (1000) jure      (1000)     2331 2019-12-20 09:07:53.000000 DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/bootstrap/field/select_multiple.html
--rw-rw-r--   0 jure      (1000) jure      (1000)      529 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/bootstrap/field/textarea.html
--rw-rw-r--   0 jure      (1000) jure      (1000)      987 2019-06-28 12:42:14.000000 DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/bootstrap/modal_dialog_v3.html
--rw-rw-r--   0 jure      (1000) jure      (1000)     1007 2019-06-28 12:42:14.000000 DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/bootstrap/modal_dialog_v4.html
--rw-rw-r--   0 jure      (1000) jure      (1000)      658 2019-07-09 09:00:49.000000 DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/bootstrap/page.html
--rw-rw-r--   0 jure      (1000) jure      (1000)      896 2019-07-26 11:13:36.000000 DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/bootstrap/progress_dialog.html
--rw-rw-r--   0 jure      (1000) jure      (1000)      286 2019-07-09 09:00:49.000000 DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/bootstrap/progress_dialog_style.html
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2020-03-24 09:30:13.000000 DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/jquery_ui/
--rw-rw-r--   0 jure      (1000) jure      (1000)      258 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/jquery_ui/base.html
--rw-rw-r--   0 jure      (1000) jure      (1000)     1426 2019-11-15 08:08:56.000000 DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/jquery_ui/base_form.html
--rw-r--r--   0 jure      (1000) jure      (1000)     2584 2020-02-26 13:41:06.000000 DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/jquery_ui/base_includes.html
--rw-rw-r--   0 jure      (1000) jure      (1000)     1923 2019-05-22 07:53:00.000000 DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/jquery_ui/base_list.html
--rw-rw-r--   0 jure      (1000) jure      (1000)     1479 2019-06-28 12:42:14.000000 DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/jquery_ui/base_table_body.html
--rw-rw-r--   0 jure      (1000) jure      (1000)     1197 2019-12-06 13:40:15.000000 DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/jquery_ui/base_table_filter.html
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2020-03-24 09:30:13.000000 DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/jquery_ui/field/
--rw-rw-r--   0 jure      (1000) jure      (1000)     2109 2019-05-22 07:53:00.000000 DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/jquery_ui/field/base_field.html
--rw-rw-r--   0 jure      (1000) jure      (1000)      669 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/jquery_ui/field/checkbox.html
--rw-rw-r--   0 jure      (1000) jure      (1000)      516 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/jquery_ui/field/checkbox_multiple.html
--rw-rw-r--   0 jure      (1000) jure      (1000)      179 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/jquery_ui/field/dict_field.html
--rw-rw-r--   0 jure      (1000) jure      (1000)      287 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/jquery_ui/field/fieldset.html
--rw-rw-r--   0 jure      (1000) jure      (1000)      301 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/jquery_ui/field/form.html
--rw-r--r--   0 jure      (1000) jure      (1000)      828 2020-02-25 12:32:14.000000 DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/jquery_ui/field/input.html
--rw-rw-r--   0 jure      (1000) jure      (1000)      172 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/jquery_ui/field/list_field.html
--rw-rw-r--   0 jure      (1000) jure      (1000)      195 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/jquery_ui/field/list_fieldset.html
--rw-rw-r--   0 jure      (1000) jure      (1000)      864 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/jquery_ui/field/radio.html
--rw-rw-r--   0 jure      (1000) jure      (1000)     3320 2019-12-20 09:07:53.000000 DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/jquery_ui/field/select.html
--rw-rw-r--   0 jure      (1000) jure      (1000)     2078 2019-12-20 09:07:53.000000 DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/jquery_ui/field/select_multiple.html
--rw-r--r--   0 jure      (1000) jure      (1000)      492 2020-02-25 12:32:14.000000 DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/jquery_ui/field/textarea.html
--rw-rw-r--   0 jure      (1000) jure      (1000)     1105 2019-10-15 06:32:16.000000 DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/jquery_ui/modal_dialog.html
--rw-rw-r--   0 jure      (1000) jure      (1000)      694 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/jquery_ui/page.html
--rw-rw-r--   0 jure      (1000) jure      (1000)      286 2019-07-26 10:42:57.000000 DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/jquery_ui/progress_dialog.html
--rw-rw-r--   0 jure      (1000) jure      (1000)      378 2019-07-09 09:00:49.000000 DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/jquery_ui/progress_dialog_style.html
-drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2020-03-24 09:30:13.000000 DynamicForms-0.9.8/dynamicforms/templatetags/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2019-05-14 15:53:14.000000 DynamicForms-0.9.8/dynamicforms/templatetags/__init__.py
--rw-r--r--   0 jure      (1000) jure      (1000)    10150 2020-03-24 09:28:35.000000 DynamicForms-0.9.8/dynamicforms/templatetags/dynamicforms.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      229 2020-01-23 08:59:43.000000 DynamicForms-0.9.8/dynamicforms/urls.py
--rw-rw-r--   0 jure      (1000) jure      (1000)       38 2020-01-23 08:59:43.000000 DynamicForms-0.9.8/dynamicforms/views.py
--rw-r--r--   0 jure      (1000) jure      (1000)    14879 2020-02-20 11:21:04.000000 DynamicForms-0.9.8/dynamicforms/viewsets.py
--rw-r--r--   0 jure      (1000) jure      (1000)      104 2020-03-24 09:28:35.000000 DynamicForms-0.9.8/requirements.txt
--rw-rw-r--   0 jure      (1000) jure      (1000)       25 2019-05-29 07:17:47.000000 DynamicForms-0.9.8/requirements_test_functional.txt
--rw-r--r--   0 jure      (1000) jure      (1000)       38 2020-03-24 09:30:13.000000 DynamicForms-0.9.8/setup.cfg
--rw-rw-r--   0 jure      (1000) jure      (1000)     1440 2020-03-24 09:29:47.000000 DynamicForms-0.9.8/setup.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2020-04-17 08:04:14.000000 DynamicForms-0.9.9/
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2020-04-17 08:04:14.000000 DynamicForms-0.9.9/DynamicForms.egg-info/
+-rw-r--r--   0 jure      (1000) jure      (1000)     8214 2020-04-17 08:04:14.000000 DynamicForms-0.9.9/DynamicForms.egg-info/PKG-INFO
+-rw-r--r--   0 jure      (1000) jure      (1000)    11559 2020-04-17 08:04:14.000000 DynamicForms-0.9.9/DynamicForms.egg-info/SOURCES.txt
+-rw-r--r--   0 jure      (1000) jure      (1000)        1 2020-04-17 08:04:14.000000 DynamicForms-0.9.9/DynamicForms.egg-info/dependency_links.txt
+-rw-r--r--   0 jure      (1000) jure      (1000)      107 2020-04-17 08:04:14.000000 DynamicForms-0.9.9/DynamicForms.egg-info/requires.txt
+-rw-r--r--   0 jure      (1000) jure      (1000)       13 2020-04-17 08:04:14.000000 DynamicForms-0.9.9/DynamicForms.egg-info/top_level.txt
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1499 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/LICENSE.rst
+-rw-rw-r--   0 jure      (1000) jure      (1000)      189 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/MANIFEST.in
+-rw-r--r--   0 jure      (1000) jure      (1000)     8214 2020-04-17 08:04:14.000000 DynamicForms-0.9.9/PKG-INFO
+-rw-rw-r--   0 jure      (1000) jure      (1000)     5917 2020-04-16 10:50:05.000000 DynamicForms-0.9.9/README.rst
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2020-04-17 08:04:14.000000 DynamicForms-0.9.9/dynamicforms/
+-rw-r--r--   0 jure      (1000) jure      (1000)      228 2020-04-17 08:03:53.000000 DynamicForms-0.9.9/dynamicforms/__init__.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)    20638 2020-03-03 07:27:29.000000 DynamicForms-0.9.9/dynamicforms/action.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)       99 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/apps.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1002 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/context_processors.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     1561 2020-02-25 12:32:14.000000 DynamicForms-0.9.9/dynamicforms/dynamicforms_migration_mixin.py
+-rw-r--r--   0 jure      (1000) jure      (1000)    28721 2020-03-24 09:34:21.000000 DynamicForms-0.9.9/dynamicforms/fields.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2020-04-17 08:04:14.000000 DynamicForms-0.9.9/dynamicforms/migrations/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/migrations/__init__.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2020-04-17 08:04:14.000000 DynamicForms-0.9.9/dynamicforms/mixins/
+-rw-r--r--   0 jure      (1000) jure      (1000)      362 2020-03-24 12:08:45.000000 DynamicForms-0.9.9/dynamicforms/mixins/__init__.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      492 2020-03-24 12:08:45.000000 DynamicForms-0.9.9/dynamicforms/mixins/action.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     1321 2020-03-24 12:08:45.000000 DynamicForms-0.9.9/dynamicforms/mixins/help_text.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      233 2020-03-24 12:08:45.000000 DynamicForms-0.9.9/dynamicforms/mixins/implicit_hidden.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     3433 2020-03-24 12:08:45.000000 DynamicForms-0.9.9/dynamicforms/mixins/implicit_natural_date.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     1026 2020-03-24 12:08:45.000000 DynamicForms-0.9.9/dynamicforms/mixins/null_choice.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     1552 2020-03-24 12:08:45.000000 DynamicForms-0.9.9/dynamicforms/mixins/related_field_ajax.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     6316 2020-04-17 08:03:53.000000 DynamicForms-0.9.9/dynamicforms/mixins/render.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      110 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/models.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1885 2019-07-26 10:41:59.000000 DynamicForms-0.9.9/dynamicforms/progress.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     6766 2020-02-20 09:31:54.000000 DynamicForms-0.9.9/dynamicforms/renderers.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)    10271 2020-04-16 15:55:16.000000 DynamicForms-0.9.9/dynamicforms/serializers.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     6935 2020-02-25 08:08:58.000000 DynamicForms-0.9.9/dynamicforms/settings.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2020-04-17 08:04:14.000000 DynamicForms-0.9.9/dynamicforms/static/
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2020-04-17 08:04:14.000000 DynamicForms-0.9.9/dynamicforms/static/bootstrap-3.4.1-dist/
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2020-04-17 08:04:14.000000 DynamicForms-0.9.9/dynamicforms/static/bootstrap-3.4.1-dist/css/
+-rw-rw-r--   0 jure      (1000) jure      (1000)    25682 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/bootstrap-3.4.1-dist/css/bootstrap-theme.css
+-rw-rw-r--   0 jure      (1000) jure      (1000)    48005 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/bootstrap-3.4.1-dist/css/bootstrap-theme.css.map
+-rw-rw-r--   0 jure      (1000) jure      (1000)    23411 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/bootstrap-3.4.1-dist/css/bootstrap-theme.min.css
+-rw-rw-r--   0 jure      (1000) jure      (1000)    75600 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/bootstrap-3.4.1-dist/css/bootstrap-theme.min.css.map
+-rw-rw-r--   0 jure      (1000) jure      (1000)   145933 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/bootstrap-3.4.1-dist/css/bootstrap.css
+-rw-rw-r--   0 jure      (1000) jure      (1000)   390887 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/bootstrap-3.4.1-dist/css/bootstrap.css.map
+-rw-rw-r--   0 jure      (1000) jure      (1000)   121457 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/bootstrap-3.4.1-dist/css/bootstrap.min.css
+-rw-rw-r--   0 jure      (1000) jure      (1000)   540434 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/bootstrap-3.4.1-dist/css/bootstrap.min.css.map
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2020-04-17 08:04:14.000000 DynamicForms-0.9.9/dynamicforms/static/bootstrap-3.4.1-dist/fonts/
+-rw-rw-r--   0 jure      (1000) jure      (1000)    20127 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/bootstrap-3.4.1-dist/fonts/glyphicons-halflings-regular.eot
+-rw-rw-r--   0 jure      (1000) jure      (1000)   108738 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/bootstrap-3.4.1-dist/fonts/glyphicons-halflings-regular.svg
+-rw-rw-r--   0 jure      (1000) jure      (1000)    45404 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/bootstrap-3.4.1-dist/fonts/glyphicons-halflings-regular.ttf
+-rw-rw-r--   0 jure      (1000) jure      (1000)    23424 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/bootstrap-3.4.1-dist/fonts/glyphicons-halflings-regular.woff
+-rw-rw-r--   0 jure      (1000) jure      (1000)    18028 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/bootstrap-3.4.1-dist/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2020-04-17 08:04:14.000000 DynamicForms-0.9.9/dynamicforms/static/bootstrap-3.4.1-dist/js/
+-rw-rw-r--   0 jure      (1000) jure      (1000)    75484 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/bootstrap-3.4.1-dist/js/bootstrap.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)    39680 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/bootstrap-3.4.1-dist/js/bootstrap.min.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)      484 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/bootstrap-3.4.1-dist/js/npm.js
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2020-04-17 08:04:14.000000 DynamicForms-0.9.9/dynamicforms/static/bootstrap-4.3.1-dist/
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2020-04-17 08:04:14.000000 DynamicForms-0.9.9/dynamicforms/static/bootstrap-4.3.1-dist/css/
+-rw-rw-r--   0 jure      (1000) jure      (1000)    64548 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/bootstrap-4.3.1-dist/css/bootstrap-grid.css
+-rw-rw-r--   0 jure      (1000) jure      (1000)   151749 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/bootstrap-4.3.1-dist/css/bootstrap-grid.css.map
+-rw-rw-r--   0 jure      (1000) jure      (1000)    48488 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/bootstrap-4.3.1-dist/css/bootstrap-grid.min.css
+-rw-rw-r--   0 jure      (1000) jure      (1000)   108539 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/bootstrap-4.3.1-dist/css/bootstrap-grid.min.css.map
+-rw-rw-r--   0 jure      (1000) jure      (1000)     4897 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/bootstrap-4.3.1-dist/css/bootstrap-reboot.css
+-rw-rw-r--   0 jure      (1000) jure      (1000)    76483 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/bootstrap-4.3.1-dist/css/bootstrap-reboot.css.map
+-rw-rw-r--   0 jure      (1000) jure      (1000)     4021 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/bootstrap-4.3.1-dist/css/bootstrap-reboot.min.css
+-rw-rw-r--   0 jure      (1000) jure      (1000)    32461 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/bootstrap-4.3.1-dist/css/bootstrap-reboot.min.css.map
+-rw-rw-r--   0 jure      (1000) jure      (1000)   192348 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/bootstrap-4.3.1-dist/css/bootstrap.css
+-rw-rw-r--   0 jure      (1000) jure      (1000)   492048 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/bootstrap-4.3.1-dist/css/bootstrap.css.map
+-rw-rw-r--   0 jure      (1000) jure      (1000)   155758 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/bootstrap-4.3.1-dist/css/bootstrap.min.css
+-rw-rw-r--   0 jure      (1000) jure      (1000)   625953 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/bootstrap-4.3.1-dist/css/bootstrap.min.css.map
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2020-04-17 08:04:14.000000 DynamicForms-0.9.9/dynamicforms/static/bootstrap-4.3.1-dist/js/
+-rw-rw-r--   0 jure      (1000) jure      (1000)   222911 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/bootstrap-4.3.1-dist/js/bootstrap.bundle.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)   402249 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/bootstrap-4.3.1-dist/js/bootstrap.bundle.js.map
+-rw-rw-r--   0 jure      (1000) jure      (1000)    78635 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/bootstrap-4.3.1-dist/js/bootstrap.bundle.min.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)   311949 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/bootstrap-4.3.1-dist/js/bootstrap.bundle.min.js.map
+-rw-rw-r--   0 jure      (1000) jure      (1000)   131637 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/bootstrap-4.3.1-dist/js/bootstrap.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)   250568 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/bootstrap-4.3.1-dist/js/bootstrap.js.map
+-rw-rw-r--   0 jure      (1000) jure      (1000)    58072 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/bootstrap-4.3.1-dist/js/bootstrap.min.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)   190253 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/bootstrap-4.3.1-dist/js/bootstrap.min.js.map
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2020-04-17 08:04:14.000000 DynamicForms-0.9.9/dynamicforms/static/dynamicforms/
+-rw-r--r--   0 jure      (1000) jure      (1000)    51688 2020-04-17 08:03:53.000000 DynamicForms-0.9.9/dynamicforms/static/dynamicforms/dynamicforms.js
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2020-04-17 08:04:14.000000 DynamicForms-0.9.9/dynamicforms/static/jquery_ui/
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2020-04-17 08:04:14.000000 DynamicForms-0.9.9/dynamicforms/static/jquery_ui/css/
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2020-04-17 08:04:14.000000 DynamicForms-0.9.9/dynamicforms/static/jquery_ui/css/images/
+-rw-rw-r--   0 jure      (1000) jure      (1000)      418 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/jquery_ui/css/images/ui-bg_diagonals-thick_18_b81900_40x40.png
+-rw-rw-r--   0 jure      (1000) jure      (1000)      312 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/jquery_ui/css/images/ui-bg_diagonals-thick_20_666666_40x40.png
+-rw-rw-r--   0 jure      (1000) jure      (1000)      262 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/jquery_ui/css/images/ui-bg_glass_100_f6f6f6_1x400.png
+-rw-rw-r--   0 jure      (1000) jure      (1000)      348 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/jquery_ui/css/images/ui-bg_glass_100_fdf5ce_1x400.png
+-rw-rw-r--   0 jure      (1000) jure      (1000)      207 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/jquery_ui/css/images/ui-bg_glass_65_ffffff_1x400.png
+-rw-rw-r--   0 jure      (1000) jure      (1000)     5815 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/jquery_ui/css/images/ui-bg_gloss-wave_35_f6a828_500x100.png
+-rw-rw-r--   0 jure      (1000) jure      (1000)      278 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/jquery_ui/css/images/ui-bg_highlight-soft_100_eeeeee_1x100.png
+-rw-rw-r--   0 jure      (1000) jure      (1000)      328 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/jquery_ui/css/images/ui-bg_highlight-soft_75_ffe45c_1x100.png
+-rw-rw-r--   0 jure      (1000) jure      (1000)     6922 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/jquery_ui/css/images/ui-icons_222222_256x240.png
+-rw-rw-r--   0 jure      (1000) jure      (1000)     4549 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/jquery_ui/css/images/ui-icons_228ef1_256x240.png
+-rw-rw-r--   0 jure      (1000) jure      (1000)     4549 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/jquery_ui/css/images/ui-icons_ef8c08_256x240.png
+-rw-rw-r--   0 jure      (1000) jure      (1000)     4549 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/jquery_ui/css/images/ui-icons_ffd27a_256x240.png
+-rw-rw-r--   0 jure      (1000) jure      (1000)     6299 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/jquery_ui/css/images/ui-icons_ffffff_256x240.png
+-rw-rw-r--   0 jure      (1000) jure      (1000)    31583 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/jquery_ui/css/jquery-ui.min.css
+-rw-rw-r--   0 jure      (1000) jure      (1000)    15548 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/jquery_ui/css/jquery-ui.structure.min.css
+-rw-rw-r--   0 jure      (1000) jure      (1000)    14436 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/jquery_ui/css/jquery-ui.theme.min.css
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2020-04-17 08:04:14.000000 DynamicForms-0.9.9/dynamicforms/static/jquery_ui/js/
+-rw-rw-r--   0 jure      (1000) jure      (1000)    86927 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/jquery_ui/js/jquery-3.3.1.min.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)   253669 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/jquery_ui/js/jquery-ui.min.js
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2020-04-17 08:04:14.000000 DynamicForms-0.9.9/dynamicforms/static/select2/
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2020-04-17 08:04:14.000000 DynamicForms-0.9.9/dynamicforms/static/select2/css/
+-rw-rw-r--   0 jure      (1000) jure      (1000)    16792 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/select2/css/select2-bootstrap3.min.css
+-rw-rw-r--   0 jure      (1000) jure      (1000)    19533 2019-05-31 14:28:35.000000 DynamicForms-0.9.9/dynamicforms/static/select2/css/select2-bootstrap4.min.css
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2020-04-17 08:04:14.000000 DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2020-04-17 08:04:14.000000 DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/css/
+-rw-rw-r--   0 jure      (1000) jure      (1000)    15196 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/css/select2.min.css
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2020-04-17 08:04:14.000000 DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2020-04-17 08:04:14.000000 DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/
+-rw-rw-r--   0 jure      (1000) jure      (1000)      846 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/af.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)      868 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/ar.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)      701 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/az.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)      906 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/bg.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)      940 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/bs.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)      876 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/ca.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1252 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/cs.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)      808 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/da.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)      853 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/de.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1015 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/dsb.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1132 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/el.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)      827 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/en.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)      892 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/es.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)      775 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/et.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)      844 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/eu.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1004 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/fa.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)      782 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/fi.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)      883 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/fr.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)      886 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/gl.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)      951 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/he.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1125 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/hi.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)      839 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/hr.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1016 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/hsb.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)      802 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/hu.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1005 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/hy.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)      752 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/id.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)      773 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/is.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)      876 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/it.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)      848 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/ja.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1065 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/km.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)      854 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/ko.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)      913 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/lt.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)      872 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/lv.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)      979 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/mk.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)      791 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/ms.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)      775 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/nb.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)      896 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/nl.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)      925 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/pl.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1019 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/ps.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)      853 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/pt-BR.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)      859 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/pt.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)      910 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/ro.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1127 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/ru.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1266 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/sk.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)      890 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/sl.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1067 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/sr-Cyrl.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)      938 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/sr.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)      786 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/sv.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1048 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/th.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)      773 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/tr.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1117 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/uk.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)      800 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/vi.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)      769 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/zh-CN.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)      708 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/zh-TW.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)   162676 2019-11-04 14:15:16.000000 DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/select2.full.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)    74931 2019-11-04 14:15:16.000000 DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/select2.full.min.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)   142778 2019-11-04 14:15:16.000000 DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/select2.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)    66615 2019-11-04 14:15:16.000000 DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/select2.min.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1260 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/struct.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2020-04-17 08:04:14.000000 DynamicForms-0.9.9/dynamicforms/templates/
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2020-04-17 08:04:14.000000 DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2020-04-17 08:04:14.000000 DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/bootstrap/
+-rw-rw-r--   0 jure      (1000) jure      (1000)      327 2019-07-09 09:00:49.000000 DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/bootstrap/base.html
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1411 2019-11-15 08:08:56.000000 DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/bootstrap/base_form.html
+-rw-rw-r--   0 jure      (1000) jure      (1000)      257 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/bootstrap/base_includes_select2.html
+-rw-rw-r--   0 jure      (1000) jure      (1000)     2374 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/bootstrap/base_includes_v3.html
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1519 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/bootstrap/base_includes_v4.html
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1957 2019-07-09 09:00:49.000000 DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/bootstrap/base_list.html
+-rw-r--r--   0 jure      (1000) jure      (1000)     1456 2020-04-17 08:03:53.000000 DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/bootstrap/base_table_body.html
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1190 2019-12-06 13:40:15.000000 DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/bootstrap/base_table_filter.html
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2020-04-17 08:04:14.000000 DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/bootstrap/field/
+-rw-rw-r--   0 jure      (1000) jure      (1000)     2184 2019-05-22 07:53:00.000000 DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/bootstrap/field/base_field_v3.html
+-rw-rw-r--   0 jure      (1000) jure      (1000)     2191 2019-05-22 07:53:00.000000 DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/bootstrap/field/base_field_v4.html
+-rw-rw-r--   0 jure      (1000) jure      (1000)      674 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/bootstrap/field/checkbox.html
+-rw-rw-r--   0 jure      (1000) jure      (1000)      515 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/bootstrap/field/checkbox_multiple.html
+-rw-rw-r--   0 jure      (1000) jure      (1000)      179 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/bootstrap/field/dict_field.html
+-rw-rw-r--   0 jure      (1000) jure      (1000)      620 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/bootstrap/field/fieldset.html
+-rw-rw-r--   0 jure      (1000) jure      (1000)      304 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/bootstrap/field/form.html
+-rw-rw-r--   0 jure      (1000) jure      (1000)      788 2019-11-04 14:15:16.000000 DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/bootstrap/field/input.html
+-rw-rw-r--   0 jure      (1000) jure      (1000)      172 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/bootstrap/field/list_field.html
+-rw-rw-r--   0 jure      (1000) jure      (1000)      668 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/bootstrap/field/list_fieldset.html
+-rw-rw-r--   0 jure      (1000) jure      (1000)      863 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/bootstrap/field/radio.html
+-rw-rw-r--   0 jure      (1000) jure      (1000)     2738 2019-12-20 09:07:53.000000 DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/bootstrap/field/select.html
+-rw-rw-r--   0 jure      (1000) jure      (1000)     2331 2019-12-20 09:07:53.000000 DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/bootstrap/field/select_multiple.html
+-rw-rw-r--   0 jure      (1000) jure      (1000)      529 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/bootstrap/field/textarea.html
+-rw-rw-r--   0 jure      (1000) jure      (1000)      987 2019-06-28 12:42:14.000000 DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/bootstrap/modal_dialog_v3.html
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1007 2019-06-28 12:42:14.000000 DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/bootstrap/modal_dialog_v4.html
+-rw-rw-r--   0 jure      (1000) jure      (1000)      658 2019-07-09 09:00:49.000000 DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/bootstrap/page.html
+-rw-rw-r--   0 jure      (1000) jure      (1000)      896 2019-07-26 11:13:36.000000 DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/bootstrap/progress_dialog.html
+-rw-rw-r--   0 jure      (1000) jure      (1000)      286 2019-07-09 09:00:49.000000 DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/bootstrap/progress_dialog_style.html
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2020-04-17 08:04:14.000000 DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/jquery_ui/
+-rw-rw-r--   0 jure      (1000) jure      (1000)      258 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/jquery_ui/base.html
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1426 2019-11-15 08:08:56.000000 DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/jquery_ui/base_form.html
+-rw-r--r--   0 jure      (1000) jure      (1000)     2584 2020-02-26 13:41:06.000000 DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/jquery_ui/base_includes.html
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1923 2019-05-22 07:53:00.000000 DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/jquery_ui/base_list.html
+-rw-r--r--   0 jure      (1000) jure      (1000)     1438 2020-04-17 08:03:53.000000 DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/jquery_ui/base_table_body.html
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1197 2019-12-06 13:40:15.000000 DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/jquery_ui/base_table_filter.html
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2020-04-17 08:04:14.000000 DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/jquery_ui/field/
+-rw-rw-r--   0 jure      (1000) jure      (1000)     2109 2019-05-22 07:53:00.000000 DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/jquery_ui/field/base_field.html
+-rw-rw-r--   0 jure      (1000) jure      (1000)      669 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/jquery_ui/field/checkbox.html
+-rw-rw-r--   0 jure      (1000) jure      (1000)      516 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/jquery_ui/field/checkbox_multiple.html
+-rw-rw-r--   0 jure      (1000) jure      (1000)      179 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/jquery_ui/field/dict_field.html
+-rw-rw-r--   0 jure      (1000) jure      (1000)      287 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/jquery_ui/field/fieldset.html
+-rw-rw-r--   0 jure      (1000) jure      (1000)      301 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/jquery_ui/field/form.html
+-rw-r--r--   0 jure      (1000) jure      (1000)      828 2020-02-25 12:32:14.000000 DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/jquery_ui/field/input.html
+-rw-rw-r--   0 jure      (1000) jure      (1000)      172 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/jquery_ui/field/list_field.html
+-rw-rw-r--   0 jure      (1000) jure      (1000)      195 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/jquery_ui/field/list_fieldset.html
+-rw-rw-r--   0 jure      (1000) jure      (1000)      864 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/jquery_ui/field/radio.html
+-rw-rw-r--   0 jure      (1000) jure      (1000)     3320 2019-12-20 09:07:53.000000 DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/jquery_ui/field/select.html
+-rw-rw-r--   0 jure      (1000) jure      (1000)     2078 2019-12-20 09:07:53.000000 DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/jquery_ui/field/select_multiple.html
+-rw-r--r--   0 jure      (1000) jure      (1000)      492 2020-02-25 12:32:14.000000 DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/jquery_ui/field/textarea.html
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1105 2019-10-15 06:32:16.000000 DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/jquery_ui/modal_dialog.html
+-rw-rw-r--   0 jure      (1000) jure      (1000)      694 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/jquery_ui/page.html
+-rw-rw-r--   0 jure      (1000) jure      (1000)      286 2019-07-26 10:42:57.000000 DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/jquery_ui/progress_dialog.html
+-rw-rw-r--   0 jure      (1000) jure      (1000)      378 2019-07-09 09:00:49.000000 DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/jquery_ui/progress_dialog_style.html
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2020-04-17 08:04:14.000000 DynamicForms-0.9.9/dynamicforms/templatetags/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2019-05-14 15:53:14.000000 DynamicForms-0.9.9/dynamicforms/templatetags/__init__.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     9744 2020-04-17 08:03:53.000000 DynamicForms-0.9.9/dynamicforms/templatetags/dynamicforms.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      229 2020-01-23 08:59:43.000000 DynamicForms-0.9.9/dynamicforms/urls.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)       38 2020-01-23 08:59:43.000000 DynamicForms-0.9.9/dynamicforms/views.py
+-rw-r--r--   0 jure      (1000) jure      (1000)    14879 2020-02-20 11:21:04.000000 DynamicForms-0.9.9/dynamicforms/viewsets.py
+-rw-r--r--   0 jure      (1000) jure      (1000)      104 2020-03-24 09:34:21.000000 DynamicForms-0.9.9/requirements.txt
+-rw-rw-r--   0 jure      (1000) jure      (1000)       25 2019-05-29 07:17:47.000000 DynamicForms-0.9.9/requirements_test_functional.txt
+-rw-r--r--   0 jure      (1000) jure      (1000)       38 2020-04-17 08:04:14.000000 DynamicForms-0.9.9/setup.cfg
+-rw-r--r--   0 jure      (1000) jure      (1000)     1440 2020-04-17 08:03:53.000000 DynamicForms-0.9.9/setup.py
```

### Comparing `DynamicForms-0.9.8/DynamicForms.egg-info/PKG-INFO` & `DynamicForms-0.9.9/DynamicForms.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: DynamicForms
-Version: 0.9.8
+Version: 0.9.9
 Summary: DynamicForms performs all the visualisation & data entry of your DRF Serializers & ViewSets and adds some candy of its own: It is a django library that gives you the power of dynamically-shown form fields, auto-filled default values, dynamic record loading and similar candy with little effort. To put it differently: once defined, a particular ViewSet / Serializer can be rendered in multiple ways allowing you to perform viewing and authoring operations on the data in question.
 Home-page: https://github.com/velis74/DynamicForms
 Author: Jure Erznožnik
 Author-email: jure@velis.si
 License: BSD-3-Clause
 Description: What is DynamicForms?
         =====================
         
-        DynamicForms is a library that eliminates HTML form boilerplate by providing all the relevant functionality. Instead
-        of having to program tables, dialog, data forms, DynamicForms already provides you with the functionality - all you have
-        to do is declare a few extra properties to your DRF Serializers and ViewSets.
+        DynamicForms wants to eliminate HTML form boilerplate for generic tables & forms. Specifying a single DRF Serializer / ViewSet and possibly desired form layout instantly provides both HTML renders and JSON renders (and anything else DRF supports) giving you free choice of how to implement your project. 
         
         It performs all the visualisation & data entry of your DRF Serializers & ViewSets and adds some candy of its
         own: It is a `django <https://www.djangoproject.com/>`_ library that gives you the power of dynamically-shown form
         fields, auto-filled default values, dynamic record loading and similar candy with little effort. To put it differently:
         once defined, a particular ViewSet / Serializer can be rendered in multiple ways allowing you to perform viewing and
         authoring operations on the data in question.
         
@@ -29,24 +27,25 @@
         
         * Turn your rest-framework ViewSets into HTML forms
         * Powerful HTML based CRUD
         
            * Support for fetching "new" records, both in JSON or in HTML
            * Render to HTML, dialog html or from your own template
            * Render form (embedded or dialog) or table, depending on situation
+           * Dynamically display & hide fields based on other fields' values
            * Easily add actions and place the buttons to execute them anywhere you like
         
         * Clear separation of list & dialog templates
         * Dynamic loading of additional records for table views
         * Easy implementation of simple filtering
         * Action items, declared globally, placed where you need them
         * Custom templates whenever & wherever you want them
         * Render to full html or work with dialogs within same page or both at the same time
         * Each form and field have a unique HTML id for easy finding & manipulation
-        * Bootstrap 3 & 4 templates, jQuery UI coming soon, easy to make your own or enhance existing
+        * Bootstrap 3 & 4 and jQuery UI templates, easy to make your own or enhance existing
         * Support for form validation, will show errors even if they are not tied to a field
         * Convenient JS functions for easier action scripting
         * Progress dialog for long lasting ajax operations
         
         Quick start guide
         =================
```

### Comparing `DynamicForms-0.9.8/DynamicForms.egg-info/SOURCES.txt` & `DynamicForms-0.9.9/DynamicForms.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -11,25 +11,32 @@
 DynamicForms.egg-info/top_level.txt
 dynamicforms/__init__.py
 dynamicforms/action.py
 dynamicforms/apps.py
 dynamicforms/context_processors.py
 dynamicforms/dynamicforms_migration_mixin.py
 dynamicforms/fields.py
-dynamicforms/mixins.py
 dynamicforms/models.py
 dynamicforms/progress.py
 dynamicforms/renderers.py
 dynamicforms/serializers.py
 dynamicforms/settings.py
 dynamicforms/struct.py
 dynamicforms/urls.py
 dynamicforms/views.py
 dynamicforms/viewsets.py
 dynamicforms/migrations/__init__.py
+dynamicforms/mixins/__init__.py
+dynamicforms/mixins/action.py
+dynamicforms/mixins/help_text.py
+dynamicforms/mixins/implicit_hidden.py
+dynamicforms/mixins/implicit_natural_date.py
+dynamicforms/mixins/null_choice.py
+dynamicforms/mixins/related_field_ajax.py
+dynamicforms/mixins/render.py
 dynamicforms/static/bootstrap-3.4.1-dist/css/bootstrap-theme.css
 dynamicforms/static/bootstrap-3.4.1-dist/css/bootstrap-theme.css.map
 dynamicforms/static/bootstrap-3.4.1-dist/css/bootstrap-theme.min.css
 dynamicforms/static/bootstrap-3.4.1-dist/css/bootstrap-theme.min.css.map
 dynamicforms/static/bootstrap-3.4.1-dist/css/bootstrap.css
 dynamicforms/static/bootstrap-3.4.1-dist/css/bootstrap.css.map
 dynamicforms/static/bootstrap-3.4.1-dist/css/bootstrap.min.css
```

### Comparing `DynamicForms-0.9.8/LICENSE.rst` & `DynamicForms-0.9.9/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/PKG-INFO` & `DynamicForms-0.9.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: DynamicForms
-Version: 0.9.8
+Version: 0.9.9
 Summary: DynamicForms performs all the visualisation & data entry of your DRF Serializers & ViewSets and adds some candy of its own: It is a django library that gives you the power of dynamically-shown form fields, auto-filled default values, dynamic record loading and similar candy with little effort. To put it differently: once defined, a particular ViewSet / Serializer can be rendered in multiple ways allowing you to perform viewing and authoring operations on the data in question.
 Home-page: https://github.com/velis74/DynamicForms
 Author: Jure Erznožnik
 Author-email: jure@velis.si
 License: BSD-3-Clause
 Description: What is DynamicForms?
         =====================
         
-        DynamicForms is a library that eliminates HTML form boilerplate by providing all the relevant functionality. Instead
-        of having to program tables, dialog, data forms, DynamicForms already provides you with the functionality - all you have
-        to do is declare a few extra properties to your DRF Serializers and ViewSets.
+        DynamicForms wants to eliminate HTML form boilerplate for generic tables & forms. Specifying a single DRF Serializer / ViewSet and possibly desired form layout instantly provides both HTML renders and JSON renders (and anything else DRF supports) giving you free choice of how to implement your project. 
         
         It performs all the visualisation & data entry of your DRF Serializers & ViewSets and adds some candy of its
         own: It is a `django <https://www.djangoproject.com/>`_ library that gives you the power of dynamically-shown form
         fields, auto-filled default values, dynamic record loading and similar candy with little effort. To put it differently:
         once defined, a particular ViewSet / Serializer can be rendered in multiple ways allowing you to perform viewing and
         authoring operations on the data in question.
         
@@ -29,24 +27,25 @@
         
         * Turn your rest-framework ViewSets into HTML forms
         * Powerful HTML based CRUD
         
            * Support for fetching "new" records, both in JSON or in HTML
            * Render to HTML, dialog html or from your own template
            * Render form (embedded or dialog) or table, depending on situation
+           * Dynamically display & hide fields based on other fields' values
            * Easily add actions and place the buttons to execute them anywhere you like
         
         * Clear separation of list & dialog templates
         * Dynamic loading of additional records for table views
         * Easy implementation of simple filtering
         * Action items, declared globally, placed where you need them
         * Custom templates whenever & wherever you want them
         * Render to full html or work with dialogs within same page or both at the same time
         * Each form and field have a unique HTML id for easy finding & manipulation
-        * Bootstrap 3 & 4 templates, jQuery UI coming soon, easy to make your own or enhance existing
+        * Bootstrap 3 & 4 and jQuery UI templates, easy to make your own or enhance existing
         * Support for form validation, will show errors even if they are not tied to a field
         * Convenient JS functions for easier action scripting
         * Progress dialog for long lasting ajax operations
         
         Quick start guide
         =================
```

### Comparing `DynamicForms-0.9.8/README.rst` & `DynamicForms-0.9.9/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 What is DynamicForms?
 =====================
 
-DynamicForms is a library that eliminates HTML form boilerplate by providing all the relevant functionality. Instead
-of having to program tables, dialog, data forms, DynamicForms already provides you with the functionality - all you have
-to do is declare a few extra properties to your DRF Serializers and ViewSets.
+DynamicForms wants to eliminate HTML form boilerplate for generic tables & forms. Specifying a single DRF Serializer / ViewSet and possibly desired form layout instantly provides both HTML renders and JSON renders (and anything else DRF supports) giving you free choice of how to implement your project. 
 
 It performs all the visualisation & data entry of your DRF Serializers & ViewSets and adds some candy of its
 own: It is a `django <https://www.djangoproject.com/>`_ library that gives you the power of dynamically-shown form
 fields, auto-filled default values, dynamic record loading and similar candy with little effort. To put it differently:
 once defined, a particular ViewSet / Serializer can be rendered in multiple ways allowing you to perform viewing and
 authoring operations on the data in question.
 
@@ -21,24 +19,25 @@
 
 * Turn your rest-framework ViewSets into HTML forms
 * Powerful HTML based CRUD
 
    * Support for fetching "new" records, both in JSON or in HTML
    * Render to HTML, dialog html or from your own template
    * Render form (embedded or dialog) or table, depending on situation
+   * Dynamically display & hide fields based on other fields' values
    * Easily add actions and place the buttons to execute them anywhere you like
 
 * Clear separation of list & dialog templates
 * Dynamic loading of additional records for table views
 * Easy implementation of simple filtering
 * Action items, declared globally, placed where you need them
 * Custom templates whenever & wherever you want them
 * Render to full html or work with dialogs within same page or both at the same time
 * Each form and field have a unique HTML id for easy finding & manipulation
-* Bootstrap 3 & 4 templates, jQuery UI coming soon, easy to make your own or enhance existing
+* Bootstrap 3 & 4 and jQuery UI templates, easy to make your own or enhance existing
 * Support for form validation, will show errors even if they are not tied to a field
 * Convenient JS functions for easier action scripting
 * Progress dialog for long lasting ajax operations
 
 Quick start guide
 =================
```

### Comparing `DynamicForms-0.9.8/dynamicforms/action.py` & `DynamicForms-0.9.9/dynamicforms/action.py`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/context_processors.py` & `DynamicForms-0.9.9/dynamicforms/context_processors.py`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/dynamicforms_migration_mixin.py` & `DynamicForms-0.9.9/dynamicforms/dynamicforms_migration_mixin.py`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/fields.py` & `DynamicForms-0.9.9/dynamicforms/fields.py`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/mixins.py` & `DynamicForms-0.9.9/dynamicforms/viewsets.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,303 +1,330 @@
-import re
-import uuid as uuid_module
-from collections.abc import Hashable
-from datetime import datetime
-from enum import IntEnum
-from typing import Any, Optional, Union
-
-from django.utils import timezone
-from rest_framework.fields import ChoiceField, DateField, TimeField
-from rest_framework.relations import ManyRelatedField, RelatedField
+from datetime import datetime, timedelta
+from typing import List, Union
+
+import pytz
+from django.conf import settings
+from django.contrib.auth.views import redirect_to_login
+from django.db import models
+from django.http import Http404
+from rest_framework import status, viewsets
+from rest_framework.exceptions import ValidationError
+from rest_framework.renderers import JSONRenderer
+from rest_framework.response import Response
 from rest_framework.serializers import ListSerializer
-from rest_framework.templatetags import rest_framework as drftt
+from rest_framework.utils.serializer_helpers import ReturnDict, ReturnList
 
-from .action import Actions
+from dynamicforms.fields import BooleanField
+from .renderers import TemplateHTMLRenderer
 from .settings import DYNAMICFORMS
 
 
-class DisplayMode(IntEnum):
-    SUPPRESS = 1  # Field will be entirely suppressed. it will not render (not even to JSON) and will not parse for PUT
-    HIDDEN = 5  # Field will render as <input type="hidden"> or <tr data-field_name>
-    INVISIBLE = 8  # Field will render completely, but with display: none. Equal to setting its style = {display: none}
-    FULL = 10  # Field will render completely
-
-
-class RenderMixin(object):
+class NewMixin(object):
     """
-    Is used in fields and serializers, so every field and serializer gets its unique id. Also to specify where and how
-    fields should render.
-
-    In form where serializer is used, id is serializers uuid. Table with list of records has id »list-serializer.uuid«,
-    in dialog id is »dialog-{serializer.uuid}« and save button's id on dialog is »save-{serializer.uuid}«
+    Provides support for retrieving default values for a new record.
 
-    Similar for fields: All inputs in HTML get id from field.uuid. Div that contains all that belongs to the field has
-    »container-{field.uuid}« for id, label has »label-{field.uuid}« and help text (if exists) has »help-{field.uuid}«
-    for id.
-
-    Used for rendering individual field to table view
+    Caution: Do not use directly. This is only a mixin and is used in final ViewSet derivatives.
     """
 
-    def __init__(self, *args, uuid: uuid_module.UUID = None,
-                 display: DisplayMode = None,  # Leave at default
-                 display_table: DisplayMode = None,  # Leave at default
-                 display_form: DisplayMode = None,  # Leave at default
-                 table_classes: str = '',
-                 **kwargs):
+    def new_object(self: viewsets.ModelViewSet):
         """
+        Returns a new model instance. If you need it pre-populated with default values, this is the method to override.
 
-        :param args: passed on to inherited constructors
-        :param uuid: custom specified field UUID. if not specified, it will be assigned automatically
-        :param display: see DisplayMode enum. Specifies how field will render. Leave at None for default (FULL)
-            display_form and display_table also accepted for better granularity
-        :param table_classes: css classes to add to the table column
-        :param kwargs: passed on to inherited constructors
+        :return: model instance
         """
-        super().__init__(*args, **kwargs)
-        self.uuid = uuid or uuid_module.uuid1()
-        # noinspection PyUnresolvedReferences
-        self.display_table = display_table or display or \
-            (DisplayMode.FULL if not getattr(self, 'write_only', False) else DisplayMode.SUPPRESS)
-        self.display_form = display_form or display or DisplayMode.FULL
-        self.table_classes = table_classes
-
-    def set_display(self, value):
-        self.display_form = self.display_table = value
-
-    display = property(lambda self: self.display_form, set_display)
-
-    # noinspection PyUnusedLocal
-    def render_to_table(self, value, row_data):
-        """
-        Renders field value for table view
-
-        :param value: field value
-        :param row_data: data for entire row (for more complex renderers)
-        :return: rendered value for table view
-        """
-        get_queryset = getattr(self, 'get_queryset', None)
-        if isinstance(self, RelatedField) or get_queryset:
-            # shortcut for getting display value for table without actually getting the entire table into choices
-            qs = get_queryset()
-            try:
-                qs = qs.filter(pk=value)
-                choices = {self.to_representation(item): self.display_value(item) for item in qs}
-            except:
-                choices = getattr(self, 'choices', {})
-        elif isinstance(self, ManyRelatedField):
-            # if value is a list, we're dealing with ManyRelatedField, so let's not do that
-            cr = self.child_relation
-            return ', '.join((cr.display_value(item) for item in cr.get_queryset().filter(pk__in=value)))
-        else:
-            choices = getattr(self, 'choices', {})
+        # TODO: This function must return an object that has its field values correctly / realistically filled out
+        # Example: if a certain field's value hides (sets another field to None), then that second field can't be
+        # set to 42, can it?
+        # can we run some kind of validation to enforce this?
+        # Not that easy: the returned record may not validate for its (correctly) empty fields
+        # Maybe we will have to run JavaScript onchange for all fields displayed to ensure at least some consistency?
+        # If we do not, subsequent validation may fail because a hidden field has a value
+        return self.get_queryset().model()
 
-        if isinstance(value, Hashable) and value in choices:
-            # choice field: let's render display names, not values
-            return drftt.format_value(choices[value])
-        if value is None:
-            return DYNAMICFORMS.null_text_table
-
-        return drftt.format_value(value)
-
-    def validate_empty_values(self, data):
-        res = super().validate_empty_values(data)
-        # This is to fix a problem with calculated fields which was only solved in DRF 3.10.
-        # Forces validation and inclusion of the field into validated data. See comment in original function.
-        if res == (True, None) and data is None and self.source == '*':
-            return (False, None)
-        return res
+    # noinspection PyUnresolvedReferences
+    def retrieve(self: viewsets.ModelViewSet, request, *args, **kwargs):
+        try:
+            if not hasattr(super(), 'retrieve'):
+                raise Http404()  # This is not a ModelViewSet, so we don't have a retrieval mechanism
+            return super().retrieve(request, *args, **kwargs)
+        except Http404:
+            lookup_url_kwarg = self.lookup_url_kwarg or self.lookup_field
+            filter_kwargs = {self.lookup_field: self.kwargs[lookup_url_kwarg]}
+            if filter_kwargs.get('pk', None) == 'new':
+                instance = self.new_object()
+                serializer = self.get_serializer(instance)
+                return Response(serializer.data)
+            else:
+                raise
 
 
-class ActionMixin(object):
-    """
-    Used in fields allowing declaration of actions that happen when field values change
+class PutPostMixin(object):
     """
+    Provides support for when there is no record id in URL when calling PUT
+    (First empty form is loaded. Than user loads existing data to this form and updates it... - Perform PUT action)
 
-    def __init__(self, *args, actions: Actions = None, **kwargs):
-        super().__init__(*args, **kwargs)
-        act = actions or Actions(None)
-        act.actions.extend(getattr(self, 'actions', Actions()).actions)
-        # Obtain a personalised list of actions
-        self.actions = act.get_resolved_copy(self)
-
+    or
 
-class NullChoiceMixin(object):
+    Provides support for when there is record id in URL when calling POST
+    (First form for some existing record is loaded. Than user wants to create new record for it.
+    - deletes redord ID and perform POST action)
     """
-    Declaring ChoiceField's null_choice_text
-      (what should be rendered for "no selection"; DRF's default is ---------)
-      We also support user declaring a choice with None value and a different text (see hidden fields example)
-    """
-
-    @property
-    def null_choice_text(self):
-        res = '--------'
-        if isinstance(self, ChoiceField) and not getattr(self, 'get_queryset', None):
-            # Only do this for true ChoiceFields. ReladedFields would run a query here
-            # Possibly we will at some point have to enable this for relatedfields too
-            for opt in self.iter_options():
-                if opt.start_option_group or opt.end_option_group:
-                    pass
-                elif opt.value is None:
-                    res = opt.display_text
-        return res
 
-    def iter_options_bound(self, value):
-        return super().iter_options()
+    # When there is no record id in URL when calling PUT, this function will be called
+    # noinspection PyUnresolvedReferences
+    def put(self: viewsets.ModelViewSet, request, *args, **kwargs):
+        self.kwargs['pk'] = request.data['id']
+        return self.update(request, *args, **kwargs)
 
+    # When there is record id in URL when calling POST, this function will be called
+    # noinspection PyUnresolvedReferences
+    def post(self: viewsets.ModelViewSet, request, *args, **kwargs):
+        return self.create(request, *args, **kwargs)
 
-class HiddenFieldMixin(RenderMixin):
 
-    def __init__(self, *args, **kwargs):
-        kwargs.setdefault('display_table', DisplayMode.SUPPRESS)
-        super().__init__(*args, **kwargs)
+class TemplateRendererMixin():
+    template_context = {}
+    """
+    template_context provides configuration to templates being rendered
 
+    Note that when adding data from database, it is advised to make this definition a callable so that it is evaluated
+    on each render of the ViewSet: that way you can ensure data is always loaded fresh from database.
 
-class RelatedFieldAJAXMixin(object):
+    e.g.
 
-    def __init__(self, *args, url_reverse: Optional[str] = None, placeholder: Optional[str] = None,
-                 additional_parameters: Optional[dict] = None, query_field: str = 'query', **kwargs):
-        """
-        Allows us to use AJAX to populate select2 options instead of pre-populating at render time
+    .. code-block:: python
 
-        :param args:
-        :param url_reverse: reverse url to ViewSet providing the JSON data
-        :param placeholder: select2 placeholder to display until user selects a value
-        :param additional_parameters: additional parameters to be sent to ViewSet as part of the query
-        :param query_field: field against which user search will be performed
-        :param kwargs:
-        """
-        super().__init__(*args, **kwargs)
-        self.url_reverse = url_reverse
-        self.placeholder = placeholder
-        self.additional_parameters = additional_parameters
-        self.query_field = query_field
-
-    @property
-    def additional_parameters_urlencoded(self):
-        from django.utils.http import urlencode
-        return '?' + urlencode(self.additional_parameters)
+       template_context = lambda self: dict(items=MyModel.objects.all())
 
-    # noinspection PyUnresolvedReferences
-    def iter_options_bound(self, value):
-        if self.url_reverse:
-            qry = self.get_queryset()
-            try:
-                qry = qry.filter(pk=value)
-                return [dict(value=value, display_text=self.display_value(qry.first()))]
-            except:
-                return []
-        return super().iter_options()
+    or
 
+    .. code-block:: python
 
-class NaturalDateTimeMixin(object):
-    """
-    Used for rendering datetime in human natural style (e.g.: 1 hour, 10 minutes ago)
+       def template_context(self):
+           return dict(items=MyModel.objects.all())
     """
 
-    def __init__(self, *args, table_format: str = '', **kwargs) -> None:
-        """
+    template_name = DYNAMICFORMS.table_base_template  #: template filename for listing multiple records (html renderer)
 
-        :param args:
-        :param table_format: Format for datetime rendering in table (non editable). If format is %N:{precision},
-            datetime will render in natural style with {precision} depth
-        :param kwargs:
-        """
-        super().__init__(*args, **kwargs)
-        self.table_format = table_format
+    # noinspection PyAttributeOutsideInit
+    def initialize_request(self, request, *args, **kwargs):
+        # Caution: just to be sure for any future debugging: the request parameter to this function is a WSGIRequest
+        #  while the return Request is actually DRF Request
+        #  As a consequence, form values don't get parsed until you actually call super().initialize_request
+        #  There's no "request.data", etc. Just saying. So you don't debug for two hours next time. By "you" I mean me
+
+        # Force render using a given render path (full page, table, table rows, form, dialog with form)
+        self.render_type = request.META.get('HTTP_X_DF_RENDER_TYPE', request.GET.get('df_render_type', 'page'))
+
+        if request.method.lower() == 'post' and request.POST.get('data-dynamicforms-method', None):
+            # This is a hack because HTML forms can only do POST & GET. This way we also get PUT & PATCH
+            request.method = request.POST.get('data-dynamicforms-method')
+            # If we don't set this META, django won't recognise our CSRF token
+            request.META['HTTP_X_CSRFTOKEN'] = request.POST['csrfmiddlewaretoken']
+        return super().initialize_request(request, *args, **kwargs)
+
+    def finalize_response(self, request, response, *args, **kwargs):
+        if not isinstance(response, Response):
+            return response
+
+        res = super().finalize_response(request, response, *args, **kwargs)
+
+        def get_query_params():
+            if request.query_params:
+                return '?' + '&'.join(['%s=%s' % (key, value) for key, value in request.query_params.items()])
+            return ''
+
+        if isinstance(res.accepted_renderer, TemplateHTMLRenderer):
+            if status.is_success(res.status_code) or res.status_code == status.HTTP_400_BAD_REQUEST:
+                if isinstance(res.data, dict) and 'next' in res.data and 'results' in res.data and \
+                        isinstance(res.data['results'], (ReturnList, ReturnDict)):
+                    serializer = res.data['results'].serializer
+                else:
+                    serializer = res.data.serializer
 
-    # noinspection PyUnresolvedReferences
-    def to_representation(self, value: Any) -> Any:
-        if not value:
-            return None
+                if isinstance(serializer, ListSerializer):
+                    serializer.child.render_type = self.render_type
+                else:
+                    serializer.render_type = self.render_type
 
-        if isinstance(value, str):
-            return value
+                if self.render_type in ('table', 'table rows'):
+                    serializer.data_template = self.template_name
+                elif self.render_type == 'dialog':
+                    serializer.data_template = DYNAMICFORMS.modal_dialog_template
+                    res.template_name = DYNAMICFORMS.modal_dialog_template
+                elif self.render_type == 'form':
+                    serializer.data_template = res.data.serializer.template_name
+                    res.template_name = res.data.serializer.template_name
+                else:
+                    if isinstance(serializer, ListSerializer):
+                        serializer.child.render_type = 'table'
+                        serializer.child.data_template = self.template_name
+                    else:
+                        serializer.render_type = 'form'
+                        serializer.data_template = serializer.template_name
+            elif res.status_code in (status.HTTP_401_UNAUTHORIZED, status.HTTP_403_FORBIDDEN) and \
+                    self.render_type != 'dialog':
+                # TODO: We should show a message here that user is not authorized for this action (only for 403)
+                res = redirect_to_login(request.path_info + get_query_params())
+        return res
 
-        if isinstance(self.parent.parent, ListSerializer):
-            output_format = getattr(self, 'table_format', None)
-            if output_format is not None:
-                if re.match(r'%N:\d+', output_format):
-                    imported = False
-                    try:
-                        # This library (will-natural) is used because is the only one we could find that adds text
-                        # saying when is this datetime ("ago" or "from now") and have the possibility to set max
-                        # precision
-
-                        # noinspection PyPackageRequirements
-                        from natural.date import duration
-                        imported = True
-                    except:
-                        print('Install library for natural presentation of date (pip install will-natural)')
-
-                    if imported:
-                        if isinstance(self, DateField):
-                            now = timezone.now().date()
-                        elif isinstance(self, TimeField):
-                            now = datetime.now()
-                            value = datetime.now().replace(hour=value.hour, minute=value.minute, second=value.second,
-                                                           microsecond=value.microsecond)
-                        else:
-                            now = timezone.now()
 
-                        # noinspection PyUnboundLocalVariable
-                        return duration(value, now=now, precision=int(output_format.split(':')[1]))
-                else:
-                    global_format = getattr(self, 'format', None)
-                    setattr(self, 'format', output_format)
-                    value = super().to_representation(value)
-                    setattr(self, 'format', global_format)
-                    return value
-        return super().to_representation(value)
+class ModelViewSet(NewMixin, PutPostMixin, TemplateRendererMixin, viewsets.ModelViewSet):
+    """
+    In addition to all the functionality, provided by DRF, DynamicForms ViewSet has some extra features:
 
+    * Separate templates for rendering list or single record
+    * You can request a "new" record and even have it pre-populated with values
+    * To render viewset as API or JSON use the same method as in DRF: To render it in HTML just add ".html" to the URL.
+    * Standard DRF router URL patterns apply:
 
-class TimeFieldMixin(NaturalDateTimeMixin):
+       * To render a new record use pk=new.
+       * To render an existing record (for editing) use pk={record_id}.
 
-    def __init__(self, *args, table_format: str = None, **kwargs) -> None:
-        super().__init__(*args, table_format=table_format, **kwargs)
+    """
 
+    def paginate_queryset(self, queryset):
+        """
+        Return a single page of results, or `None` if pagination is disabled.
+        """
+        if self.paginator is None:
+            return None
+        # determine request format and handle pagination for json format
+        if isinstance(self.request.accepted_renderer, JSONRenderer) and not BooleanField().to_internal_value(
+                self.request.META.get('HTTP_X_PAGINATION', self.request.GET.get('x_df_pagination', False))):
+            return None
+        return self.paginator.paginate_queryset(queryset, self.request, view=self)
 
-class DateFieldMixin(NaturalDateTimeMixin):
+    def get_queryset(self):
+        """
+        Returns records from queryset with filters applied
+
+        :return: filtered records
+        """
+        return super().get_queryset()
 
-    def __init__(self, *args, table_format: str = None, **kwargs) -> None:
-        super().__init__(*args, table_format=table_format, **kwargs)
+    def filter_queryset(self, queryset, query_params=None):
+        """
+        Applies filters for all fields
 
+        :param queryset: Queryset
+        :param query_params: Custom query_params if needed
+        :return: queryset with filters applied
+        """
+        res = queryset
+        if self.request:
+            if query_params is None:
+                query_params = self.request.query_params
+            for fld, val in query_params.items():
+                res = self.filter_queryset_field(res, fld, val)
+        return res
 
-class DateTimeFieldMixin(NaturalDateTimeMixin):
+    # noinspection PyMethodMayBeStatic
+    def filter_queryset_field(self, queryset, field, value):
+        """
+        Applies filter to individual field
 
-    def __init__(self, *args, table_format: str = None, **kwargs) -> None:
-        super().__init__(*args, table_format=table_format, **kwargs)
+        :param queryset: Queryset
+        :param field: Field name
+        :param value: Field value
+        :return: queryset with applied filter for the field
+        """
+        if value is None or value == '':
+            return queryset
 
+        model_meta = queryset.model._meta
 
-class FieldHelpTextMixin(object):
-    """
-    Redefines help_text property such that we can set help text for api docs and form help text
-    """
+        if field not in (fld.name for fld in model_meta.get_fields()):
+            return queryset
 
-    def __init__(self, *args, help_text: Union[str, dict, None] = None, help_text_form: Optional[str] = None,
-                 **kwargs) -> None:
-        super().__init__(*args, help_text=help_text, **kwargs)
-        self.help_text = help_text
-        if help_text_form or not isinstance(help_text, dict):
-            self._help_text_form = help_text_form or self.help_text
-
-    def get_help_text(self):
-        return self._help_text
-
-    def set_help_text(self, value):
-        if isinstance(value, dict):
-            self._help_text = value.get('doc', None)
-            self._help_text_form = value.get('form', None)
+        # TODO: this would probably be better moved into the fields themselves
+        if isinstance(model_meta.get_field(field), (models.CharField, models.TextField)):
+            return queryset.filter(**{field + '__icontains': value})
+        if isinstance(model_meta.get_field(field), (models.DateField, models.DateTimeField)):
+            date_time = None
+            for date_time_fmt in [settings.DATETIME_FORMAT, '%Y-%m-%dT%H:%M:%S', settings.DATE_FORMAT, '%Y-%m-%d']:
+                try:
+                    date_time = datetime.strptime(value, date_time_fmt)
+                    break
+                except:
+                    pass
+            if date_time is None:
+                return queryset
+            date_time = pytz.timezone(settings.TIME_ZONE).localize(date_time).astimezone(pytz.utc)
+            if len(value) <= 10:
+                return queryset.filter(**{field + '__gte': date_time, field + '__lt': date_time + timedelta(days=1)})
+            return queryset.filter(**{field + '__gte': date_time, field + '__lt': date_time + timedelta(seconds=1)})
         else:
-            self._help_text = value
-            self._help_text_form = getattr(self, '_help_text_form', None) or value
+            if isinstance(model_meta.get_field(field), models.BooleanField):
+                value = (value == 'true')
+            return queryset.filter(**{field: value})
 
-    def get_help_text_form(self):
-        return self._help_text_form
+    @staticmethod
+    def generate_paged_loader(page_size: int = 30, ordering: Union[str, List[str]] = 'id'):
+        """
+        Generates a Pagination class that will handle dynamic data loading for ViewSets with a lot of data.
+        Use by declaring `pagination_class = ModelViewSet.generate_paged_loader()` in class variables
 
-    def set_help_text_form(self, value):
-        if isinstance(value, dict):
-            self._help_text = value.get('form', None)
-        else:
-            self._help_text_form = value
+        :param page_size: how many records should be fetched at a time
+        :param ordering: This should be a string, or list of strings, indicating the field against which the cursor
+           based pagination will be applied. For example: ordering = 'slug'
+        :return: a Pagination class
+        """
+        from rest_framework.pagination import CursorPagination
+        ps = page_size
+        ordr = ordering
+
+        class MyCursorPagination(CursorPagination):
+            ordering = ordr
+            page_size = ps
+            df_request = None
+
+            def paginate_queryset(self, queryset, request, view=None):
+                self.df_request = request
+                return super().paginate_queryset(queryset, request, view=None)
+
+            def encode_cursor(self, cursor):
+                # Following code is needed when we have https proxy server that redirects requests to http servers.
+                # In that case original code generates cursor links that have http scheme.
+                # So here I check REFERER header to find out which scheme is originally declared.
+                # And use that one in cursor link.
+                request = getattr(self, 'df_request', None)
+                cursor_url = super().encode_cursor(cursor).split(':', 1)
+                req_url = self.df_request.META.get('HTTP_REFERER', None)
+                if req_url:
+                    req_url = req_url.split(':', 1)
+                    if cursor_url[0] != req_url[0] and req_url[0].lower() in ('http', 'https'):
+                        cursor_url[0] = req_url[0]
+                cursor_url = ':'.join(cursor_url)
+                if request and isinstance(request.accepted_renderer, JSONRenderer):
+                    cursor_url += '&x_df_pagination=1'
+                return cursor_url
+
+        return MyCursorPagination
+
+    def handle_create_validation_exception(self, e, request, *args, **kwargs):
+        instance = self.new_object()
+        ser = self.get_serializer(instance, data=request.data, partial=False)
+        ser.is_valid(raise_exception=False)
+        e.detail.serializer = ser
+        raise e
+
+    def create(self, request, *args, **kwargs):
+        try:
+            return super().create(request, *args, **kwargs)
+        except ValidationError as e:
+            self.handle_create_validation_exception(e, request, *args, **kwargs)
+
+
+class SingleRecordViewSet(NewMixin, TemplateRendererMixin, viewsets.GenericViewSet):
+
+    def new_object(self):
+        raise NotImplementedError()
+
+    def create(self, request, *args, **kwargs):
+        raise NotImplementedError()
 
-    help_text = property(get_help_text, set_help_text)
-    help_text_form = property(get_help_text_form, set_help_text_form)
+
+# noinspection PyUnresolvedReferences
+class GenericViewSet(NewMixin, PutPostMixin, TemplateRendererMixin, viewsets.GenericViewSet):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DynamicForms-0.9.8/dynamicforms/progress.py` & `DynamicForms-0.9.9/dynamicforms/progress.py`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/renderers.py` & `DynamicForms-0.9.9/dynamicforms/renderers.py`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/serializers.py` & `DynamicForms-0.9.9/dynamicforms/serializers.py`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/settings.py` & `DynamicForms-0.9.9/dynamicforms/settings.py`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/bootstrap-3.4.1-dist/css/bootstrap-theme.css` & `DynamicForms-0.9.9/dynamicforms/static/bootstrap-3.4.1-dist/css/bootstrap-theme.css`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/bootstrap-3.4.1-dist/css/bootstrap-theme.css.map` & `DynamicForms-0.9.9/dynamicforms/static/bootstrap-3.4.1-dist/css/bootstrap-theme.css.map`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/bootstrap-3.4.1-dist/css/bootstrap-theme.min.css` & `DynamicForms-0.9.9/dynamicforms/static/bootstrap-3.4.1-dist/css/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/bootstrap-3.4.1-dist/css/bootstrap-theme.min.css.map` & `DynamicForms-0.9.9/dynamicforms/static/bootstrap-3.4.1-dist/css/bootstrap-theme.min.css.map`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/bootstrap-3.4.1-dist/css/bootstrap.css` & `DynamicForms-0.9.9/dynamicforms/static/bootstrap-3.4.1-dist/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/bootstrap-3.4.1-dist/css/bootstrap.css.map` & `DynamicForms-0.9.9/dynamicforms/static/bootstrap-3.4.1-dist/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/bootstrap-3.4.1-dist/css/bootstrap.min.css` & `DynamicForms-0.9.9/dynamicforms/static/bootstrap-3.4.1-dist/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/bootstrap-3.4.1-dist/css/bootstrap.min.css.map` & `DynamicForms-0.9.9/dynamicforms/static/bootstrap-3.4.1-dist/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/bootstrap-3.4.1-dist/fonts/glyphicons-halflings-regular.eot` & `DynamicForms-0.9.9/dynamicforms/static/bootstrap-3.4.1-dist/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/bootstrap-3.4.1-dist/fonts/glyphicons-halflings-regular.svg` & `DynamicForms-0.9.9/dynamicforms/static/bootstrap-3.4.1-dist/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/bootstrap-3.4.1-dist/fonts/glyphicons-halflings-regular.ttf` & `DynamicForms-0.9.9/dynamicforms/static/bootstrap-3.4.1-dist/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/bootstrap-3.4.1-dist/fonts/glyphicons-halflings-regular.woff` & `DynamicForms-0.9.9/dynamicforms/static/bootstrap-3.4.1-dist/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/bootstrap-3.4.1-dist/fonts/glyphicons-halflings-regular.woff2` & `DynamicForms-0.9.9/dynamicforms/static/bootstrap-3.4.1-dist/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/bootstrap-3.4.1-dist/js/bootstrap.js` & `DynamicForms-0.9.9/dynamicforms/static/bootstrap-3.4.1-dist/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/bootstrap-3.4.1-dist/js/bootstrap.min.js` & `DynamicForms-0.9.9/dynamicforms/static/bootstrap-3.4.1-dist/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/bootstrap-4.3.1-dist/css/bootstrap-grid.css` & `DynamicForms-0.9.9/dynamicforms/static/bootstrap-4.3.1-dist/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/bootstrap-4.3.1-dist/css/bootstrap-grid.css.map` & `DynamicForms-0.9.9/dynamicforms/static/bootstrap-4.3.1-dist/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/bootstrap-4.3.1-dist/css/bootstrap-grid.min.css` & `DynamicForms-0.9.9/dynamicforms/static/bootstrap-4.3.1-dist/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/bootstrap-4.3.1-dist/css/bootstrap-grid.min.css.map` & `DynamicForms-0.9.9/dynamicforms/static/bootstrap-4.3.1-dist/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/bootstrap-4.3.1-dist/css/bootstrap-reboot.css` & `DynamicForms-0.9.9/dynamicforms/static/bootstrap-4.3.1-dist/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/bootstrap-4.3.1-dist/css/bootstrap-reboot.css.map` & `DynamicForms-0.9.9/dynamicforms/static/bootstrap-4.3.1-dist/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/bootstrap-4.3.1-dist/css/bootstrap-reboot.min.css` & `DynamicForms-0.9.9/dynamicforms/static/bootstrap-4.3.1-dist/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/bootstrap-4.3.1-dist/css/bootstrap-reboot.min.css.map` & `DynamicForms-0.9.9/dynamicforms/static/bootstrap-4.3.1-dist/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/bootstrap-4.3.1-dist/css/bootstrap.css` & `DynamicForms-0.9.9/dynamicforms/static/bootstrap-4.3.1-dist/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/bootstrap-4.3.1-dist/css/bootstrap.css.map` & `DynamicForms-0.9.9/dynamicforms/static/bootstrap-4.3.1-dist/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/bootstrap-4.3.1-dist/css/bootstrap.min.css` & `DynamicForms-0.9.9/dynamicforms/static/bootstrap-4.3.1-dist/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/bootstrap-4.3.1-dist/css/bootstrap.min.css.map` & `DynamicForms-0.9.9/dynamicforms/static/bootstrap-4.3.1-dist/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/bootstrap-4.3.1-dist/js/bootstrap.bundle.js` & `DynamicForms-0.9.9/dynamicforms/static/bootstrap-4.3.1-dist/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/bootstrap-4.3.1-dist/js/bootstrap.bundle.js.map` & `DynamicForms-0.9.9/dynamicforms/static/bootstrap-4.3.1-dist/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/bootstrap-4.3.1-dist/js/bootstrap.bundle.min.js` & `DynamicForms-0.9.9/dynamicforms/static/bootstrap-4.3.1-dist/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/bootstrap-4.3.1-dist/js/bootstrap.bundle.min.js.map` & `DynamicForms-0.9.9/dynamicforms/static/bootstrap-4.3.1-dist/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/bootstrap-4.3.1-dist/js/bootstrap.js` & `DynamicForms-0.9.9/dynamicforms/static/bootstrap-4.3.1-dist/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/bootstrap-4.3.1-dist/js/bootstrap.js.map` & `DynamicForms-0.9.9/dynamicforms/static/bootstrap-4.3.1-dist/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/bootstrap-4.3.1-dist/js/bootstrap.min.js` & `DynamicForms-0.9.9/dynamicforms/static/bootstrap-4.3.1-dist/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/bootstrap-4.3.1-dist/js/bootstrap.min.js.map` & `DynamicForms-0.9.9/dynamicforms/static/bootstrap-4.3.1-dist/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/dynamicforms/dynamicforms.js` & `DynamicForms-0.9.9/dynamicforms/static/dynamicforms/dynamicforms.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -437,14 +437,16 @@
             var hasPrevId = (typeof prevId !== typeof undefined && prevId !== false && prevId != '');
 
             if (hasPrevId) {
                 if (prevId == 'None')
                     $lastRow = $('#list-' + formID + ' > tbody > tr[data-id]').first();
                 else {
                     $lastRow = $('#list-' + formID + ' > tbody > tr[data-id="' + prevId + '"]').first(); // First row of table
+                    if ($lastRow.length == 0)
+                        console.log('Row with prevId = "' + prevId + '" not found!');
                 }
             } else if (!dynamicforms.isLinkNext(tbl_pagination.link_next))
                 $lastRow = $('#list-' + formID + ' > tbody > tr[data-id]').last(); // Last row before adding new record
             if ($lastRow != undefined && $lastRow.length) {
                 if (prevId == 'None')
                     $newRow.insertBefore($lastRow);
                 else
@@ -464,17 +466,15 @@
         var $rowToRefresh = null; // Row to refresh
         var $htmlObject = (data instanceof jQuery) ? data : $(data);
 
         if (recordID) {
             var trSelector = "tr[data-id='" + recordID + "']";
             $rowToRefresh = $('#list-' + formID + ' > tbody > ' + trSelector); // Row to refresh
             var $editedRow = $htmlObject.find("table[id^='list-'] > tbody > " + trSelector); // Edited record from ajax returned html
-        }
 
-        if (recordID) {
             if ($editedRow.length) {
                 var prevId = $editedRow.attr('data-df_prev_id');
                 var hasPrevId = (typeof prevId !== typeof undefined && prevId !== false && prevId != '');
 
                 if ($rowToRefresh != null && $rowToRefresh.length) {
                     if (hasPrevId) {
                         $rowToRefresh.remove();
```

### Comparing `DynamicForms-0.9.8/dynamicforms/static/jquery_ui/css/images/ui-bg_gloss-wave_35_f6a828_500x100.png` & `DynamicForms-0.9.9/dynamicforms/static/jquery_ui/css/images/ui-bg_gloss-wave_35_f6a828_500x100.png`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/jquery_ui/css/images/ui-icons_222222_256x240.png` & `DynamicForms-0.9.9/dynamicforms/static/jquery_ui/css/images/ui-icons_222222_256x240.png`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/jquery_ui/css/images/ui-icons_228ef1_256x240.png` & `DynamicForms-0.9.9/dynamicforms/static/jquery_ui/css/images/ui-icons_228ef1_256x240.png`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/jquery_ui/css/images/ui-icons_ef8c08_256x240.png` & `DynamicForms-0.9.9/dynamicforms/static/jquery_ui/css/images/ui-icons_ef8c08_256x240.png`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/jquery_ui/css/images/ui-icons_ffd27a_256x240.png` & `DynamicForms-0.9.9/dynamicforms/static/jquery_ui/css/images/ui-icons_ffd27a_256x240.png`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/jquery_ui/css/images/ui-icons_ffffff_256x240.png` & `DynamicForms-0.9.9/dynamicforms/static/jquery_ui/css/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/jquery_ui/css/jquery-ui.min.css` & `DynamicForms-0.9.9/dynamicforms/static/jquery_ui/css/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/jquery_ui/css/jquery-ui.structure.min.css` & `DynamicForms-0.9.9/dynamicforms/static/jquery_ui/css/jquery-ui.structure.min.css`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/jquery_ui/css/jquery-ui.theme.min.css` & `DynamicForms-0.9.9/dynamicforms/static/jquery_ui/css/jquery-ui.theme.min.css`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/jquery_ui/js/jquery-3.3.1.min.js` & `DynamicForms-0.9.9/dynamicforms/static/jquery_ui/js/jquery-3.3.1.min.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/jquery_ui/js/jquery-ui.min.js` & `DynamicForms-0.9.9/dynamicforms/static/jquery_ui/js/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/select2/css/select2-bootstrap3.min.css` & `DynamicForms-0.9.9/dynamicforms/static/select2/css/select2-bootstrap3.min.css`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/select2/css/select2-bootstrap4.min.css` & `DynamicForms-0.9.9/dynamicforms/static/select2/css/select2-bootstrap4.min.css`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/css/select2.min.css` & `DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/css/select2.min.css`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/af.js` & `DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/af.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/ar.js` & `DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/ar.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/az.js` & `DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/az.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/bg.js` & `DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/bg.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/bs.js` & `DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/bs.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/ca.js` & `DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/ca.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/cs.js` & `DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/cs.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/da.js` & `DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/da.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/de.js` & `DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/de.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/dsb.js` & `DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/dsb.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/el.js` & `DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/el.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/en.js` & `DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/en.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/es.js` & `DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/es.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/et.js` & `DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/et.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/eu.js` & `DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/eu.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/fa.js` & `DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/fa.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/fi.js` & `DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/fi.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/fr.js` & `DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/fr.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/gl.js` & `DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/gl.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/he.js` & `DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/he.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/hi.js` & `DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/hi.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/hr.js` & `DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/hr.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/hsb.js` & `DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/hsb.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/hu.js` & `DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/hu.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/hy.js` & `DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/hy.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/id.js` & `DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/id.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/is.js` & `DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/is.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/it.js` & `DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/it.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/ja.js` & `DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/ja.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/km.js` & `DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/km.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/ko.js` & `DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/ko.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/lt.js` & `DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/lt.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/lv.js` & `DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/lv.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/mk.js` & `DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/mk.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/ms.js` & `DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/ms.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/nb.js` & `DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/nb.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/nl.js` & `DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/nl.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/pl.js` & `DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/pl.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/ps.js` & `DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/ps.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/pt-BR.js` & `DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/pt-BR.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/pt.js` & `DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/pt.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/ro.js` & `DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/ro.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/ru.js` & `DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/ru.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/sk.js` & `DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/sk.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/sl.js` & `DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/sl.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/sr-Cyrl.js` & `DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/sr-Cyrl.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/sr.js` & `DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/sr.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/sv.js` & `DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/sv.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/th.js` & `DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/th.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/tr.js` & `DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/tr.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/uk.js` & `DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/uk.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/vi.js` & `DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/vi.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/zh-CN.js` & `DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/zh-CN.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/i18n/zh-TW.js` & `DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/i18n/zh-TW.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/select2.full.js` & `DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/select2.full.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/select2.full.min.js` & `DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/select2.full.min.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/select2.js` & `DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/select2.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/static/select2/select2-4.0.5/js/select2.min.js` & `DynamicForms-0.9.9/dynamicforms/static/select2/select2-4.0.5/js/select2.min.js`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/struct.py` & `DynamicForms-0.9.9/dynamicforms/struct.py`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/bootstrap/base_form.html` & `DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/bootstrap/base_form.html`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/bootstrap/base_includes_v3.html` & `DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/bootstrap/base_includes_v3.html`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/bootstrap/base_includes_v4.html` & `DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/bootstrap/base_includes_v4.html`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/bootstrap/base_list.html` & `DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/bootstrap/base_list.html`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/bootstrap/base_table_body.html` & `DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/bootstrap/base_table_body.html`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
   >
     {% render_table_commands serializer "rowstart" %}
     {% for key, column in serializer.fields.items %}
       {% if column.display_table == DYNAMICFORMS.DisplayMode.FULL or column.display_table == DYNAMICFORMS.DisplayMode.INVISIBLE %}
         {% dict_item_default var='value' d=row k=key default='' %}
         <td class="{{ column.table_classes }}{% if column.display_table == DYNAMICFORMS.DisplayMode.INVISIBLE %}d-none{% endif %}" {{ value|add_nested_class }} data-name="{{ key }}">
           {% render_table_commands serializer "fieldleft" key %}
-          {% render_field_to_table serializer key value row %}
+          {{ value }}
           {% render_table_commands serializer "fieldright" key %}
         </td>
       {% endif %}
     {% endfor %}
     {% render_table_commands serializer "rowend" %}
   </tr>
 {% empty %}
```

### Comparing `DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/bootstrap/base_table_filter.html` & `DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/bootstrap/base_table_filter.html`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/bootstrap/field/base_field_v3.html` & `DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/bootstrap/field/base_field_v3.html`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/bootstrap/field/base_field_v4.html` & `DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/bootstrap/field/base_field_v4.html`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/bootstrap/field/checkbox.html` & `DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/bootstrap/field/checkbox.html`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/bootstrap/field/checkbox_multiple.html` & `DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/bootstrap/field/checkbox_multiple.html`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/bootstrap/field/fieldset.html` & `DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/bootstrap/field/fieldset.html`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/bootstrap/field/input.html` & `DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/bootstrap/field/input.html`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/bootstrap/field/list_fieldset.html` & `DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/bootstrap/field/list_fieldset.html`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/bootstrap/field/radio.html` & `DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/bootstrap/field/radio.html`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/bootstrap/field/select.html` & `DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/bootstrap/field/select.html`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/bootstrap/field/select_multiple.html` & `DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/bootstrap/field/select_multiple.html`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/bootstrap/field/textarea.html` & `DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/bootstrap/field/textarea.html`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/bootstrap/modal_dialog_v3.html` & `DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/bootstrap/modal_dialog_v3.html`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/bootstrap/modal_dialog_v4.html` & `DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/bootstrap/modal_dialog_v4.html`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/bootstrap/page.html` & `DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/bootstrap/page.html`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/bootstrap/progress_dialog.html` & `DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/bootstrap/progress_dialog.html`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/jquery_ui/base_form.html` & `DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/jquery_ui/base_form.html`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/jquery_ui/base_includes.html` & `DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/jquery_ui/base_includes.html`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/jquery_ui/base_list.html` & `DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/jquery_ui/base_list.html`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/jquery_ui/base_table_body.html` & `DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/jquery_ui/base_table_body.html`

 * *Files 15% similar despite different names*

```diff
@@ -12,15 +12,15 @@
   >
     {% render_table_commands serializer "rowstart" %}
     {% for key, column in serializer.fields.items %}
       {% if column.display_table == DYNAMICFORMS.DisplayMode.FULL or column.display_table == DYNAMICFORMS.DisplayMode.INVISIBLE %}
         {% dict_item_default var='value' d=row k=key default='' %}
         <td {{ value|add_nested_class }}{% if column.display_table == DYNAMICFORMS.DisplayMode.INVISIBLE %} style="display: none" {% endif %} data-name="{{ key }}">
           {% render_table_commands serializer "fieldleft" key %}
-          {% render_field_to_table serializer key value row %}
+          {{ value }}
           {% render_table_commands serializer "fieldright" key %}
         </td>
       {% endif %}
     {% endfor %}
     {% render_table_commands serializer "rowend" %}
   </tr>
 {% empty %}
```

### Comparing `DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/jquery_ui/base_table_filter.html` & `DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/jquery_ui/base_table_filter.html`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/jquery_ui/field/base_field.html` & `DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/jquery_ui/field/base_field.html`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/jquery_ui/field/checkbox.html` & `DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/jquery_ui/field/checkbox.html`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/jquery_ui/field/checkbox_multiple.html` & `DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/jquery_ui/field/checkbox_multiple.html`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/jquery_ui/field/input.html` & `DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/jquery_ui/field/input.html`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/jquery_ui/field/radio.html` & `DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/jquery_ui/field/radio.html`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/jquery_ui/field/select.html` & `DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/jquery_ui/field/select.html`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/jquery_ui/field/select_multiple.html` & `DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/jquery_ui/field/select_multiple.html`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/jquery_ui/modal_dialog.html` & `DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/jquery_ui/modal_dialog.html`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/templates/dynamicforms/jquery_ui/page.html` & `DynamicForms-0.9.9/dynamicforms/templates/dynamicforms/jquery_ui/page.html`

 * *Files identical despite different names*

### Comparing `DynamicForms-0.9.8/dynamicforms/templatetags/dynamicforms.py` & `DynamicForms-0.9.9/dynamicforms/templatetags/dynamicforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,28 +106,14 @@
     :return: rendered field template
     """
     renderer = style.get('renderer', HTMLFormRenderer())
     return renderer.render_field(field, style)
 
 
 @register.simple_tag
-def render_field_to_table(serializer, field_name, value, row_data):
-    """
-    Renders separate field to table view.
-
-    :param serializer: Serializer
-    :param field_name: Field name
-    :param value: Field value
-    :param row_data: data for entire row
-    :return: rendered field for table view
-    """
-    return serializer.fields[field_name].render_to_table(value, row_data)
-
-
-@register.simple_tag
 def table_columns_count(serializer):
     """
     Returns number of columns including control columns
 
     :param serializer: Serializer
     :return: Number of all columns
     """
```

### Comparing `DynamicForms-0.9.8/setup.py` & `DynamicForms-0.9.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('README.rst', 'r') as fh:
     long_description = fh.read()
 with open('requirements.txt', 'r') as fh:
     requirements = fh.readlines()
 
 setuptools.setup(
     name="DynamicForms",
-    version="0.9.8",
+    version="0.9.9",
     author="Jure Erznožnik",
     author_email="jure@velis.si",
     description="DynamicForms performs all the visualisation & data entry of your DRF Serializers & ViewSets and adds "
                 "some candy of its own: It is a django library that gives you the power of dynamically-shown form "
                 "fields, auto-filled default values, dynamic record loading and similar candy with little effort. "
                 "To put it differently: once defined, a particular ViewSet / Serializer can be rendered in multiple "
                 "ways allowing you to perform viewing and authoring operations on the data in question.",
```

