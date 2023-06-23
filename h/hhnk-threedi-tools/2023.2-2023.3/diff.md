# Comparing `tmp/hhnk-threedi-tools-2023.2.tar.gz` & `tmp/hhnk-threedi-tools-2023.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hhnk-threedi-tools-2023.2.tar", last modified: Wed May 10 16:04:19 2023, max compression
+gzip compressed data, was "hhnk-threedi-tools-2023.3.tar", last modified: Fri Jun 23 05:21:49 2023, max compression
```

## Comparing `hhnk-threedi-tools-2023.2.tar` & `hhnk-threedi-tools-2023.3.tar`

### file list

```diff
@@ -1,123 +1,125 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 16:04:15.789337 hhnk-threedi-tools-2023.2/
--rw-rw-rw-   0        0        0      227 2021-12-20 09:07:09.000000 hhnk-threedi-tools-2023.2/MANIFEST.in
--rw-rw-rw-   0        0        0      587 2023-05-10 16:04:19.501200 hhnk-threedi-tools-2023.2/PKG-INFO
--rw-rw-rw-   0        0        0      348 2023-04-24 14:42:58.000000 hhnk-threedi-tools-2023.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 16:04:15.809337 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/
--rw-rw-rw-   0        0        0     1486 2023-05-10 09:39:42.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 16:04:15.956339 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/
--rw-rw-rw-   0        0        0       50 2021-12-13 08:25:18.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 16:04:16.127342 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/api/
--rw-rw-rw-   0        0        0        0 2021-12-13 08:25:18.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/api/__init__.py
--rw-rw-rw-   0        0        0    32989 2023-05-03 08:34:10.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/api/calculation.py
--rw-rw-rw-   0        0        0    21367 2023-05-03 08:34:10.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/api/calculation_functions.py
--rw-rw-rw-   0        0        0    82195 2023-05-10 08:00:23.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/api/calculation_gui_class.py
--rw-rw-rw-   0        0        0     2911 2023-05-03 08:34:10.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/api/download_functions.py
--rw-rw-rw-   0        0        0    57886 2023-05-10 08:00:23.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/api/download_gui_class.py
--rw-rw-rw-   0        0        0    29178 2023-05-03 08:34:10.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/api/downloader.py
--rw-rw-rw-   0        0        0      345 2022-08-26 12:20:20.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/api/read_api_file.py
-drwxrwxrwx   0        0        0        0 2023-05-10 16:04:16.305345 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/api/upload_model/
--rw-rw-rw-   0        0        0        0 2022-08-17 14:12:32.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/api/upload_model/__init__.py
--rw-rw-rw-   0        0        0      871 2022-08-26 12:20:21.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/api/upload_model/constants.py
--rw-rw-rw-   0        0        0     3036 2022-08-26 12:20:21.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/api/upload_model/download.py
--rw-rw-rw-   0        0        0      420 2022-08-26 12:20:21.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/api/upload_model/login.py
--rw-rw-rw-   0        0        0     3742 2023-04-29 07:27:21.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/api/upload_model/simulate.py
--rw-rw-rw-   0        0        0    44747 2022-08-31 12:10:25.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/api/upload_model/threedi_calls.py
--rw-rw-rw-   0        0        0    10753 2023-01-09 08:31:28.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/api/upload_model/upload.py
-drwxrwxrwx   0        0        0        0 2023-05-10 16:04:16.524348 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/checks/
--rw-rw-rw-   0        0        0        0 2021-12-13 08:25:18.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/checks/__init__.py
--rw-rw-rw-   0        0        0    29923 2023-05-09 13:00:44.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/checks/bank_levels.py
--rw-rw-rw-   0        0        0     5352 2023-05-10 08:00:23.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/checks/grid_result_metadata.py
--rw-rw-rw-   0        0        0     5587 2021-12-13 08:25:18.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/checks/model_backup.py
--rw-rw-rw-   0        0        0    16137 2023-05-03 08:34:10.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/checks/model_splitter.py
--rw-rw-rw-   0        0        0    22134 2021-12-13 08:25:18.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/checks/model_state.py
--rw-rw-rw-   0        0        0    18055 2023-05-10 08:00:23.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/checks/one_d_two_d.py
-drwxrwxrwx   0        0        0        0 2023-05-10 16:04:16.590350 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/checks/sqlite/
--rw-rw-rw-   0        0        0        0 2021-12-13 08:25:18.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/checks/sqlite/__init__.py
--rw-rw-rw-   0        0        0    33209 2023-05-10 09:34:17.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/checks/sqlite/sqlite_main.py
--rw-rw-rw-   0        0        0     7858 2023-05-09 14:45:30.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/checks/sqlite/structure_control.py
--rw-rw-rw-   0        0        0    14230 2022-08-26 12:20:21.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/checks/zero_d_one_d.py
-drwxrwxrwx   0        0        0        0 2023-05-10 16:04:16.895354 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/climate_scenarios/
--rw-rw-rw-   0        0        0        0 2022-04-12 14:08:35.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/climate_scenarios/__init__.py
--rw-rw-rw-   0        0        0     6560 2023-01-09 08:37:42.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/climate_scenarios/interpolate_rasters.py
--rw-rw-rw-   0        0        0    12065 2023-05-08 16:10:22.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/climate_scenarios/klimaatsommen_prep.py
--rw-rw-rw-   0        0        0    15484 2021-12-13 08:25:18.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/climate_scenarios/maskerkaart.py
--rw-rw-rw-   0        0        0     1851 2023-05-05 14:49:14.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/climate_scenarios/maskerkaart_raster.py
--rw-rw-rw-   0        0        0     2351 2021-12-13 08:25:18.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/climate_scenarios/peilgebieden.py
--rw-rw-rw-   0        0        0     5343 2023-05-03 08:34:10.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/climate_scenarios/ruimtekaart.py
--rw-rw-rw-   0        0        0     3239 2023-01-23 09:53:44.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/climate_scenarios/schadekaart.py
--rw-rw-rw-   0        0        0     9178 2023-05-09 13:00:44.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/climate_scenarios/schadekaart_peilgebieden.py
--rw-rw-rw-   0        0        0     6203 2023-05-10 08:00:23.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/folder_helpers.py
--rw-rw-rw-   0        0        0    26271 2023-05-10 11:23:53.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/folders.py
-drwxrwxrwx   0        0        0        0 2023-05-10 16:04:17.099357 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/resources/
--rw-rw-rw-   0        0        0    12288 2023-01-23 09:53:44.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/resources/Thumbs.db
--rw-rw-rw-   0        0        0        0 2021-12-13 08:25:18.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/resources/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 16:04:17.278360 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/resources/__pycache__/
--rw-rw-rw-   0        0        0      167 2022-07-14 07:53:38.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/resources/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0      171 2022-07-06 13:22:12.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/resources/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0    10193 2023-05-10 14:39:34.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/resources/model_settings.xlsx
--rw-rw-rw-   0        0        0     9864 2023-05-10 14:39:34.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/resources/model_settings_default.xlsx
--rw-rw-rw-   0        0        0    12764 2023-01-09 08:28:05.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/resources/precipitation_frequency.xlsx
--rw-rw-rw-   0        0        0  2080345 2021-12-13 08:25:18.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/resources/precipitation_zones_hhnk.tif
-drwxrwxrwx   0        0        0        0 2023-05-10 16:04:17.369362 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/utils/
--rw-rw-rw-   0        0        0        0 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 16:04:17.547365 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/utils/__pycache__/
--rw-rw-rw-   0        0        0      163 2022-07-14 07:53:38.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/utils/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0      167 2022-07-06 13:21:07.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/utils/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0    14142 2022-07-14 07:53:38.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/utils/__pycache__/queries.cpython-37.pyc
--rw-rw-rw-   0        0        0    15694 2022-07-06 13:21:07.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/utils/__pycache__/queries.cpython-39.pyc
--rw-rw-rw-   0        0        0    12108 2022-07-14 07:53:38.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/utils/__pycache__/queries_general_checks.cpython-37.pyc
--rw-rw-rw-   0        0        0    12291 2022-07-06 13:22:12.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/utils/__pycache__/queries_general_checks.cpython-39.pyc
-drwxrwxrwx   0        0        0        0 2023-05-10 16:04:17.894370 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/utils/notebooks/
-drwxrwxrwx   0        0        0        0 2023-05-10 16:04:18.016372 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/utils/notebooks/.ipynb_checkpoints/
--rw-rw-rw-   0        0        0     1986 2023-01-23 09:53:44.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/utils/notebooks/.ipynb_checkpoints/01_calculation_gui-checkpoint.ipynb
--rw-rw-rw-   0        0        0     5495 2023-04-11 15:21:12.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/utils/notebooks/.ipynb_checkpoints/02_download_gui-checkpoint.ipynb
--rw-rw-rw-   0        0        0     1900 2023-04-24 14:42:58.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/utils/notebooks/01_calculation_gui.ipynb
--rw-rw-rw-   0        0        0     5268 2023-05-03 12:03:29.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/utils/notebooks/02_download_gui.ipynb
--rw-rw-rw-   0        0        0    22783 2023-05-10 11:55:59.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/utils/notebooks/03_nabewerking_klimaatsommen.ipynb
--rw-rw-rw-   0        0        0     6806 2023-05-05 11:03:21.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/utils/notebooks/04_netcdf_naar_raster.ipynb
--rw-rw-rw-   0        0        0     2647 2023-05-10 09:39:49.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/utils/notebooks/05_sqlite_create_grid.ipynb
--rw-rw-rw-   0        0        0        0 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/utils/notebooks/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 16:04:18.128374 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/utils/notebooks/__pycache__/
--rw-rw-rw-   0        0        0      179 2022-01-31 10:15:01.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/utils/notebooks/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0      177 2022-06-29 11:24:40.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/utils/notebooks/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     6121 2023-04-25 11:04:59.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/utils/notebooks/__pycache__/run.cpython-37.pyc
--rw-rw-rw-   0        0        0     6212 2023-04-24 15:18:38.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/utils/notebooks/__pycache__/run.cpython-39.pyc
--rw-rw-rw-   0        0        0      308 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/utils/notebooks/constants.py
--rw-rw-rw-   0        0        0     7154 2023-04-24 14:42:59.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/utils/notebooks/run.py
--rw-rw-rw-   0        0        0     1585 2023-05-05 10:47:26.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/utils/notebooks/test.py
--rw-rw-rw-   0        0        0    20400 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/utils/queries.py
--rw-rw-rw-   0        0        0    25714 2022-03-24 14:59:34.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/utils/queries_general_checks.py
-drwxrwxrwx   0        0        0        0 2023-05-10 16:04:18.767384 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/variables/
--rw-rw-rw-   0        0        0        0 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/variables/__init__.py
--rw-rw-rw-   0        0        0     1858 2023-05-10 08:00:23.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/variables/api_settings.py
--rw-rw-rw-   0        0        0      256 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/variables/backups_table_names.py
--rw-rw-rw-   0        0        0     1043 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/variables/bank_levels.py
--rw-rw-rw-   0        0        0      303 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/variables/damo_hdb_datachecker_variables.py
--rw-rw-rw-   0        0        0     1649 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/variables/database_aliases.py
--rw-rw-rw-   0        0        0     2601 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/variables/database_variables.py
--rw-rw-rw-   0        0        0      134 2023-05-06 10:58:04.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/variables/datachecker_variables.py
--rw-rw-rw-   0        0        0      162 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/variables/default_variables.py
--rw-rw-rw-   0        0        0      130 2023-05-06 07:30:57.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/variables/definitions.py
--rw-rw-rw-   0        0        0      618 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/variables/model_state.py
--rw-rw-rw-   0        0        0      953 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/variables/one_d_two_d.py
--rw-rw-rw-   0        0        0      830 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/variables/sqlite.py
--rw-rw-rw-   0        0        0      254 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/variables/weirs.py
--rw-rw-rw-   0        0        0     1767 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools/variables/zero_d_one_d.py
-drwxrwxrwx   0        0        0        0 2023-05-10 16:04:15.899339 hhnk-threedi-tools-2023.2/hhnk_threedi_tools.egg-info/
--rw-rw-rw-   0        0        0      587 2023-05-10 16:04:15.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5026 2023-05-10 16:04:15.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 16:04:15.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-05-10 16:04:15.000000 hhnk-threedi-tools-2023.2/hhnk_threedi_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 16:04:19.531017 hhnk-threedi-tools-2023.2/setup.cfg
--rw-rw-rw-   0        0        0      943 2023-05-10 13:26:24.000000 hhnk-threedi-tools-2023.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-10 16:04:19.453395 hhnk-threedi-tools-2023.2/tests/
--rw-rw-rw-   0        0        0        0 2023-04-24 14:42:59.000000 hhnk-threedi-tools-2023.2/tests/__init__.py
--rw-rw-rw-   0        0        0      468 2023-05-10 11:12:23.000000 hhnk-threedi-tools-2023.2/tests/config.py
--rw-rw-rw-   0        0        0     1649 2023-05-09 14:38:42.000000 hhnk-threedi-tools-2023.2/tests/rtest_klimaatsommen_prep.py
--rw-rw-rw-   0        0        0      852 2023-04-24 14:43:04.000000 hhnk-threedi-tools-2023.2/tests/rtest_notebooks.py
--rw-rw-rw-   0        0        0      296 2023-04-24 15:40:50.000000 hhnk-threedi-tools-2023.2/tests/set_local_paths.py
--rw-rw-rw-   0        0        0     5355 2023-05-10 10:13:58.000000 hhnk-threedi-tools-2023.2/tests/test_bank_level_test.py
--rw-rw-rw-   0        0        0     2656 2023-05-10 11:19:49.000000 hhnk-threedi-tools-2023.2/tests/test_folder_structures.py
--rw-rw-rw-   0        0        0     2059 2023-05-10 10:08:41.000000 hhnk-threedi-tools-2023.2/tests/test_one_d_two_d.py
--rw-rw-rw-   0        0        0     4344 2023-05-10 09:59:41.000000 hhnk-threedi-tools-2023.2/tests/test_sqlite.py
--rw-rw-rw-   0        0        0     1198 2023-05-10 10:09:30.000000 hhnk-threedi-tools-2023.2/tests/test_zero_d_one_d.py
+drwxrwxrwx   0        0        0        0 2023-06-23 05:21:44.779554 hhnk-threedi-tools-2023.3/
+-rw-rw-rw-   0        0        0      245 2023-06-19 15:02:38.000000 hhnk-threedi-tools-2023.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      578 2023-06-23 05:21:49.166687 hhnk-threedi-tools-2023.3/PKG-INFO
+-rw-rw-rw-   0        0        0      349 2023-06-12 13:52:12.000000 hhnk-threedi-tools-2023.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 05:21:44.801554 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/
+-rw-rw-rw-   0        0        0     1509 2023-06-21 07:44:04.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-23 05:21:45.060558 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/
+-rw-rw-rw-   0        0        0       50 2021-12-13 08:25:18.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-23 05:21:45.247561 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/api/
+-rw-rw-rw-   0        0        0        0 2021-12-13 08:25:18.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/api/__init__.py
+-rw-rw-rw-   0        0        0    32989 2023-05-03 08:34:10.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/api/calculation.py
+-rw-rw-rw-   0        0        0    82230 2023-06-16 09:23:43.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/api/calculation_gui_class.py
+-rw-rw-rw-   0        0        0     2911 2023-05-03 08:34:10.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/api/download_functions.py
+-rw-rw-rw-   0        0        0    57886 2023-06-16 09:23:43.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/api/download_gui_class.py
+-rw-rw-rw-   0        0        0    29178 2023-05-03 08:34:10.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/api/downloader.py
+drwxrwxrwx   0        0        0        0 2023-06-23 05:21:45.455564 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/api/upload_model/
+-rw-rw-rw-   0        0        0        0 2022-08-17 14:12:32.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/api/upload_model/__init__.py
+-rw-rw-rw-   0        0        0      871 2022-08-26 12:20:21.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/api/upload_model/constants.py
+-rw-rw-rw-   0        0        0     3036 2022-08-26 12:20:21.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/api/upload_model/download.py
+-rw-rw-rw-   0        0        0      420 2022-08-26 12:20:21.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/api/upload_model/login.py
+-rw-rw-rw-   0        0        0     3742 2023-04-29 07:27:21.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/api/upload_model/simulate.py
+-rw-rw-rw-   0        0        0    44747 2022-08-31 12:10:25.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/api/upload_model/threedi_calls.py
+-rw-rw-rw-   0        0        0    10753 2023-01-09 08:31:28.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/api/upload_model/upload.py
+drwxrwxrwx   0        0        0        0 2023-06-23 05:21:45.917571 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/checks/
+-rw-rw-rw-   0        0        0        0 2021-12-13 08:25:18.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/checks/__init__.py
+-rw-rw-rw-   0        0        0    29924 2023-06-21 12:26:28.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/checks/bank_levels.py
+-rw-rw-rw-   0        0        0     5352 2023-05-10 08:00:23.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/checks/grid_result_metadata.py
+-rw-rw-rw-   0        0        0     5587 2021-12-13 08:25:18.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/checks/model_backup.py
+-rw-rw-rw-   0        0        0    13300 2023-06-21 09:41:43.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/checks/model_splitter.py
+-rw-rw-rw-   0        0        0    22134 2021-12-13 08:25:18.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/checks/model_state.py
+-rw-rw-rw-   0        0        0    17897 2023-06-21 08:08:05.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/checks/one_d_two_d.py
+drwxrwxrwx   0        0        0        0 2023-06-23 05:21:46.048573 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/checks/sqlite/
+-rw-rw-rw-   0        0        0        0 2021-12-13 08:25:18.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/checks/sqlite/__init__.py
+-rw-rw-rw-   0        0        0    32770 2023-05-26 14:59:07.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/checks/sqlite/sqlite_main.py
+-rw-rw-rw-   0        0        0     7858 2023-05-26 15:08:20.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/checks/sqlite/structure_control.py
+-rw-rw-rw-   0        0        0    14230 2022-08-26 12:20:21.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/checks/zero_d_one_d.py
+drwxrwxrwx   0        0        0        0 2023-06-23 05:21:46.337577 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/climate_scenarios/
+-rw-rw-rw-   0        0        0        0 2022-04-12 14:08:35.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/climate_scenarios/__init__.py
+-rw-rw-rw-   0        0        0     6560 2023-01-09 08:37:42.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/climate_scenarios/interpolate_rasters.py
+-rw-rw-rw-   0        0        0    11827 2023-06-21 08:08:01.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/climate_scenarios/klimaatsommen_prep.py
+-rw-rw-rw-   0        0        0    15484 2021-12-13 08:25:18.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/climate_scenarios/maskerkaart.py
+-rw-rw-rw-   0        0        0     1851 2023-05-05 14:49:14.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/climate_scenarios/maskerkaart_raster.py
+-rw-rw-rw-   0        0        0     2351 2021-12-13 08:25:18.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/climate_scenarios/peilgebieden.py
+-rw-rw-rw-   0        0        0     5343 2023-05-03 08:34:10.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/climate_scenarios/ruimtekaart.py
+-rw-rw-rw-   0        0        0     3239 2023-01-23 09:53:44.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/climate_scenarios/schadekaart.py
+-rw-rw-rw-   0        0        0     9351 2023-06-13 10:35:59.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/climate_scenarios/schadekaart_peilgebieden.py
+-rw-rw-rw-   0        0        0     6203 2023-05-10 08:00:23.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/folder_helpers.py
+-rw-rw-rw-   0        0        0    26403 2023-05-24 16:21:17.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/folders.py
+-rw-rw-rw-   0        0        0     4555 2023-06-21 06:32:41.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/migrate_schematisation.py
+drwxrwxrwx   0        0        0        0 2023-06-23 05:21:46.493580 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/result_rasters/
+-rw-rw-rw-   0        0        0        0 2023-06-13 10:35:59.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/result_rasters/__init__.py
+-rw-rw-rw-   0        0        0    10108 2023-06-13 10:35:59.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/result_rasters/calculate_raster.py
+-rw-rw-rw-   0        0        0     9480 2023-05-05 12:18:08.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/result_rasters/netcdf_to_gridgpkg.py
+drwxrwxrwx   0        0        0        0 2023-06-23 05:21:46.721583 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/resources/
+-rw-rw-rw-   0        0        0        0 2021-12-13 08:25:18.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/resources/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-23 05:21:47.012588 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/resources/__pycache__/
+-rw-rw-rw-   0        0        0      167 2022-07-14 07:53:38.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/resources/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0      171 2022-07-06 13:22:12.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/resources/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0    10193 2023-05-10 14:39:34.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/resources/model_settings.xlsx
+-rw-rw-rw-   0        0        0     9864 2023-05-10 14:39:34.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/resources/model_settings_default.xlsx
+-rw-rw-rw-   0        0        0    12764 2023-01-09 08:28:05.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/resources/precipitation_frequency.xlsx
+-rw-rw-rw-   0        0        0  2080345 2021-12-13 08:25:18.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/resources/precipitation_zones_hhnk.tif
+drwxrwxrwx   0        0        0        0 2023-06-23 05:21:47.130590 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/
+-rw-rw-rw-   0        0        0        0 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-23 05:21:47.398594 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/__pycache__/
+-rw-rw-rw-   0        0        0      163 2022-07-14 07:53:38.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0      167 2022-07-06 13:21:07.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0    14142 2022-07-14 07:53:38.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/__pycache__/queries.cpython-37.pyc
+-rw-rw-rw-   0        0        0    15694 2022-07-06 13:21:07.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/__pycache__/queries.cpython-39.pyc
+-rw-rw-rw-   0        0        0    12108 2022-07-14 07:53:38.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/__pycache__/queries_general_checks.cpython-37.pyc
+-rw-rw-rw-   0        0        0    12291 2022-07-06 13:22:12.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/__pycache__/queries_general_checks.cpython-39.pyc
+drwxrwxrwx   0        0        0        0 2023-06-23 05:21:47.934602 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/notebooks/
+drwxrwxrwx   0        0        0        0 2023-06-23 05:21:48.009603 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/notebooks/.ipynb_checkpoints/
+-rw-rw-rw-   0        0        0     1986 2023-01-23 09:53:44.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/notebooks/.ipynb_checkpoints/01_calculation_gui-checkpoint.ipynb
+-rw-rw-rw-   0        0        0     5495 2023-04-11 15:21:12.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/notebooks/.ipynb_checkpoints/02_download_gui-checkpoint.ipynb
+-rw-rw-rw-   0        0        0     1877 2023-06-21 06:32:41.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/notebooks/01_calculation_gui.ipynb
+-rw-rw-rw-   0        0        0     4791 2023-06-21 11:51:11.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/notebooks/02_download_gui.ipynb
+-rw-rw-rw-   0        0        0    22514 2023-06-21 08:03:06.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/notebooks/03_nabewerking_klimaatsommen.ipynb
+-rw-rw-rw-   0        0        0     6622 2023-06-21 07:58:12.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/notebooks/04_netcdf_naar_raster.ipynb
+-rw-rw-rw-   0        0        0     2090 2023-06-21 07:55:43.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/notebooks/05_sqlite_create_grid.ipynb
+-rw-rw-rw-   0        0        0        0 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/notebooks/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-23 05:21:48.172606 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/notebooks/__pycache__/
+-rw-rw-rw-   0        0        0      179 2022-01-31 10:15:01.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/notebooks/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0      177 2022-06-29 11:24:40.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/notebooks/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0      847 2023-06-21 10:23:54.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/notebooks/__pycache__/notebook_setup.cpython-39.pyc
+-rw-rw-rw-   0        0        0     6121 2023-04-25 11:04:59.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/notebooks/__pycache__/run.cpython-37.pyc
+-rw-rw-rw-   0        0        0     6291 2023-06-21 06:54:36.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/notebooks/__pycache__/run.cpython-39.pyc
+-rw-rw-rw-   0        0        0      308 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/notebooks/constants.py
+-rw-rw-rw-   0        0        0      456 2023-06-21 08:09:29.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/notebooks/notebook_data.json
+-rw-rw-rw-   0        0        0      595 2023-06-21 10:23:46.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/notebooks/notebook_setup.py
+-rw-rw-rw-   0        0        0     7404 2023-06-21 06:32:41.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/notebooks/run.py
+-rw-rw-rw-   0        0        0    20400 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/queries.py
+-rw-rw-rw-   0        0        0    25714 2022-03-24 14:59:34.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/queries_general_checks.py
+drwxrwxrwx   0        0        0        0 2023-06-23 05:21:44.717553 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/variables/
+-rw-rw-rw-   0        0        0        0 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/variables/__init__.py
+-rw-rw-rw-   0        0        0     1858 2023-05-10 08:00:23.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/variables/api_settings.py
+-rw-rw-rw-   0        0        0      256 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/variables/backups_table_names.py
+-rw-rw-rw-   0        0        0     1043 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/variables/bank_levels.py
+-rw-rw-rw-   0        0        0      303 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/variables/damo_hdb_datachecker_variables.py
+-rw-rw-rw-   0        0        0     1649 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/variables/database_aliases.py
+-rw-rw-rw-   0        0        0     2601 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/variables/database_variables.py
+-rw-rw-rw-   0        0        0      134 2023-05-06 10:58:04.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/variables/datachecker_variables.py
+-rw-rw-rw-   0        0        0      162 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/variables/default_variables.py
+-rw-rw-rw-   0        0        0      130 2023-05-06 07:30:57.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/variables/definitions.py
+-rw-rw-rw-   0        0        0      618 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/variables/model_state.py
+-rw-rw-rw-   0        0        0      953 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/variables/one_d_two_d.py
+-rw-rw-rw-   0        0        0      830 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/variables/sqlite.py
+-rw-rw-rw-   0        0        0      254 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/variables/weirs.py
+-rw-rw-rw-   0        0        0     1767 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/variables/zero_d_one_d.py
+drwxrwxrwx   0        0        0        0 2023-06-23 05:21:44.928556 hhnk-threedi-tools-2023.3/hhnk_threedi_tools.egg-info/
+-rw-rw-rw-   0        0        0      578 2023-06-23 05:21:44.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5227 2023-06-23 05:21:44.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 05:21:44.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-06-23 05:21:44.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-23 05:21:49.182115 hhnk-threedi-tools-2023.3/setup.cfg
+-rw-rw-rw-   0        0        0     1659 2023-06-21 07:43:33.000000 hhnk-threedi-tools-2023.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 05:21:49.136620 hhnk-threedi-tools-2023.3/tests/
+-rw-rw-rw-   0        0        0     4361 2023-06-21 12:30:22.000000 hhnk-threedi-tools-2023.3/tests/test_bank_level_check.py
+-rw-rw-rw-   0        0        0     2661 2023-06-14 13:34:27.000000 hhnk-threedi-tools-2023.3/tests/test_folder_structures.py
+-rw-rw-rw-   0        0        0     2098 2023-06-21 08:04:34.000000 hhnk-threedi-tools-2023.3/tests/test_klimaatsommen_prep.py
+-rw-rw-rw-   0        0        0     1843 2023-06-21 08:04:56.000000 hhnk-threedi-tools-2023.3/tests/test_one_d_two_d.py
+-rw-rw-rw-   0        0        0     2095 2023-06-21 08:05:17.000000 hhnk-threedi-tools-2023.3/tests/test_result_rasters.py
+-rw-rw-rw-   0        0        0     1147 2023-06-21 08:07:12.000000 hhnk-threedi-tools-2023.3/tests/test_schema_migration.py
+-rw-rw-rw-   0        0        0     3288 2023-06-21 08:05:53.000000 hhnk-threedi-tools-2023.3/tests/test_sqlite.py
+-rw-rw-rw-   0        0        0      977 2023-06-21 08:06:10.000000 hhnk-threedi-tools-2023.3/tests/test_zero_d_one_d.py
```

### Comparing `hhnk-threedi-tools-2023.2/PKG-INFO` & `hhnk-threedi-tools-2023.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: hhnk-threedi-tools
-Version: 2023.2
+Version: 2023.3
 Summary: HHNK watersystemen analysis tools
 Home-page: https://github.com/threedi/hhnk-threedi-tools
 Author: Wietse van Gerwen, Laure Ravier
 Author-email: w.vangerwen@hhnk.nl
 Maintainer: Wietse van Gerwen
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/threedi/hhnk-threedi-tools/issues
-Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
+
+UNKNOWN
+
```

### Comparing `hhnk-threedi-tools-2023.2/hhnk_threedi_tools/__init__.py` & `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,25 +9,23 @@
 from hhnk_threedi_tools.core.folders import Folders
 
 
 import hhnk_threedi_tools.core
 import hhnk_threedi_tools.resources
 
 
-#api
-from hhnk_threedi_tools.core.api.read_api_file import read_api_file
 
 # tests
 from hhnk_threedi_tools.core.checks.bank_levels import (
     BankLevelTest,
 )  # FIXME TypeError: metaclass conflict: the metaclass of a derived class must be a (non-strict) subclass of the metaclasses of all its bases
 from hhnk_threedi_tools.core.checks.one_d_two_d import OneDTwoDTest
 from hhnk_threedi_tools.core.checks.sqlite.sqlite_main import SqliteCheck  # FIXME
 from hhnk_threedi_tools.core.checks.zero_d_one_d import ZeroDOneDTest
-
+from hhnk_threedi_tools.core.migrate_schematisation import MigrateSchema
 
 # notebooks
 from hhnk_threedi_tools.utils.notebooks.run import add_notebook_paths
 from hhnk_threedi_tools.utils.notebooks.run import write_notebook_json
 from hhnk_threedi_tools.utils.notebooks.run import read_notebook_json
 from hhnk_threedi_tools.utils.notebooks.run import open_server
 from hhnk_threedi_tools.utils.notebooks.run import copy_notebooks
@@ -35,7 +33,10 @@
 
 # backup
 from hhnk_threedi_tools.core.checks.model_backup import (
     create_backups,
     select_values_to_update_from_backup,
     update_bank_levels_last_calc,
 )
+
+
+__version__ = '2023.3'
```

### Comparing `hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/api/calculation.py` & `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/api/calculation.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/api/calculation_gui_class.py` & `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/api/calculation_gui_class.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 # threedi
 # from threedi_scenario_downloader import downloader as dl
 from hhnk_threedi_tools.core.api import downloader as dl
 
 # local imports
 import hhnk_threedi_tools as htt
+import hhnk_research_tools as hrt
 from hhnk_threedi_tools import Folders
 
 from hhnk_threedi_tools.core.api.calculation import Simulation
 
 # Globals
 from hhnk_threedi_tools.variables.api_settings import (
     RAIN_SETTINGS,
@@ -1162,15 +1163,15 @@
         contracts = self.sim.threedi_api.contracts_list().results
         self.vars.contracts = {}
         for con in contracts:
             self.vars.contracts[con.organisation_name] = con
 
 
     def update_api_keys(self, api_keys_path):
-        self.vars.api_keys = htt.read_api_file(api_keys_path)
+        self.vars.api_keys = hrt.read_api_file(api_keys_path)
         self.login.lizard_apikey_widget.value=self.vars.api_keys["lizard"]
         self.login.threedi_apikey_widget.value=self.vars.api_keys["threedi"]
         self.login.button.click()
 
 
     def update_organisations(self):
         self.model.organisation_box.options = self.vars.organisations_viewlist
```

### Comparing `hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/api/download_functions.py` & `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/api/download_functions.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/api/download_gui_class.py` & `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/api/download_gui_class.py`

 * *Files 0% similar despite different names*

```diff
@@ -1070,15 +1070,15 @@
         # else:
         self.download_batch.dem_path_dropdown.options = [
             self.vars.folder.model.schema_base.rasters.dem.path
         ]
 
 
     def update_api_keys(self, api_keys_path):
-        self.vars.api_keys = htt.read_api_file(api_keys_path)
+        self.vars.api_keys = hrt.read_api_file(api_keys_path)
         self.login.lizard_apikey_widget.value=self.vars.api_keys["lizard"]
         # self.login.threedi_apikey_widget.value=self.vars.api_keys["threedi"]
         # self.login.button.click()
 
     @property
     def button_codes(self):
         """Map buttons to scenario result code on lizard"""
```

### Comparing `hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/api/downloader.py` & `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/api/downloader.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/api/upload_model/constants.py` & `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/api/upload_model/constants.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/api/upload_model/download.py` & `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/api/upload_model/download.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/api/upload_model/simulate.py` & `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/api/upload_model/simulate.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/api/upload_model/threedi_calls.py` & `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/api/upload_model/threedi_calls.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/api/upload_model/upload.py` & `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/api/upload_model/upload.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/checks/bank_levels.py` & `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/checks/bank_levels.py`

 * *Files 1% similar despite different names*

```diff
@@ -419,18 +419,20 @@
 
 def get_manholes_to_add_to_model(all_manholes):
     """
     Creates dataframe of new manholes to be added to model, formatted for insertion into the model
     """
     try:
         # Nodes with no manhole id need new manholes. Do not create manhole at fixeddrainage.
+
         new_manholes_df = all_manholes[
             (all_manholes[a_man_id].isna())
             & (all_manholes[type_col] != one_d_two_d_crosses_fixed)
         ].drop(df_geo_col, axis=1)
+
         new_manholes_for_model = dataframe_from_new_manholes(new_manholes_df)
         return new_manholes_for_model
     except Exception as e:
         raise e from None
 
 
 def intersections_1d2d(
@@ -559,21 +561,19 @@
         )
         new_manholes_model_df[code_col] = new_manholes_model_df[display_name_col]
         new_manholes_model_df[conn_node_id_col] = new_manholes[a_man_conn_id]
         new_manholes_model_df[shape_col] = "00"
         new_manholes_model_df[width_col] = 1
         new_manholes_model_df[manhole_indicator_col] = 0
         new_manholes_model_df[calculation_type_col] = np.where(
-            np.isnan(new_manholes[drain_level_col]), 1, 2
-        )
-        new_manholes_model_df[drain_level_col] = np.where(
-            np.isnan(new_manholes[drain_level_col]),
-            "null",
-            new_manholes[drain_level_col],
+            new_manholes[drain_level_col].isna(), 1, 2
         )
+        new_manholes_model_df[drain_level_col] = new_manholes[drain_level_col]
+        new_manholes_model_df.loc[new_manholes_model_df[drain_level_col].isna(), drain_level_col] = "null"
+
         new_manholes_model_df[bottom_lvl_col] = -10
         new_manholes_model_df[surface_lvl_col] = new_manholes[initial_waterlevel_col]
         new_manholes_model_df[zoom_cat_col] = 0
         new_manholes_model_df.set_index(conn_node_id_col)
         new_manholes_model_df[storage_area_col] = new_manholes[storage_area_col]
         # Add new storage area column where appropriate
         new_manholes_model_df.insert(
```

### Comparing `hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/checks/grid_result_metadata.py` & `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/checks/grid_result_metadata.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/checks/model_backup.py` & `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/checks/model_backup.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/checks/model_state.py` & `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/checks/model_state.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/checks/one_d_two_d.py` & `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/checks/one_d_two_d.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,9 @@
 # %%
 # -*- coding: utf-8 -*-
-"""
-Created on Mon Aug 23 11:27:51 2021
-
-@author: chris.kerklaan
-"""
-
-# if __name__ == "__main__":
-#     import set_local_paths  # add local git repos.
-
 # Third-party imports
 import os
 import numpy as np
 import pandas as pd
 import geopandas as gpd
 from shapely.geometry import box
 from shapely.geometry import LineString
@@ -64,17 +55,19 @@
 
 # TODO functies weer in class onderbrengen, class nu buiten gebruik.
 class OneDTwoDTest:
     def __init__(self, folder: Folders, revision=0, dem_path=None):
         self.fenv = folder
         self.revision = revision
 
+
         self.result_fd = self.fenv.threedi_results.one_d_two_d[self.revision]
         self.output_fd = self.fenv.output.one_d_two_d[self.revision]
 
+
         self.grid_result = self.result_fd.grid
 
         (
             rain,
             detected_rain,
             timestep,
             days_dry_start,
```

### Comparing `hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/checks/sqlite/sqlite_main.py` & `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/checks/sqlite/sqlite_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,15 +161,15 @@
         self.results = {}
 
 
     def run_controlled_structures(self, overwrite=False):
         """Create leayer with structure control in schematisation"""
         self.structure_control = StructureControl(model=self.fenv.model.schema_base.database, 
                             hdb_control_layer=self.fenv.source_data.hdb.layers.sturing_3di,
-                            output_file=self.fenv.output.sqlite_tests.gestuurde_kunstwerken.pl)
+                            output_file=self.output_fd.gestuurde_kunstwerken.pl)
         self.structure_control.run(overwrite=overwrite)
 
 
     def run_dem_max_value(self):
         try:
             stats = self.dem.statistics(approve_ok=False, force=True)
             if stats['max'] > DEM_MAX_VALUE:
@@ -373,28 +373,14 @@
         """
         Checks whether the reference level of any of the adjacent cross section locations (channels) to a structure
         is lower than the reference level for that structure (3di crashes if it is)
         """
         datachecker_culvert_layer = self.fenv.source_data.datachecker.layers.culvert
         damo_duiker_sifon_layer = self.fenv.source_data.damo.layers.DuikerSifonHevel
 
-
-        import csv
-
-        # open the file in the write mode
-        with open(r'E:\02.modellen\model_test_v2\t.txt', 'w') as f:
-            # create the csv writer
-            writer = csv.writer(f)
-
-            # write a row to the csv file
-            writer.writerow([f"{self.fenv.source_data}"])
-            writer.writerow([f"{datachecker_culvert_layer.parent}"])
-            writer.writerow([f"{damo_duiker_sifon_layer.parent}"])
-
-
         try:
             below_ref_query = struct_channel_bed_query
             gdf_below_ref = self.model.execute_sql_selection(query=below_ref_query)
             gdf_below_ref.rename(columns={'id':a_chan_bed_struct_id},inplace=True)
 
             # See git issue about below statements
             gdf_with_damo = add_damo_info(layer=damo_duiker_sifon_layer, gdf=gdf_below_ref
@@ -410,19 +396,21 @@
             self.results["struct_channel_bed_level"] = gdf_with_datacheck
             return gdf_with_datacheck
         except Exception as e:
             raise e from None
 
     def run_watersurface_area(self):
         """
-        Deze test controleert per peilgebied in het model hoe groot het gebied is dat het oppervlaktewater beslaat in het
-        model. Dit totaal is opgebouwd uit de ```storage_area``` uit de ```v2_connection_nodes``` tafel opgeteld bij het
-        oppervlak van de watergangen (uitgelezen uit de ```channel_surface_from_profiles```) shapefile. Vervolgens worden de
-        totalen per peilgebied vergeleken met diezelfde totalen uit de DAMO database.
-
+        Deze test controleert per peilgebied in het model hoe groot het gebied 
+        is dat het oppervlaktewater beslaat in het model. Dit totaal is opgebouwd 
+        uit de kolom `storage_area` uit de `v2_connection_nodes` in de sqlite opgeteld
+        bij het oppervlak van de watergangen (uitgelezen uit `channel_surface_from_profiles`)
+        shapefile. Vervolgens worden de totalen per peilgebied vergeleken met diezelfde
+        totalen uit de waterdelen in DAMO.
+        
         De kolom namen in het resultaat zijn als volgt:
         From v2_connection_nodes -> area_nodes_m2
         From channel_surface_from_profiles -> area_channels_m2
         From DAMO -> area_waterdeel_m2
         """
 
         try:
```

### Comparing `hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/checks/sqlite/structure_control.py` & `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/checks/sqlite/structure_control.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/checks/zero_d_one_d.py` & `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/checks/zero_d_one_d.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/climate_scenarios/interpolate_rasters.py` & `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/climate_scenarios/interpolate_rasters.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/climate_scenarios/klimaatsommen_prep.py` & `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/climate_scenarios/klimaatsommen_prep.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,49 +1,36 @@
 # %%
 import os
-import json
-try:
-    with open(os.getcwd() + "/notebook_data.json") as f:
-        notebook_data = json.load(f)
-except:
-    pass
 from hhnk_threedi_tools import Folders
 import pandas as pd
 import geopandas as gpd
-from osgeo import gdal
 import hhnk_research_tools as hrt
 from hhnk_threedi_tools.core.result_rasters.netcdf_to_gridgpkg import ThreediGrid
 from hhnk_threedi_tools.core.result_rasters.calculate_raster import BaseCalculatorGPKG
-import zipfile
 
 import sys
 from pathlib import Path
 
 class KlimaatsommenPrep:
     """Postprocessing of climate scenarios. This object will turn the 
     raw netcdf results into depth and damage rasters for each scenario. 
     """
     def __init__(
         self,
         folder: Folders,
         batch_name: str,
-        cfg_file:Path = None,
+        cfg_file = "cfg_lizard.cfg",
         landuse_file:str = r"\\corp.hhnk.nl\data\Hydrologen_data\Data\01.basisgegevens\rasters\landgebruik\landuse2019_tiles\combined_rasters.vrt",
-        SCHADESCHATTER_PATH:Path=Path(r"E:\01.basisgegevens\hhnk_schadeschatter"), #TODO naar een localsettings oid verplaatsen?
         verify=True,
     ):
-
-        #Schadeschatter import pas na aanroepen class
-        if str(SCHADESCHATTER_PATH) not in sys.path:
-            sys.path.insert(1, str(SCHADESCHATTER_PATH))
-        import hhnk_schadeschatter as hhnk_wss
-        self.hhnk_wss = hhnk_wss
-        if cfg_file is None:
-            cfg_file = SCHADESCHATTER_PATH/'01_data/cfg/cfg_lizard.cfg'
-
+        if type(cfg_file) == str:
+            cfg_file = hrt.get_pkg_resource_path(package_resource=hrt.waterschadeschatter.resources, 
+                                name=cfg_file)
+            if not os.path.exists(cfg_file):
+                raise Exception(f"{cfg_file} doesnt exist.")            
 
         self.folder = folder
         self.batch_fd = self.folder.threedi_results.batch[batch_name]
 
         self.cfg_file = cfg_file
         self.landuse_file = landuse_file
         
@@ -180,25 +167,25 @@
                             'cfg_file':self.cfg_file,
                             'dmg_type':'gem'}
 
             if output_raster.exists and not overwrite:
                 return
 
             #Calculation
-            wss = self.hhnk_wss.Waterschadeschatter(depth_file=depth_file.path, 
+            wss = hrt.Waterschadeschatter(depth_file=depth_file.path, 
                                     landuse_file=self.landuse_file, 
                                     wss_settings=wss_settings)
 
             # Berekenen schaderaster
             wss.run(output_raster=output_raster, 
                     calculation_type="sum",
                     overwrite=overwrite)
 
 
-    def run(self, gridgpkg=True, depth=True, dmg=True, wlvl=False, overwrite=False):
+    def run(self, gridgpkg=True, depth=True, dmg=True, wlvl=False, overwrite=False, testing=False):
         try:
             self.dem = self.get_dem()
 
             for name in self.batch_fd.downloads.names:
                 scenario = self.get_scenario(name=name)
                 threedi_result = scenario.netcdf
 
@@ -223,20 +210,25 @@
 
                 #Waterlevelraster berekenen
                 if wlvl:
                     self.calculate_wlvl(scenario=scenario,
                                             threedi_result=threedi_result, 
                                             overwrite=overwrite)
 
-            self.create_scenario_metadata(overwrite=overwrite)
+
+                if testing:
+                    #For pytests we dont need to run this 18 times
+                    break
+
+            self.create_scenario_metadata(overwrite=overwrite, testing=testing)
         except Exception as e:
             raise e from None
 
 
-    def create_scenario_metadata(self, overwrite=False):
+    def create_scenario_metadata(self, overwrite=False, testing=False):
         """Metadata of all scenarios together. """
         #TODO create checks on a result if they make sense 
         #e.g. total volume of scenarios should be higher with more precip.
         #Also bounds should be same.
         
         self.info_file = {}
 
@@ -250,14 +242,18 @@
                 scenario = self.get_scenario(name=name)
 
                 info_row = self._scenario_metadata_row(scenario=scenario,
                                                         raster_type=raster_type)
                 #Add row to df
                 info_df = info_df.append(info_row, ignore_index=True)
 
+                if testing:
+                    #For pytests we dont need to run this 18 times
+                    break
+
             #Write to file
 
             info_df.set_index(['filename'], inplace=True)
             info_df.to_csv(self.info_file[raster_type], sep=';')
         
 
     def _scenario_metadata_row(self, scenario, raster_type) -> pd.Series:
@@ -285,17 +281,15 @@
     from pathlib import Path
     from hhnk_threedi_tools import Folders
 
     # TEST_MODEL = Path(__file__).parent.parent.parent.parent / "tests/data/model_test/"
     TEST_MODEL = r"E:\02.modellen\model_test_v2"
     folder = Folders(TEST_MODEL)
 
-    SCHADESCHATTER_PATH=Path(r"E:\01.basisgegevens\hhnk_schadeschatter") #TODO naar een localsettings oid verplaatsen?
-
     self = KlimaatsommenPrep(folder=folder,
         batch_name="batch_test2",
-        cfg_file = SCHADESCHATTER_PATH/'01_data/cfg/cfg_lizard.cfg',
+        cfg_file = 'cfg_lizard.cfg',
         landuse_file = r"\\corp.hhnk.nl\data\Hydrologen_data\Data\01.basisgegevens\rasters\landgebruik\landuse2019_tiles\combined_rasters.vrt",
-        SCHADESCHATTER_PATH=SCHADESCHATTER_PATH
+        verify=True
     )
 
     self.run(overwrite=False)
```

### Comparing `hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/climate_scenarios/maskerkaart.py` & `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/climate_scenarios/maskerkaart.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/climate_scenarios/maskerkaart_raster.py` & `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/climate_scenarios/maskerkaart_raster.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/climate_scenarios/peilgebieden.py` & `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/climate_scenarios/peilgebieden.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/climate_scenarios/ruimtekaart.py` & `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/climate_scenarios/ruimtekaart.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/climate_scenarios/schadekaart.py` & `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/climate_scenarios/schadekaart.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/climate_scenarios/schadekaart_peilgebieden.py` & `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/climate_scenarios/schadekaart_peilgebieden.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,16 @@
-import numpy as np
-import multiprocessing as mp
-
 # Third-party imports
+import numpy as np
 import shapely.geometry
 import geopandas as gpd
-from osgeo import gdal
 
 # Local imports
 import hhnk_research_tools as hrt
-import hhnk_threedi_tools as htt
-from deprecated.core.climate_results.processes import multiprocess
-from tqdm.notebook import trange, tqdm
+# from deprecated.core.climate_results.processes import multiprocess
+from tqdm.notebook import trange
 
 
 def maak_schade_polygon(
     peilgebiedenbestand,
     schade_raster_file,
     pixel_factor,
     output_schade_file,
@@ -114,134 +110,134 @@
 
     # Opslaan naar shapefile en csv
     schades.to_file(output_schade_file)
     schade_per_polder.to_csv(output_polder_file)
     return schades, schade_per_polder
 
 
-def bereken_schade_per_peilgebied_parallel(idx, row, pixel_factor, meta, boundingbox):
-    """sommeer de schadewaarden per peilgebied"""
-    #     # Maak een masker per polygon
-    #     try:
-    #         poly = row.geometry.intersection(boundingbox)
-    #     except:
-    #         poly = shapely.geometry.Polygon(row.geometry.exterior).intersection(boundingbox)
-
-    #     poly_gdf = gpd.GeoDataFrame(geometry=[poly])
-    #     #Voeg kolom toe aan gdf, deze waarden worden in het raster gezet.
-    #     poly_gdf['val']=1
-
-    #     print('{} peilgebied_raster_maken'.format(idx))
-    #     #Maak raster masker van het geselecteerde peilgebied.
-    #     mask_peilgebied = wsa.polygon_to_raster(polygon_gdf=poly_gdf, valuefield='val', raster_output_path='', nodata=0,
-    #                                  meta=meta, epsg=28992, driver='MEM', datatype=gdal.GDT_Byte)
-
-    # bereken gesommeerde schade per peilgebied
-    schade_peilgebied = {}
-    for schade_type in ["overlast", "plas"]:
-        schade_peilgebied[schade_type] = (
-            np.nansum(contante_schade[schade_type][peilgebied_array == idx])
-            * pixel_factor
-        )
-    return (idx, schade_peilgebied)
-
-
-def maak_schade_polygon_parallel(
-    peilgebiedenbestand,
-    schade_raster_file,
-    pixel_factor,
-    output_schade_file,
-    output_polder_file,
-):
-    """Aggregeer de schaderasters van overlast en plasvorming naar peilgebiedniveau."""
-
-    # --------------------------------------------------------------
-    # importeer schaderasters
-    global contante_schade
-    contante_schade = {}
-    for schade_type in ["overlast", "plas"]:
-        raster = hrt.Raster(schade_raster_file[schade_type])
-        nodata = raster.nodata
-        meta = raster.metadata
-        contante_schade[schade_type] = raster.get_array()
-        contante_schade[schade_type][contante_schade[schade_type] == nodata] = 0
-
-    # Importeer peilgebieden
-    # gaf een fout: TopologyException: Input geom 0 is invalid: Too few points in geometry component
-    # at or near point 103946.02710008621 502783.65950012207 at 103946.02710008621 502783.65950012207
-    # Op deze coordinaten zat een heel klein polygon zonder peil en met opmerking dat het een heel kleine polygon was, deze is verwijderd
-    # dit kan vaker voorkomen doordat er fouten zitten in de peilgebieden bestanden
-    # oplossing: coordinaten in GIS opzoeken en fouten lijnen of hele kleine peilgebieden verwijderen
-    peilgebieden = gpd.read_file(peilgebiedenbestand)
-    peilgebieden["geometry"] = peilgebieden.buffer(0)
-
-    # Selecteer de peilgebieden die intersecten met de bounding box van de rasters
-    boundingbox = shapely.geometry.box(*meta["bounds"])
-    peilgebieden = peilgebieden.loc[peilgebieden.intersects(boundingbox)]
-
-    global peilgebied_array
-    # rasterize peilgebieden
-    peilgebieden["val"] = peilgebieden.index
-    peilgebied_array = hrt.gdf_to_raster(
-        peilgebieden,
-        value_field="val",
-        raster_out="",
-        nodata=255,
-        metadata=meta,
-        epsg=28992,
-        driver="MEM",
-        datatype=gdal.GDT_Int16,
-    )
-
-    # #Bereken de schade per peilgebied
-    results = multiprocess(
-        df=peilgebieden,
-        target_function=bereken_schade_per_peilgebied_parallel,
-        processes=mp.cpu_count() - 1,
-        pixel_factor=pixel_factor,
-        meta=meta,
-        boundingbox=boundingbox,
-    )
-    # De resulaten staan in random volgorde van berekenen. Omdat per resultaat ook de index meegegeven is, kan dit
-    # terug gezet worden in de originele gdf
-    peilgebied_schade = peilgebieden.copy()
-    for idx, schade_peilgebied in results:
-        for schade_type in ["overlast", "plas"]:
-            peilgebied_schade.loc[
-                idx, "cw_schade_{}".format(schade_type)
-            ] = schade_peilgebied[schade_type]
-
-    # #Tabel opschonen
-    schades = peilgebied_schade[
-        [
-            "id",
-            "peil_id",
-            "code",
-            "name",
-            "cw_schade_overlast",
-            "cw_schade_plas",
-            "geometry",
-        ]
-    ].sort_values(by="cw_schade_overlast", ascending=False)
-
-    schades.columns = [
-        i.replace("schade_overlast", "ws").replace("schade_plas", "mv")
-        for i in schades.columns
-    ]
-    schades["cw_tot"] = schades["cw_ws"] + schades["cw_mv"]
-
-    schades = schades.loc[schades["cw_tot"] > 0.0]
-
-    schade_per_polder = (
-        schades[["name", "cw_tot", "cw_ws", "cw_mv"]]
-        .groupby("name")
-        .sum()
-        .sort_values(by="cw_ws", ascending=False)
-    )
-
-    # Opslaan naar shapefile en csv
-    schades.to_file(output_schade_file)
-    schade_per_polder.to_csv(output_polder_file)
+# def bereken_schade_per_peilgebied_parallel(idx, row, pixel_factor, meta, boundingbox):
+#     """sommeer de schadewaarden per peilgebied"""
+#     #     # Maak een masker per polygon
+#     #     try:
+#     #         poly = row.geometry.intersection(boundingbox)
+#     #     except:
+#     #         poly = shapely.geometry.Polygon(row.geometry.exterior).intersection(boundingbox)
+
+#     #     poly_gdf = gpd.GeoDataFrame(geometry=[poly])
+#     #     #Voeg kolom toe aan gdf, deze waarden worden in het raster gezet.
+#     #     poly_gdf['val']=1
+
+#     #     print('{} peilgebied_raster_maken'.format(idx))
+#     #     #Maak raster masker van het geselecteerde peilgebied.
+#     #     mask_peilgebied = wsa.polygon_to_raster(polygon_gdf=poly_gdf, valuefield='val', raster_output_path='', nodata=0,
+#     #                                  meta=meta, epsg=28992, driver='MEM', datatype=gdal.GDT_Byte)
+
+#     # bereken gesommeerde schade per peilgebied
+#     schade_peilgebied = {}
+#     for schade_type in ["overlast", "plas"]:
+#         schade_peilgebied[schade_type] = (
+#             np.nansum(contante_schade[schade_type][peilgebied_array == idx])
+#             * pixel_factor
+#         )
+#     return (idx, schade_peilgebied)
+
+#TODO uitfaseren of werkend maken voor windows.
+# def maak_schade_polygon_parallel(
+#     peilgebiedenbestand,
+#     schade_raster_file,
+#     pixel_factor,
+#     output_schade_file,
+#     output_polder_file,
+# ):
+#     """Aggregeer de schaderasters van overlast en plasvorming naar peilgebiedniveau."""
+
+#     # --------------------------------------------------------------
+#     # importeer schaderasters
+#     global contante_schade
+#     contante_schade = {}
+#     for schade_type in ["overlast", "plas"]:
+#         raster = hrt.Raster(schade_raster_file[schade_type])
+#         nodata = raster.nodata
+#         meta = raster.metadata
+#         contante_schade[schade_type] = raster.get_array()
+#         contante_schade[schade_type][contante_schade[schade_type] == nodata] = 0
+
+#     # Importeer peilgebieden
+#     # gaf een fout: TopologyException: Input geom 0 is invalid: Too few points in geometry component
+#     # at or near point 103946.02710008621 502783.65950012207 at 103946.02710008621 502783.65950012207
+#     # Op deze coordinaten zat een heel klein polygon zonder peil en met opmerking dat het een heel kleine polygon was, deze is verwijderd
+#     # dit kan vaker voorkomen doordat er fouten zitten in de peilgebieden bestanden
+#     # oplossing: coordinaten in GIS opzoeken en fouten lijnen of hele kleine peilgebieden verwijderen
+#     peilgebieden = gpd.read_file(peilgebiedenbestand)
+#     peilgebieden["geometry"] = peilgebieden.buffer(0)
+
+#     # Selecteer de peilgebieden die intersecten met de bounding box van de rasters
+#     boundingbox = shapely.geometry.box(*meta["bounds"])
+#     peilgebieden = peilgebieden.loc[peilgebieden.intersects(boundingbox)]
+
+#     global peilgebied_array
+#     # rasterize peilgebieden
+#     peilgebieden["val"] = peilgebieden.index
+#     peilgebied_array = hrt.gdf_to_raster(
+#         peilgebieden,
+#         value_field="val",
+#         raster_out="",
+#         nodata=255,
+#         metadata=meta,
+#         epsg=28992,
+#         driver="MEM",
+#         datatype=gdal.GDT_Int16,
+#     )
+
+#     # #Bereken de schade per peilgebied
+#     results = multiprocess(
+#         df=peilgebieden,
+#         target_function=bereken_schade_per_peilgebied_parallel,
+#         processes=mp.cpu_count() - 1,
+#         pixel_factor=pixel_factor,
+#         meta=meta,
+#         boundingbox=boundingbox,
+#     )
+#     # De resulaten staan in random volgorde van berekenen. Omdat per resultaat ook de index meegegeven is, kan dit
+#     # terug gezet worden in de originele gdf
+#     peilgebied_schade = peilgebieden.copy()
+#     for idx, schade_peilgebied in results:
+#         for schade_type in ["overlast", "plas"]:
+#             peilgebied_schade.loc[
+#                 idx, "cw_schade_{}".format(schade_type)
+#             ] = schade_peilgebied[schade_type]
+
+#     # #Tabel opschonen
+#     schades = peilgebied_schade[
+#         [
+#             "id",
+#             "peil_id",
+#             "code",
+#             "name",
+#             "cw_schade_overlast",
+#             "cw_schade_plas",
+#             "geometry",
+#         ]
+#     ].sort_values(by="cw_schade_overlast", ascending=False)
+
+#     schades.columns = [
+#         i.replace("schade_overlast", "ws").replace("schade_plas", "mv")
+#         for i in schades.columns
+#     ]
+#     schades["cw_tot"] = schades["cw_ws"] + schades["cw_mv"]
+
+#     schades = schades.loc[schades["cw_tot"] > 0.0]
+
+#     schade_per_polder = (
+#         schades[["name", "cw_tot", "cw_ws", "cw_mv"]]
+#         .groupby("name")
+#         .sum()
+#         .sort_values(by="cw_ws", ascending=False)
+#     )
+
+#     # Opslaan naar shapefile en csv
+#     schades.to_file(output_schade_file)
+#     schade_per_polder.to_csv(output_polder_file)
 
-    del contante_schade
+#     del contante_schade
 
-    return schades, schade_per_polder
+#     return schades, schade_per_polder
```

### Comparing `hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/folder_helpers.py` & `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/folder_helpers.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.2/hhnk_threedi_tools/core/folders.py` & `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/folders.py`

 * *Files 0% similar despite different names*

```diff
@@ -317,14 +317,15 @@
 
     def __init__(self, base, create):
         super().__init__(os.path.join(base, "02_schematisation"), create)
 
         self.revisions = self.ModelRevisionsParent(base=self.base, create=create)
         self.schema_base = hrt.ThreediSchematisation(base=self.base, name="00_basis", create=create)
         self.schema_list = ["schema_base"]
+        self.add_file("model_sql", "model_sql.json")
 
         if create:
             self.create_readme()
         
         self.add_file("settings", "model_settings.xlsx", ftype="file")
         self.add_file("settings_default", "model_settings_default.xlsx", ftype="file")
 
@@ -546,14 +547,16 @@
             self.add_file("geisoleerde_watergangen", "geisoleerde_watergangen.gpkg", "gpkg")
             self.add_file("gestuurde_kunstwerken", "gestuurde_kunstwerken.gpkg", "gpkg")
             self.add_file("drooglegging", "drooglegging.tif", "raster")
             self.add_file("geometry_check", "geometry_check.csv", "file")
             self.add_file("general_sqlite_checks", "general_sqlite_checks.csv", "file")
             self.add_file("overlappende_profielen", "overlappende_profielen.gpkg", "file")
             self.add_file("profielen_geen_vertex", "profielen_geen_vertex.gpkg", "file")
+            self.add_file("wateroppervlak", "wateroppervlak.gpkg", "file")
+
 
             self.add_file("streefpeil", r"/temp/streefpeil.tif", "raster")
 
     class OutputDirBankLevel(Folder):
         def __init__(self, base, create):
             super().__init__(base, create=create)
             # self.layers = Layers(os.path.join(self.base, "Layers"))
```

### Comparing `hhnk-threedi-tools-2023.2/hhnk_threedi_tools/resources/model_settings.xlsx` & `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/resources/model_settings.xlsx`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.2/hhnk_threedi_tools/resources/model_settings_default.xlsx` & `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/resources/model_settings_default.xlsx`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.2/hhnk_threedi_tools/resources/precipitation_frequency.xlsx` & `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/resources/precipitation_frequency.xlsx`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.2/hhnk_threedi_tools/resources/precipitation_zones_hhnk.tif` & `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/resources/precipitation_zones_hhnk.tif`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.2/hhnk_threedi_tools/utils/__pycache__/queries.cpython-37.pyc` & `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/__pycache__/queries.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.2/hhnk_threedi_tools/utils/__pycache__/queries.cpython-39.pyc` & `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/__pycache__/queries.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.2/hhnk_threedi_tools/utils/__pycache__/queries_general_checks.cpython-37.pyc` & `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/__pycache__/queries_general_checks.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.2/hhnk_threedi_tools/utils/__pycache__/queries_general_checks.cpython-39.pyc` & `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/__pycache__/queries_general_checks.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.2/hhnk_threedi_tools/utils/notebooks/.ipynb_checkpoints/01_calculation_gui-checkpoint.ipynb` & `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/notebooks/.ipynb_checkpoints/01_calculation_gui-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.2/hhnk_threedi_tools/utils/notebooks/.ipynb_checkpoints/02_download_gui-checkpoint.ipynb` & `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/notebooks/.ipynb_checkpoints/02_download_gui-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.2/hhnk_threedi_tools/utils/notebooks/01_calculation_gui.ipynb` & `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/notebooks/01_calculation_gui.ipynb`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.981625%*

 * *Differences: {"'cells'": "{0: {'attachments': OrderedDict()}, 1: {'source': {insert: [(0, '#Add qgis plugin "*

 * *            "deps to syspath and load notebook_data\\n'), (1, 'from notebook_setup import "*

 * *            "setup_notebook\\n'), (2, 'notebook_data = setup_notebook()\\n'), (3, '\\n')], delete: "*

 * *            '[14, 13, 4, 3, 2, 1, 0]}}}'}*

```diff
@@ -1,10 +1,11 @@
 {
     "cells": [
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {
                 "ExecuteTime": {
                     "end_time": "2021-09-09T15:04:32.766713Z",
                     "start_time": "2021-09-09T15:04:32.628077Z"
                 }
             },
@@ -23,29 +24,26 @@
                     "end_time": "2021-10-15T22:52:50.428346Z",
                     "start_time": "2021-10-15T22:52:46.818054Z"
                 },
                 "tags": []
             },
             "outputs": [],
             "source": [
-                "# imports\n",
-                "import importlib\n",
-                "import sys\n",
-                "import os\n",
-                "import json\n",
+                "#Add qgis plugin deps to syspath and load notebook_data\n",
+                "from notebook_setup import setup_notebook\n",
+                "notebook_data = setup_notebook()\n",
+                "\n",
                 "\n",
                 "# ipython imports\n",
                 "import ipywidgets as widgets\n",
                 "from IPython.display import display, HTML\n",
                 "\n",
                 "display(HTML(\"<style>.container {width:90% !important;}</style>\"))\n",
                 "%matplotlib inline\n",
                 "\n",
-                "with open(os.getcwd() + \"/notebook_data.json\") as f:\n",
-                "    notebook_data = json.load(f)\n",
                 "\n",
                 "from hhnk_threedi_tools.core.api.calculation_gui_class import StartCalculationGui\n",
                 "\n",
                 "self = StartCalculationGui(data=notebook_data)\n",
                 "\n",
                 "display(self.tab) "
             ]
```

### Comparing `hhnk-threedi-tools-2023.2/hhnk_threedi_tools/utils/notebooks/02_download_gui.ipynb` & `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/notebooks/02_download_gui.ipynb`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9780381944444445%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(0, '#Add qgis plugin deps to syspath and load "*

 * *            "notebook_data\\n'), (1, 'from notebook_setup import setup_notebook\\n'), (2, "*

 * *            "'notebook_data = setup_notebook()\\n')], delete: [10, 8, 7, 6, 5, 4, 3, 2, 1, 0]}}, "*

 * *            'delete: [4]}'}*

```diff
@@ -18,25 +18,18 @@
                 "ExecuteTime": {
                     "end_time": "2021-10-18T07:27:41.321541Z",
                     "start_time": "2021-10-18T07:27:41.025441Z"
                 }
             },
             "outputs": [],
             "source": [
-                "from threedi_scenario_downloader import downloader as dl\n",
-                "import os\n",
-                "import logging\n",
-                "import sys\n",
-                "import importlib\n",
-                "import json\n",
-                "\n",
-                "with open(os.getcwd() + \"/notebook_data.json\") as f:\n",
-                "    notebook_data = json.load(f)\n",
+                "#Add qgis plugin deps to syspath and load notebook_data\n",
+                "from notebook_setup import setup_notebook\n",
+                "notebook_data = setup_notebook()\n",
                 "\n",
-                "import ipywidgets as widgets\n",
                 "from IPython.display import display, HTML\n",
                 "\n",
                 "display(HTML(\"<style>.container {width:90% !important;}</style>\"))\n",
                 "%matplotlib inline\n",
                 "\n",
                 "# local imports\n",
                 "from hhnk_threedi_tools.core.api.download_gui_class import DownloadGui\n",
@@ -75,28 +68,14 @@
             "source": [
                 "## Downloaden van rasters voor hetzelfde model op alle tijdstappen"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2021-03-24T13:51:01.238511Z",
-                    "start_time": "2021-03-24T11:56:26.877Z"
-                }
-            },
-            "outputs": [],
-            "source": [
-                "dl.set_headers(input(\"username:\"), getpass.getpass())"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import os\n",
                 "from threedi_scenario_downloader import downloader as dl\n",
                 "import getpass\n",
                 "\n",
```

### Comparing `hhnk-threedi-tools-2023.2/hhnk_threedi_tools/utils/notebooks/03_nabewerking_klimaatsommen.ipynb` & `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/notebooks/03_nabewerking_klimaatsommen.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994607533670034%*

 * *Differences: {"'cells'": "{1: {'id': '166eb613', 'source': {insert: [(0, 'from notebook_setup import "*

 * *            "setup_notebook\\n'), (1, 'notebook_data = setup_notebook()\\n'), (2, '\\n'), (12, "*

 * *            '\'\\n\'), (30, "folder = Folders(notebook_data[\'polder_folder\'])\\n"), (33, \'# '*

 * *            'folder=Folders(r"E:\\\\02.modellen\\\\model_test_v2")\\n\')], delete: [35, 32, 14, '*

 * *            '13, 12, 11, 10, 9]}}, 7: {\'source\': {insert: [(2, "    cfg_file = '*

 * *            '\'cfg_lizard.cfg\',\\n"), (4, \'   […]*

```diff
@@ -16,33 +16,31 @@
                 "Dit laatste is van belang wanneer meerdere polders in \u00e9\u00e9n poldercluster gezamelijk zijn doorgerekend.\n",
                 "Maak een kopie van je datachecker output: fixeddrainagelevelarea. Dat werkt.\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "157d44d6",
+            "id": "166eb613",
             "metadata": {},
             "outputs": [],
             "source": [
+                "from notebook_setup import setup_notebook\n",
+                "notebook_data = setup_notebook()\n",
+                "\n",
                 "import os\n",
                 "import geopandas as gpd\n",
                 "import pandas as pd\n",
                 "import matplotlib.pyplot as plt\n",
                 "import numpy as np\n",
                 "from pathlib import Path\n",
                 "import sys\n",
                 "import importlib.resources as pkg_resources  # Load resource from package\n",
                 "import ipywidgets as widgets\n",
-                "import json\n",
-                "try:\n",
-                "    with open(os.getcwd() + \"/notebook_data.json\") as f:\n",
-                "        notebook_data = json.load(f)\n",
-                "except:\n",
-                "    pass\n",
+                "\n",
                 "from hhnk_threedi_tools import Folders\n",
                 "import hhnk_threedi_tools as htt\n",
                 "import hhnk_research_tools as hrt\n",
                 "\n",
                 "# import hhnk_threedi_tools.core.climate_scenarios as hrt_climate\n",
                 "import hhnk_threedi_tools.core.climate_scenarios.maskerkaart as maskerkaart\n",
                 "import hhnk_threedi_tools.core.climate_scenarios.ruimtekaart as ruimtekaart\n",
@@ -52,18 +50,18 @@
                 "import hhnk_threedi_tools.core.climate_scenarios.schadekaart as schadekaart\n",
                 "import hhnk_threedi_tools.core.climate_scenarios.peilgebieden as peilgebieden\n",
                 "from hhnk_threedi_tools.core.climate_scenarios.schadekaart_peilgebieden import maak_schade_polygon\n",
                 "from hhnk_threedi_tools.core.climate_scenarios.maskerkaart_raster import rasterize_maskerkaart\n",
                 "from hhnk_threedi_tools.core.climate_scenarios.klimaatsommen_prep import KlimaatsommenPrep\n",
                 "\n",
                 "# Folders inladen\n",
-                "# folder = Folders(notebook_data['polder_folder'])\n",
+                "folder = Folders(notebook_data['polder_folder'])\n",
                 "\n",
                 "# Of handmatig;\n",
-                "folder=Folders(r\"E:\\02.modellen\\model_test_v2\")\n"
+                "# folder=Folders(r\"E:\\02.modellen\\model_test_v2\")\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "id": "8ec3f357",
             "metadata": {},
@@ -221,21 +219,19 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "c5740d69",
             "metadata": {},
             "outputs": [],
             "source": [
-                "SCHADESCHATTER_PATH=Path(r\"E:\\01.basisgegevens\\hhnk_schadeschatter\") #TODO naar een localsettings oid verplaatsen?\n",
-                "\n",
                 "klimaatsommenrep = KlimaatsommenPrep(folder=folder,\n",
                 "    batch_name=batch_fd.name,\n",
-                "    cfg_file = SCHADESCHATTER_PATH/'01_data/cfg/cfg_lizard.cfg',\n",
+                "    cfg_file = 'cfg_lizard.cfg',\n",
                 "    landuse_file = r\"\\\\corp.hhnk.nl\\data\\Hydrologen_data\\Data\\01.basisgegevens\\rasters\\landgebruik\\landuse2019_tiles\\combined_rasters.vrt\",\n",
-                "    SCHADESCHATTER_PATH=SCHADESCHATTER_PATH\n",
+                "    verify=True\n",
                 ")\n",
                 "\n",
                 "klimaatsommenrep.run(gridgpkg=True, \n",
                 "                    depth=True, \n",
                 "                    dmg=True, \n",
                 "                    wlvl=False, \n",
                 "                    overwrite=False)"
```

### Comparing `hhnk-threedi-tools-2023.2/hhnk_threedi_tools/utils/notebooks/04_netcdf_naar_raster.ipynb` & `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/notebooks/04_netcdf_naar_raster.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9984763105823724%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(0, '#Add qgis plugin deps to syspath and load "*

 * *            "notebook_data\\n'), (1, 'from notebook_setup import setup_notebook\\n'), (2, "*

 * *            "'notebook_data = setup_notebook()\\n'), (3, '\\n'), (4, '\\n'), (16, 'folder_path = "*

 * *            'r"E:\\\\02.modellen\\\\model_test_v2"\\n\'), (23, "# dem_path = '*

 * *            'r\'E:\\\\\\\\02.modellen\\\\\\\\23_Katvoed\\\\\\\\02_schematisation\\\\\\\\00_basis\\\\\\\\rasters/dem_katvoed_ahn3.tif\'\\n")], '*

 * *            […]*

```diff
@@ -24,33 +24,38 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "cb23f2c3",
             "metadata": {},
             "outputs": [],
             "source": [
+                "#Add qgis plugin deps to syspath and load notebook_data\n",
+                "from notebook_setup import setup_notebook\n",
+                "notebook_data = setup_notebook()\n",
+                "\n",
+                "\n",
                 "import xarray \n",
                 "import threedi_raster_edits as tre\n",
                 "from hhnk_threedi_tools import Folders\n",
                 "import hhnk_research_tools as hrt\n",
                 "import geopandas as gpd\n",
                 "\n",
                 "from hhnk_threedi_tools.core.result_rasters.netcdf_to_gridgpkg import ThreediGrid\n",
                 "from hhnk_threedi_tools.core.result_rasters.calculate_raster import BaseCalculatorGPKG\n",
                 "\n",
                 "\n",
                 "#User input\n",
-                "folder_path = r\"E:\\02.modellen\\23_Katvoed\"\n",
+                "folder_path = r\"E:\\02.modellen\\model_test_v2\"\n",
                 "scenario = \"katvoed #1 piek_ghg_T1000\" #mapnaam\n",
                 "\n",
                 "\n",
                 "folder = Folders(folder_path)\n",
                 "\n",
                 "dem_path = folder.model.schema_base.rasters.dem.path\n",
-                "dem_path = r'E:\\\\02.modellen\\\\23_Katvoed\\\\02_schematisation\\\\00_basis\\\\rasters/dem_katvoed_ahn3.tif'\n",
+                "# dem_path = r'E:\\\\02.modellen\\\\23_Katvoed\\\\02_schematisation\\\\00_basis\\\\rasters/dem_katvoed_ahn3.tif'\n",
                 "\n",
                 "threedi_result = folder.threedi_results.one_d_two_d[scenario]\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
@@ -107,20 +112,18 @@
             "source": [
                 "calculator_kwargs = {\"dem_path\":dem_path,\n",
                 "                        \"grid_gdf\":grid_gdf, \n",
                 "                        \"wlvl_column\":\"wlvl_max_replaced\"}\n",
                 "\n",
                 "#Init calculator\n",
                 "with BaseCalculatorGPKG(**calculator_kwargs) as self:\n",
-                "    self.run(output_folder=threedi_result.pl,  \n",
-                "                output_raster_name=\"wlvl_corr.tif\",\n",
+                "    self.run(output_file=threedi_result.pl/\"wlvl_corr.tif\",  \n",
                 "                mode=\"MODE_WLVL\",\n",
                 "                overwrite=OVERWRITE)\n",
-                "    self.run(output_folder=threedi_result.pl,  \n",
-                "                output_raster_name=\"wdepth_corr.tif\",\n",
+                "    self.run(output_file=threedi_result.pl/\"wdepth_corr.tif\",  \n",
                 "                mode=\"MODE_WDEPTH\",\n",
                 "                overwrite=OVERWRITE)\n",
                 "    print(\"Done.\")"
             ]
         },
         {
             "cell_type": "code",
@@ -130,16 +133,15 @@
             "outputs": [],
             "source": [
                 "calculator_kwargs = {\"dem_path\":dem_path,\n",
                 "                        \"grid_gdf\":grid_gdf, \n",
                 "                        \"wlvl_column\":\"wlvl_max_orig\"}\n",
                 "\n",
                 "with BaseCalculatorGPKG(**calculator_kwargs) as self:\n",
-                "    self.run(output_folder=threedi_result.pl,  \n",
-                "                output_raster_name=\"wdepth_orig.tif\",\n",
+                "    self.run(output_file=threedi_result.pl/\"wdepth_orig.tif\",  \n",
                 "                mode=\"MODE_WDEPTH\",\n",
                 "                overwrite=OVERWRITE)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
@@ -154,39 +156,32 @@
             "execution_count": null,
             "id": "2fc5875b",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Schadeschatter heeft wat extra voorbereiding nodig.\n",
                 "from pathlib import Path\n",
-                "schadeschatter_path = Path(r\"E:\\01.basisgegevens\\hhnk_schadeschatter\")\n",
-                "\n",
-                "import sys\n",
-                "if str(schadeschatter_path) not in sys.path:\n",
-                "    sys.path.append(str(schadeschatter_path))\n",
-                "import hhnk_schadeschatter as hhnk_wss\n",
-                "\n",
                 "\n",
                 "#Variables\n",
-                "# cfg_file = schadeschatter_path/'01_data/cfg/cfg_hhnk_2020.cfg'\n",
-                "cfg_file = schadeschatter_path/'01_data/cfg/cfg_lizard.cfg'\n",
-                "landuse_file = schadeschatter_path/'01_data/landuse2020_tiles/combined_rasters.vrt'\n",
+                "cfg_file = hrt.get_pkg_resource_path(package_resource=hrt.waterschadeschatter.resources, \n",
+                "                                name=\"cfg_lizard.cfg\")\n",
+                "landuse_file = r\"E:\\01.basisgegevens\\rasters\\landgebruik\\landuse2019_3di_tiles\\landuse2019_3di_tiles.vrt\"\n",
                 "\n",
-                "depth_file = threedi_result.pl/\"wdepth_orig.tif\"\n",
-                "output_file = threedi_result.pl/\"damage_orig_lizard.tif\"\n",
+                "depth_file = threedi_result.pl/\"wdepth_corr.tif\"\n",
+                "output_file = threedi_result.pl/\"damage_corr_lizard.tif\"\n",
                 "\n",
                 "\n",
-                "wss_settings = {'duur_uur': 48, #uren\n",
+                "wss_settings = {'inundation_period': 48, #uren\n",
                 "                'herstelperiode':'10 dagen',\n",
                 "                'maand':'sep',\n",
                 "                'cfg_file':cfg_file,\n",
                 "                'dmg_type':'gem'}\n",
                 "\n",
                 "#Calculation\n",
-                "self = hhnk_wss.Waterschadeschatter(depth_file=depth_file, \n",
+                "self = hrt.Waterschadeschatter(depth_file=depth_file, \n",
                 "                        landuse_file=landuse_file, \n",
                 "                        wss_settings=wss_settings)\n",
                 "\n",
                 "# Berkenen schaderaster\n",
                 "self.run(output_raster=hrt.Raster(output_file), \n",
                 "            calculation_type=\"sum\", \n",
                 "            verbose=False, \n",
```

### Comparing `hhnk-threedi-tools-2023.2/hhnk_threedi_tools/utils/notebooks/05_sqlite_create_grid.ipynb` & `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/notebooks/05_sqlite_create_grid.ipynb`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9968055555555555%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(0, '#Add qgis plugin deps to syspath and load "*

 * *            "notebook_data\\n'), (1, 'from notebook_setup import setup_notebook\\n'), (2, "*

 * *            "'notebook_data = setup_notebook()\\n'), (3, '\\n')], delete: [23, 22, 21, 20, 19, 18, "*

 * *            "16, 15, 14, 13, 12, 11, 10]}}, 2: {'source': {delete: [1, 0]}}}"}*

```diff
@@ -10,38 +10,29 @@
         },
         {
             "cell_type": "code",
             "execution_count": 16,
             "metadata": {},
             "outputs": [],
             "source": [
+                "#Add qgis plugin deps to syspath and load notebook_data\n",
+                "from notebook_setup import setup_notebook\n",
+                "notebook_data = setup_notebook()\n",
+                "\n",
                 "import os\n",
                 "import geopandas as gpd\n",
                 "import pandas as pd\n",
                 "import matplotlib.pyplot as plt\n",
                 "import numpy as np\n",
                 "from osgeo import gdal\n",
                 "import sys\n",
                 "import importlib.resources as pkg_resources  # Load resource from package\n",
                 "import ipywidgets as widgets\n",
                 "import json\n",
                 "\n",
-                "\n",
-                "\n",
-                "# for path in notebook_data[\"syspaths\"]:\n",
-                "#     sys.path.insert(0, path)\n",
-                "path=r'C:\\Users\\wvangerwen\\AppData\\Roaming\\QGIS\\QGIS3\\profiles\\default\\python\\plugins'\n",
-                "sys.path.insert(0, path)\n",
-                "\n",
-                "import hhnk_threedi_plugin.local_settings as local_settings\n",
-                "if local_settings.DEBUG:\n",
-                "    sys.path.insert(0, local_settings.hhnk_threedi_tools_path)\n",
-                "    import importlib, hhnk_threedi_tools\n",
-                "    hhnk_threedi_tools=importlib.reload(hhnk_threedi_tools)\n",
-                "    importlib.reload(hhnk_threedi_tools.core.folders)\n",
                 "    \n",
                 "from hhnk_threedi_tools import Folders, SqliteCheck"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 22,
@@ -52,16 +43,14 @@
                     "output_type": "stream",
                     "text": [
                         "v6\n"
                     ]
                 }
             ],
             "source": [
-                "with open(os.getcwd() + \"/notebook_data.json\") as f:\n",
-                "    notebook_data = json.load(f)\n",
                 "folder_dir = notebook_data['polder_folder']\n",
                 "\n",
                 "folder = Folders(folder_dir)\n",
                 "sqlite_test = SqliteCheck(folder)\n",
                 "\n",
                 "sqlite_test.create_grid_from_sqlite(sqlite_path=folder.model.sqlite_paths[0], \n",
                 "                                                        dem_path=folder.model.rasters.dem.path, \n",
```

### Comparing `hhnk-threedi-tools-2023.2/hhnk_threedi_tools/utils/notebooks/__pycache__/run.cpython-37.pyc` & `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/notebooks/__pycache__/run.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.2/hhnk_threedi_tools/utils/notebooks/__pycache__/run.cpython-39.pyc` & `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/notebooks/__pycache__/run.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 24 14:42:59 2023 UTC, .py size: 7154 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7395 4664 f21b 0000  a.......s.Fd....
+00000000: 610d 0d0a 0000 0000 8999 9264 ec1c 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 e000 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6402 6c05 5a05 6401 6402 6c06  Z.d.d.l.Z.d.d.l.
 00000060: 5a06 6401 6402 6c07 5a07 6401 6402 6c08  Z.d.d.l.Z.d.d.l.
 00000070: 5a08 6401 6403 6c04 6d09 5a09 0100 6404  Z.d.d.l.m.Z...d.
@@ -30,15 +30,15 @@
 000001d0: 6401 6402 8400 5a03 6403 6404 8400 5a04  d.d...Z.d.d...Z.
 000001e0: 6405 6406 8400 5a05 6407 5300 2908 da08  d.d...Z.d.S.)...
 000001f0: 5465 6d70 436f 7079 6302 0000 0000 0000  TempCopyc.......
 00000200: 0000 0000 0002 0000 0002 0000 0043 0000  .............C..
 00000210: 0073 0a00 0000 7c01 7c00 5f00 6400 5300  .s....|.|._.d.S.
 00000220: a901 4e29 01da 0d6f 7269 6769 6e61 6c5f  ..N)...original_
 00000230: 7061 7468 2902 da04 7365 6c66 7207 0000  path)...selfr...
-00000240: 00a9 0072 0900 0000 fa51 453a 5c67 6974  ...r.....QE:\git
+00000240: 00a9 0072 0900 0000 fa51 653a 5c67 6974  ...r.....Qe:\git
 00000250: 6875 625c 7776 616e 6765 7277 656e 5c68  hub\wvangerwen\h
 00000260: 686e 6b2d 7468 7265 6564 692d 746f 6f6c  hnk-threedi-tool
 00000270: 735c 6868 6e6b 5f74 6872 6565 6469 5f74  s\hhnk_threedi_t
 00000280: 6f6f 6c73 5c75 7469 6c73 5c6e 6f74 6562  ools\utils\noteb
 00000290: 6f6f 6b73 5c72 756e 2e70 79da 085f 5f69  ooks\run.py..__i
 000002a0: 6e69 745f 5f1c 0000 0073 0200 0000 0001  nit__....s......
 000002b0: 7a11 5465 6d70 436f 7079 2e5f 5f69 6e69  z.TempCopy.__ini
@@ -48,15 +48,15 @@
 000002f0: 006a 05a1 017d 0274 026a 03a0 067c 017c  .j...}.t.j...|.|
 00000300: 02a1 027c 005f 0374 07a0 087c 006a 057c  ...|._.t...|.j.|
 00000310: 006a 03a1 0201 007c 006a 0353 0072 0600  .j.....|.j.S.r..
 00000320: 0000 2909 da08 7465 6d70 6669 6c65 da0a  ..)...tempfile..
 00000330: 6765 7474 656d 7064 6972 da02 6f73 da04  gettempdir..os..
 00000340: 7061 7468 da08 6261 7365 6e61 6d65 7207  path..basenamer.
 00000350: 0000 00da 046a 6f69 6eda 0673 6875 7469  .....join..shuti
-00000360: 6cda 0563 6f70 7932 2903 7208 0000 005a  l..copy2).r....Z
+00000360: 6cda 0563 6f70 7932 2903 7208 0000 00da  l..copy2).r.....
 00000370: 0874 656d 705f 6469 72da 0962 6173 655f  .temp_dir..base_
 00000380: 7061 7468 7209 0000 0072 0900 0000 720a  pathr....r....r.
 00000390: 0000 00da 095f 5f65 6e74 6572 5f5f 1f00  .....__enter__..
 000003a0: 0000 730a 0000 0000 0108 010e 0110 0110  ..s.............
 000003b0: 017a 1254 656d 7043 6f70 792e 5f5f 656e  .z.TempCopy.__en
 000003c0: 7465 725f 5f63 0400 0000 0000 0000 0000  ter__c..........
 000003d0: 0000 0400 0000 0300 0000 4300 0000 7310  ..........C...s.
@@ -67,323 +67,328 @@
 00000420: 7863 5f76 616c da06 6578 635f 7462 7209  xc_val..exc_tbr.
 00000430: 0000 0072 0900 0000 720a 0000 00da 085f  ...r....r......_
 00000440: 5f65 7869 745f 5f26 0000 0073 0200 0000  _exit__&...s....
 00000450: 0001 7a11 5465 6d70 436f 7079 2e5f 5f65  ..z.TempCopy.__e
 00000460: 7869 745f 5f4e 2906 da08 5f5f 6e61 6d65  xit__N)...__name
 00000470: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
 00000480: 5f5f 7175 616c 6e61 6d65 5f5f 720b 0000  __qualname__r...
-00000490: 0072 1500 0000 721a 0000 0072 0900 0000  .r....r....r....
+00000490: 0072 1600 0000 721b 0000 0072 0900 0000  .r....r....r....
 000004a0: 7209 0000 0072 0900 0000 720a 0000 0072  r....r....r....r
 000004b0: 0500 0000 1b00 0000 7306 0000 0008 0108  ........s.......
 000004c0: 0308 0772 0500 0000 6302 0000 0000 0000  ...r....c.......
-000004d0: 0000 0000 0003 0000 0006 0000 0043 0000  .............C..
-000004e0: 0073 4800 0000 7400 6a01 7c00 6401 6402  .sH...t.j.|.d.d.
-000004f0: 8d02 0100 7400 a002 7c01 a101 4400 5d2a  ....t...|...D.]*
-00000500: 7d02 7c02 a003 6403 a101 7218 7404 a005  }.|...d...r.t...
-00000510: 7c01 6404 1700 7c02 1700 7c00 6404 1700  |.d...|...|.d...
-00000520: 7c02 1700 a102 0100 7118 6400 5300 2905  |.......q.d.S.).
-00000530: 4e54 2901 da08 6578 6973 745f 6f6b 7a06  NT)...exist_okz.
-00000540: 2e69 7079 6e62 fa01 2f29 0672 0e00 0000  .ipynb../).r....
-00000550: da08 6d61 6b65 6469 7273 da07 6c69 7374  ..makedirs..list
-00000560: 6469 72da 0865 6e64 7377 6974 6872 1200  dir..endswithr..
-00000570: 0000 7213 0000 0029 035a 076e 6577 5f64  ..r....).Z.new_d
-00000580: 6972 5a0c 6f72 6967 696e 616c 5f64 6972  irZ.original_dir
-00000590: da04 6669 6c65 7209 0000 0072 0900 0000  ..filer....r....
-000005a0: 720a 0000 00da 0e63 6f70 795f 6e6f 7465  r......copy_note
-000005b0: 626f 6f6b 732a 0000 0073 0800 0000 0001  books*...s......
-000005c0: 0e02 0e01 0a01 7224 0000 0063 0200 0000  ......r$...c....
-000005d0: 0000 0000 0000 0000 0300 0000 0800 0000  ................
-000005e0: 4300 0000 733e 0000 0074 007c 0064 0117  C...s>...t.|.d..
-000005f0: 0064 0283 028f 1c7d 0274 01a0 027c 017c  .d.....}.t...|.|
-00000600: 02a1 0201 0057 0064 0004 0004 0083 0301  .....W.d........
-00000610: 006e 1031 0073 3030 0001 0001 0001 0059  .n.1.s00.......Y
-00000620: 0001 0064 0053 0029 034e fa13 2f6e 6f74  ...d.S.).N../not
-00000630: 6562 6f6f 6b5f 6461 7461 2e6a 736f 6eda  ebook_data.json.
-00000640: 0177 2903 da04 6f70 656e da04 6a73 6f6e  .w)...open..json
-00000650: da04 6475 6d70 2903 da09 6469 7265 6374  ..dump)...direct
-00000660: 6f72 79da 0464 6174 61da 0166 7209 0000  ory..data..fr...
-00000670: 0072 0900 0000 720a 0000 00da 1377 7269  .r....r......wri
-00000680: 7465 5f6e 6f74 6562 6f6f 6b5f 6a73 6f6e  te_notebook_json
-00000690: 3200 0000 7304 0000 0000 0110 0172 2d00  2...s........r-.
-000006a0: 0000 6301 0000 0000 0000 0000 0000 0002  ..c.............
-000006b0: 0000 0008 0000 0043 0000 0073 3a00 0000  .......C...s:...
-000006c0: 7400 7c00 6401 1700 8301 8f1a 7d01 7401  t.|.d.......}.t.
-000006d0: a002 7c01 a101 5700 0200 6400 0400 0400  ..|...W...d.....
-000006e0: 8303 0100 5300 3100 732c 3000 0100 0100  ....S.1.s,0.....
-000006f0: 0100 5900 0100 6400 5300 2902 4e72 2500  ..Y...d.S.).Nr%.
-00000700: 0000 2903 7227 0000 0072 2800 0000 da04  ..).r'...r(.....
-00000710: 6c6f 6164 2902 722a 0000 0072 2c00 0000  load).r*...r,...
-00000720: 7209 0000 0072 0900 0000 720a 0000 00da  r....r....r.....
-00000730: 1272 6561 645f 6e6f 7465 626f 6f6b 5f6a  .read_notebook_j
-00000740: 736f 6e37 0000 0073 0400 0000 0001 0e01  son7...s........
-00000750: 722f 0000 0063 0000 0000 0000 0000 0000  r/...c..........
-00000760: 0000 0600 0000 0400 0000 4300 0000 73ba  ..........C...s.
-00000770: 0000 0064 017d 0074 006a 017d 0174 026a  ...d.}.t.j.}.t.j
-00000780: 03a0 047c 01a1 015c 027d 027d 0364 027c  ...|...\.}.}.d.|
-00000790: 0376 0072 587c 03a0 05a1 0064 0376 0072  .v.rX|.....d.v.r
-000007a0: 347c 017d 006e 0c74 0664 047c 0116 0083  4|.}.n.t.d.|....
-000007b0: 0182 0174 026a 03a0 077c 00a1 0173 504a  ...t.j...|...sPJ
-000007c0: 0082 0164 027c 0066 0253 0064 057c 0376  ...d.|.f.S.d.|.v
-000007d0: 0072 b674 0874 09a0 0a7c 01a1 016a 0b64  .r.t.t...|...j.d
-000007e0: 0619 0083 017d 0474 02a0 0c7c 04a1 017d  .....}.t...|...}
-000007f0: 0564 077c 0576 0072 8e7c 0464 0817 007d  .d.|.v.r.|.d...}
-00000800: 0064 097c 0576 0072 9e7c 0464 0a17 007d  .d.|.v.r.|.d...}
-00000810: 007c 0073 ae74 0664 0b7c 0416 0083 0182  .|.s.t.d.|......
-00000820: 0164 057c 0066 0253 0064 0153 0029 0c7a  .d.|.f.S.d.S.).z
-00000830: ef52 6574 7572 6e20 7468 6520 7061 7468  .Return the path
-00000840: 2074 6f20 7468 6520 7079 7468 6f6e 3320   to the python3 
-00000850: 696e 7465 7270 7265 7465 722e 0a0a 2020  interpreter...  
-00000860: 2020 556e 6465 7220 6c69 6e75 7820 7379    Under linux sy
-00000870: 732e 6578 6563 7574 6162 6c65 2069 7320  s.executable is 
-00000880: 7365 7420 746f 2074 6865 2070 7974 686f  set to the pytho
-00000890: 6e33 2069 6e74 6572 7072 6574 6572 2075  n3 interpreter u
-000008a0: 7365 6420 6279 2051 6769 732e 0a20 2020  sed by Qgis..   
-000008b0: 2048 6f77 6576 6572 2c20 756e 6465 7220   However, under 
-000008c0: 5769 6e64 6f77 732f 4d61 6320 7468 6973  Windows/Mac this
-000008d0: 2069 7320 6e6f 7420 7468 6520 6361 7365   is not the case
-000008e0: 2061 6e64 2073 7973 2e65 7865 6375 7461   and sys.executa
-000008f0: 626c 6520 7265 6665 7273 2074 6f20 7468  ble refers to th
-00000900: 650a 2020 2020 5167 6973 2073 7461 7274  e.    Qgis start
-00000910: 2d75 7020 7363 7269 7074 2e0a 2020 2020  -up script..    
-00000920: 4eda 0670 7974 686f 6e29 027a 0a70 7974  N..python).z.pyt
-00000930: 686f 6e2e 6578 657a 0b70 7974 686f 6e33  hon.exez.python3
-00000940: 2e65 7865 7a27 556e 6578 7065 6374 6564  .exez'Unexpected
-00000950: 2076 616c 7565 2066 6f72 2073 7973 2e65   value for sys.e
-00000960: 7865 6375 7461 626c 653a 2025 735a 0471  xecutable: %sZ.q
-00000970: 6769 7372 0100 0000 7a0b 7079 335f 656e  gisr....z.py3_en
-00000980: 762e 6261 747a 0c2f 7079 335f 656e 762e  v.batz./py3_env.
-00000990: 6261 747a 1370 7974 686f 6e2d 7167 6973  batz.python-qgis
-000009a0: 2d6c 7472 2e62 6174 7a14 2f70 7974 686f  -ltr.batz./pytho
-000009b0: 6e2d 7167 6973 2d6c 7472 2e62 6174 7a2a  n-qgis-ltr.batz*
-000009c0: 636f 756c 6420 6e6f 7420 6669 6e64 2071  could not find q
-000009d0: 6769 732d 7079 7468 6f6e 2062 6174 2066  gis-python bat f
-000009e0: 696c 6520 696e 3a20 2573 290d da03 7379  ile in: %s)...sy
-000009f0: 73da 0a65 7865 6375 7461 626c 6572 0e00  s..executabler..
-00000a00: 0000 720f 0000 00da 0573 706c 6974 da05  ..r......split..
-00000a10: 6c6f 7765 72da 1045 6e76 6972 6f6e 6d65  lower..Environme
-00000a20: 6e74 4572 726f 72da 0665 7869 7374 73da  ntError..exists.
-00000a30: 0373 7472 da07 7061 7468 6c69 6272 0300  .str..pathlibr..
-00000a40: 0000 da07 7061 7265 6e74 7372 2100 0000  ....parentsr!...
-00000a50: 2906 5a0b 696e 7465 7270 7265 7465 7272  ).Z.interpreterr
-00000a60: 3200 0000 722a 0000 00da 0866 696c 656e  2...r*.....filen
-00000a70: 616d 655a 0b6d 6169 6e5f 666f 6c64 6572  ameZ.main_folder
-00000a80: 5a0c 666f 6c64 6572 5f66 696c 6573 7209  Z.folder_filesr.
-00000a90: 0000 0072 0900 0000 720a 0000 00da 175f  ...r....r......_
-00000aa0: 6765 745f 7079 7468 6f6e 5f69 6e74 6572  get_python_inter
-00000ab0: 7072 6574 6572 3c00 0000 732e 0000 0000  preter<...s.....
-00000ac0: 0704 0106 0110 0108 020c 0106 0202 0106  ................
-00000ad0: ff04 0310 0108 0208 0214 010a 0208 0108  ................
-00000ae0: 0208 0108 0204 0102 0106 ff04 0472 3b00  .............r;.
-00000af0: 0000 6300 0000 0000 0000 0000 0000 0001  ..c.............
-00000b00: 0000 0004 0000 0043 0000 0073 3000 0000  .......C...s0...
-00000b10: 7400 a001 a100 a002 6401 6402 a102 7d00  t.......d.d...}.
-00000b20: 7403 6a04 a005 7c00 6403 1700 a101 7228  t.j...|.d.....r(
-00000b30: 7c00 6403 1700 5300 6400 5300 6400 5300  |.d...S.d.S.d.S.
-00000b40: 2904 4efa 0d73 6974 652d 7061 636b 6167  ).N..site-packag
-00000b50: 6573 da07 5363 7269 7074 737a 102f 6a75  es..Scriptsz./ju
-00000b60: 7079 7465 722d 6c61 622e 6578 65a9 06da  pyter-lab.exe...
-00000b70: 0473 6974 65da 1367 6574 7573 6572 7369  .site..getusersi
-00000b80: 7465 7061 636b 6167 6573 da07 7265 706c  tepackages..repl
-00000b90: 6163 6572 0e00 0000 720f 0000 0072 3600  acer....r....r6.
-00000ba0: 0000 a901 720f 0000 0072 0900 0000 7209  ....r....r....r.
-00000bb0: 0000 0072 0a00 0000 da1c 7573 6572 5f69  ...r......user_i
-00000bc0: 6e73 7461 6c6c 6564 5f6e 6f74 6562 6f6f  nstalled_noteboo
-00000bd0: 6b5f 7061 7468 6400 0000 7308 0000 0000  k_pathd...s.....
-00000be0: 0110 0110 0108 0272 4300 0000 6300 0000  .......rC...c...
-00000bf0: 0000 0000 0000 0000 0001 0000 0004 0000  ................
-00000c00: 0043 0000 0073 3000 0000 7400 a001 a100  .C...s0...t.....
-00000c10: a002 6401 6402 a102 7d00 7403 6a04 a005  ..d.d...}.t.j...
-00000c20: 7c00 6403 1700 a101 7228 7c00 6403 1700  |.d.....r(|.d...
-00000c30: 5300 6400 5300 6400 5300 2904 4e72 3c00  S.d.S.d.S.).Nr<.
-00000c40: 0000 723d 0000 007a 0c2f 6970 7974 686f  ..r=...z./ipytho
-00000c50: 6e2e 6578 6572 3e00 0000 7242 0000 0072  n.exer>...rB...r
-00000c60: 0900 0000 7209 0000 0072 0a00 0000 da1b  ....r....r......
-00000c70: 7573 6572 5f69 6e73 7461 6c6c 6564 5f69  user_installed_i
-00000c80: 7079 7468 6f6e 5f70 6174 686c 0000 0073  python_pathl...s
-00000c90: 0800 0000 0001 1001 1001 0802 7244 0000  ............rD..
-00000ca0: 00da 056f 7367 656f 4663 0200 0000 0000  ...osgeoFc......
-00000cb0: 0000 0000 0000 0500 0000 0300 0000 4300  ..............C.
-00000cc0: 0000 733c 0000 0074 0083 005c 027d 027d  ..s<...t...\.}.}
-00000cd0: 037c 0064 016b 0272 1e7c 0364 0264 0367  .|.d.k.r.|.d.d.g
-00000ce0: 037d 046e 1a7c 0172 2e7c 0374 0183 0067  .}.n.|.r.|.t...g
-00000cf0: 027d 046e 0a7c 0374 0283 0067 027d 047c  .}.n.|.t...g.}.|
-00000d00: 0453 0029 047a a969 6620 6a75 7079 7465  .S.).z.if jupyte
-00000d10: 7220 6973 2069 6e73 7461 6c6c 6564 2069  r is installed i
-00000d20: 6e20 6f73 6765 6f2c 2075 7365 206f 7367  n osgeo, use osg
-00000d30: 656f 2e0a 2020 2020 6966 206a 7570 7974  eo..    if jupyt
-00000d40: 6572 2069 7320 696e 7374 616c 6c65 6420  er is installed 
-00000d50: 696e 2074 6865 2075 7365 7220 6469 7220  in the user dir 
-00000d60: 2770 6970 2069 6e73 7461 6c6c 206a 7570  'pip install jup
-00000d70: 7974 6572 202d 2d75 7365 7227 0a20 2020  yter --user'.   
-00000d80: 2075 7365 2027 7573 6572 272e 0a0a 2020   use 'user'...  
-00000d90: 2020 2775 7365 7227 2075 7365 7320 616e    'user' uses an
-00000da0: 2065 7865 6374 7561 626c 650a 2020 2020   exectuable.    
-00000db0: 7245 0000 007a 022d 6d7a 0b6a 7570 7974  rE...z.-mz.jupyt
-00000dc0: 6572 2d6c 6162 2903 723b 0000 0072 4400  er-lab).r;...rD.
-00000dd0: 0000 7243 0000 0029 05da 086c 6f63 6174  ..rC...)...locat
-00000de0: 696f 6eda 0769 7079 7468 6f6e da06 7379  ion..ipython..sy
-00000df0: 7374 656d 5a12 7079 7468 6f6e 5f69 6e74  stemZ.python_int
-00000e00: 6572 7072 6574 6572 da07 636f 6d6d 616e  erpreter..comman
-00000e10: 6472 0900 0000 7209 0000 0072 0a00 0000  dr....r....r....
-00000e20: da10 6e6f 7465 626f 6f6b 5f63 6f6d 6d61  ..notebook_comma
-00000e30: 6e64 7400 0000 730e 0000 0000 070a 0108  ndt...s.........
-00000e40: 010c 0704 010c 020a 0172 4a00 0000 da03  .........rJ.....
-00000e50: 7275 6e63 0400 0000 0000 0000 0000 0000  runc............
-00000e60: 0800 0000 0a00 0000 4300 0000 7300 0100  ........C...s...
-00000e70: 0064 0164 0284 0074 006a 01a0 0264 03a1  .d.d...t.j...d..
-00000e80: 01a0 0374 006a 04a1 0144 0083 017d 047c  ...t.j...D...}.|
-00000e90: 0344 005d 367d 0574 057c 0583 017d 057c  .D.]6}.t.|...}.|
-00000ea0: 057c 0476 0172 227c 05a0 06a1 009b 0074  .|.v.r"|.......t
-00000eb0: 006a 049b 0074 006a 0164 0319 009b 009d  .j...t.j.d......
-00000ec0: 0374 006a 0164 033c 0071 2274 0764 0474  .t.j.d.<.q"t.d.t
-00000ed0: 006a 01a0 0264 03a1 01a0 0374 006a 04a1  .j...d.....t.j..
-00000ee0: 019b 009d 0283 0101 0074 087c 0183 017d  .........t.|...}
-00000ef0: 067c 0072 8e7c 06a0 097c 00a1 0101 007c  .|.r.|...|.....|
-00000f00: 0264 056b 0272 cc74 0a6a 0b7c 0664 0664  .d.k.r.t.j.|.d.d
-00000f10: 0664 0764 0764 0764 0674 0c74 0d42 0064  .d.d.d.d.t.t.B.d
-00000f20: 088d 087d 0774 0764 097c 076a 0e9b 0064  ...}.t.d.|.j...d
-00000f30: 0a7c 069b 009d 0483 0101 006e 307c 0264  .|.........n0|.d
-00000f40: 0b6b 0272 fc67 0064 0ca2 017c 0617 007d  .k.r.g.d...|...}
-00000f50: 0674 0a6a 0f7c 0664 0664 0d8d 027d 0774  .t.j.|.d.d...}.t
-00000f60: 0764 0e7c 069b 009d 0283 0101 0064 0753  .d.|.........d.S
-00000f70: 0029 0f7a e964 6972 6563 746f 7279 3a0a  .).z.directory:.
-00000f80: 2020 2020 2020 2020 6e6f 7465 626f 6f6b          notebook
-00000f90: 7320 6f70 656e 2069 6e20 6120 6365 7274  s open in a cert
-00000fa0: 6169 6e20 6469 7265 6374 6f72 790a 2020  ain directory.  
-00000fb0: 2020 6c6f 6361 7469 6f6e 3a0a 2020 2020    location:.    
-00000fc0: 2020 2020 6361 6e20 6569 7468 6572 2062      can either b
-00000fd0: 6520 276f 7367 656f 2720 6f72 2027 7573  e 'osgeo' or 'us
-00000fe0: 6572 270a 2020 2020 2020 2020 6f70 656e  er'.        open
-00000ff0: 206a 7570 7974 6572 206e 6f74 6562 6f6f   jupyter noteboo
-00001000: 6b20 6973 206f 7367 656f 206f 7220 7065  k is osgeo or pe
-00001010: 722d 7573 6572 2d69 6e73 7461 6c6c 6564  r-user-installed
-00001020: 202e 6578 650a 2020 2020 7573 653a 0a20   .exe.    use:. 
-00001030: 2020 2020 2020 2073 7562 7072 6f63 6573         subproces
-00001040: 7320 6d6f 6465 2028 2770 6f70 656e 2720  s mode ('popen' 
-00001050: 6f72 2027 7275 6e27 290a 2020 2020 6301  or 'run').    c.
-00001060: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-00001070: 0000 0053 0000 0073 1400 0000 6700 7c00  ...S...s....g.|.
-00001080: 5d0c 7d01 7400 7c01 8301 9102 7104 5300  ].}.t.|.....q.S.
-00001090: 7209 0000 0072 0200 0000 2902 da02 2e30  r....r....)....0
-000010a0: da01 6972 0900 0000 7209 0000 0072 0a00  ..ir....r....r..
-000010b0: 0000 da0a 3c6c 6973 7463 6f6d 703e 9300  ....<listcomp>..
-000010c0: 0000 f300 0000 007a 1f6f 7065 6e5f 7365  .......z.open_se
-000010d0: 7276 6572 2e3c 6c6f 6361 6c73 3e2e 3c6c  rver.<locals>.<l
-000010e0: 6973 7463 6f6d 703e da04 5041 5448 7a06  istcomp>..PATHz.
-000010f0: 7061 7468 203a da05 706f 7065 6e54 4e29  path :..popenTN)
-00001100: 07da 0573 6865 6c6c da12 756e 6976 6572  ...shell..univer
-00001110: 7361 6c5f 6e65 776c 696e 6573 da05 7374  sal_newlines..st
-00001120: 6469 6eda 0673 7464 6f75 74da 0673 7464  din..stdout..std
-00001130: 6572 72da 0963 6c6f 7365 5f66 6473 da0d  err..close_fds..
-00001140: 6372 6561 7469 6f6e 666c 6167 737a 1d53  creationflagsz.S
-00001150: 7461 7274 6564 2070 726f 6365 7373 696e  tarted processin
-00001160: 6720 7769 7468 2070 6964 3a20 7a0d 2061  g with pid: z. a
-00001170: 6e64 2063 6f6d 6d61 6e64 2072 4b00 0000  nd command rK...
-00001180: 2903 da05 7374 6172 74da 0363 6d64 7a02  )...start..cmdz.
-00001190: 2f4b a901 7252 0000 007a 2053 7461 7274  /K..rR...z Start
-000011a0: 6564 2070 726f 6365 7373 696e 6720 7769  ed processing wi
-000011b0: 7468 2063 6f6d 6d61 6e64 2029 1072 0e00  th command ).r..
-000011c0: 0000 da07 656e 7669 726f 6eda 0367 6574  ....environ..get
-000011d0: 7233 0000 00da 0770 6174 6873 6570 7203  r3.....pathsepr.
-000011e0: 0000 00da 0861 735f 706f 7369 78da 0570  .....as_posix..p
-000011f0: 7269 6e74 724a 0000 00da 0661 7070 656e  rintrJ.....appen
-00001200: 64da 0a73 7562 7072 6f63 6573 73da 0550  d..subprocess..P
-00001210: 6f70 656e da10 4445 5441 4348 4544 5f50  open..DETACHED_P
-00001220: 524f 4345 5353 da18 4352 4541 5445 5f4e  ROCESS..CREATE_N
-00001230: 4557 5f50 524f 4345 5353 5f47 524f 5550  EW_PROCESS_GROUP
-00001240: da03 7069 6472 4b00 0000 2908 722a 0000  ..pidrK...).r*..
-00001250: 0072 4600 0000 da03 7573 655a 0e6e 6f74  .rF.....useZ.not
-00001260: 6562 6f6f 6b5f 7061 7468 73da 0570 6174  ebook_paths..pat
-00001270: 6873 720f 0000 0072 4900 0000 da07 7072  hsr....rI.....pr
-00001280: 6f63 6573 7372 0900 0000 7209 0000 0072  ocessr....r....r
-00001290: 0a00 0000 da0b 6f70 656e 5f73 6572 7665  ......open_serve
-000012a0: 728a 0000 0073 3200 0000 0009 1e01 0801  r....s2.........
-000012b0: 0801 0801 2401 1e01 0802 0401 0a02 0801  ....$...........
-000012c0: 0401 0201 0201 0201 0201 0201 0201 0201  ................
-000012d0: 06f8 060a 1801 0801 0c01 0e01 726a 0000  ............rj..
-000012e0: 0063 0200 0000 0000 0000 0000 0000 0400  .c..............
-000012f0: 0000 0800 0000 4300 0000 7346 0000 0074  ......C...sF...t
-00001300: 007c 0183 017d 0274 017c 0064 0183 028f  .|...}.t.|.d....
-00001310: 207d 037c 03a0 0264 02a0 037c 02a1 01a1   }.|...d...|....
-00001320: 0101 0057 0064 0004 0004 0083 0301 006e  ...W.d.........n
-00001330: 1031 0073 3830 0001 0001 0001 0059 0001  .1.s80.......Y..
-00001340: 0064 0053 0029 034e 7226 0000 00fa 0120  .d.S.).Nr&..... 
-00001350: 2904 724a 0000 0072 2700 0000 da05 7772  ).rJ...r'.....wr
-00001360: 6974 6572 1100 0000 2904 720f 0000 0072  iter....).r....r
-00001370: 4600 0000 7249 0000 005a 0862 6174 5f66  F...rI...Z.bat_f
-00001380: 696c 6572 0900 0000 7209 0000 0072 0a00  iler....r....r..
-00001390: 0000 da17 6372 6561 7465 5f63 6f6d 6d61  ....create_comma
-000013a0: 6e64 5f62 6174 5f66 696c 65b0 0000 0073  nd_bat_file....s
-000013b0: 0600 0000 0001 0802 0c01 726d 0000 0063  ..........rm...c
-000013c0: 0100 0000 0000 0000 0000 0000 0a00 0000  ................
-000013d0: 0800 0000 4300 0000 731a 0100 0074 006a  ....C...s....t.j
-000013e0: 0164 0119 007d 017c 0164 0217 007d 0264  .d...}.|.d...}.d
-000013f0: 037d 037c 0044 005d 207d 047c 04a0 0264  .}.|.D.] }.|...d
-00001400: 0464 05a1 027d 047c 0364 067c 049b 0064  .d...}.|.d.|...d
-00001410: 079d 0317 007d 0371 1a64 087c 039b 0064  .....}.q.d.|...d
-00001420: 099d 037d 0574 006a 03a0 047c 02a1 0173  ...}.t.j...|...s
-00001430: 8474 0564 0a64 0b64 0c8d 027d 067c 0664  .t.d.d.d...}.|.d
-00001440: 0d19 0064 0e17 007d 0674 066a 077c 0664  ...d...}.t.j.|.d
-00001450: 0b64 0f8d 0201 0074 0864 107c 0683 0201  .d.....t.d.|....
-00001460: 0064 117d 0774 097c 0264 1283 028f 2a7d  .d.}.t.|.d....*}
-00001470: 087c 0844 005d 147d 097c 057c 0876 0072  .|.D.].}.|.|.v.r
-00001480: 9864 0b7d 0701 0071 ae71 9857 0064 1304  .d.}...q.q.W.d..
-00001490: 0004 0083 0301 006e 1031 0073 c230 0001  .......n.1.s.0..
-000014a0: 0001 0001 0059 0001 007c 0790 0173 1674  .....Y...|...s.t
-000014b0: 0864 147c 0583 0201 0074 097c 0264 1583  .d.|.....t.|.d..
-000014c0: 028f 1e7d 087c 08a0 0a64 167c 0517 00a1  ...}.|...d.|....
-000014d0: 0101 0057 0064 1304 0004 0083 0301 006e  ...W.d.........n
-000014e0: 1231 0090 0173 0c30 0001 0001 0001 0059  .1...s.0.......Y
-000014f0: 0001 0064 1353 0029 177a 3661 6464 7320  ...d.S.).z6adds 
-00001500: 6578 7472 6120 6e6f 7465 626f 6f6b 2070  extra notebook p
-00001510: 6174 6873 2c20 7768 6963 6820 6973 2075  aths, which is u
-00001520: 7365 6420 696e 2074 6865 2070 6c75 6769  sed in the plugi
-00001530: 6eda 0b55 5345 5250 524f 4649 4c45 7a2b  n..USERPROFILEz+
-00001540: 2f2e 6970 7974 686f 6e2f 7072 6f66 696c  /.ipython/profil
-00001550: 655f 6465 6661 756c 742f 6970 7974 686f  e_default/ipytho
-00001560: 6e5f 636f 6e66 6967 2e70 797a 0a69 6d70  n_config.pyz.imp
-00001570: 6f72 7420 7379 73fa 015c 721f 0000 007a  ort sys..\r....z
-00001580: 153b 2073 7973 2e70 6174 682e 696e 7365  .; sys.path.inse
-00001590: 7274 2830 2c22 7a02 2229 7a25 632e 496e  rt(0,"z.")z%c.In
-000015a0: 7465 7261 6374 6976 6553 6865 6c6c 4170  teractiveShellAp
-000015b0: 702e 6578 6563 5f6c 696e 6573 203d 205b  p.exec_lines = [
-000015c0: 277a 0227 5dda 0475 7365 7254 2901 7247  'z.']..userT).rG
-000015d0: 0000 00e9 0100 0000 7a0f 2070 726f 6669  ........z. profi
-000015e0: 6c65 2063 7265 6174 6572 5b00 0000 7a17  le creater[...z.
-000015f0: 4372 6561 7469 6e67 2070 726f 6669 6c65  Creating profile
-00001600: 2077 6974 683a 2046 da01 724e 7a07 4164   with: F..rNz.Ad
-00001610: 6469 6e67 3ada 0161 da01 0a29 0b72 0e00  ding:..a...).r..
-00001620: 0000 725c 0000 0072 4100 0000 720f 0000  ..r\...rA...r...
-00001630: 0072 3600 0000 724a 0000 0072 6200 0000  .r6...rJ...rb...
-00001640: 724b 0000 0072 6000 0000 7227 0000 0072  rK...r`...r'...r
-00001650: 6c00 0000 290a 5a14 6578 7472 615f 6e6f  l...).Z.extra_no
-00001660: 7465 626f 6f6b 5f70 6174 6873 5a11 7573  tebook_pathsZ.us
-00001670: 6572 5f70 726f 6669 6c65 5f70 6174 685a  er_profile_pathZ
-00001680: 1469 7079 7468 6f6e 5f70 726f 6669 6c65  .ipython_profile
-00001690: 5f70 6174 685a 0f6e 625f 7061 7468 5f63  _pathZ.nb_path_c
-000016a0: 6f6d 6d61 6e64 720f 0000 005a 096e 625f  ommandr....Z.nb_
-000016b0: 7374 7269 6e67 7249 0000 0072 3600 0000  stringrI...r6...
-000016c0: 5a0c 7072 6f66 696c 655f 636f 6465 724d  Z.profile_coderM
-000016d0: 0000 0072 0900 0000 7209 0000 0072 0a00  ...r....r....r..
-000016e0: 0000 da12 6164 645f 6e6f 7465 626f 6f6b  ....add_notebook
-000016f0: 5f70 6174 6873 b700 0000 732e 0000 0000  _paths....s.....
-00001700: 040a 0206 ff02 0404 0108 010c 0112 010c  ................
-00001710: 020c 020c 010c 020e 010a 0804 010c 0108  ................
-00001720: 0108 0104 0124 0206 010a 010c 0172 7500  .....$.......ru.
-00001730: 0000 2902 7245 0000 0046 2901 7245 0000  ..).rE...F).rE..
-00001740: 0029 1cda 075f 5f64 6f63 5f5f 720e 0000  .)...__doc__r...
-00001750: 0072 3100 0000 7262 0000 0072 3800 0000  .r1...rb...r8...
-00001760: 720c 0000 0072 1200 0000 7228 0000 0072  r....r....r(...r
-00001770: 3f00 0000 7203 0000 0072 6500 0000 7264  ?...r....re...rd
-00001780: 0000 0072 3700 0000 da08 5f5f 6669 6c65  ...r7.....__file
-00001790: 5f5f da06 7061 7265 6e74 da08 6162 736f  __..parent..abso
-000017a0: 6c75 7465 5a12 4e4f 5445 424f 4f4b 5f44  luteZ.NOTEBOOK_D
-000017b0: 4952 4543 544f 5259 7205 0000 0072 2400  IRECTORYr....r$.
-000017c0: 0000 722d 0000 0072 2f00 0000 723b 0000  ..r-...r/...r;..
-000017d0: 0072 4300 0000 7244 0000 0072 4a00 0000  .rC...rD...rJ...
-000017e0: 726a 0000 0072 6d00 0000 7275 0000 0072  rj...rm...ru...r
-000017f0: 0900 0000 7209 0000 0072 0900 0000 720a  ....r....r....r.
-00001800: 0000 00da 083c 6d6f 6475 6c65 3e03 0000  .....<module>...
-00001810: 0073 2e00 0000 0408 0801 0801 0801 0801  .s..............
-00001820: 0801 0801 0801 0801 0c02 0401 0402 1403  ................
-00001830: 0e0f 0c08 0805 0805 0828 0808 0808 0a16  .........(......
-00001840: 1226 0a07                                .&..
+000004d0: 0000 0000 0004 0000 0006 0000 0043 0000  .............C..
+000004e0: 0073 6c00 0000 7400 6a01 7c00 6401 6402  .sl...t.j.|.d.d.
+000004f0: 8d02 0100 7400 a002 7c01 a101 4400 5d4e  ....t...|...D.]N
+00000500: 7d02 7403 7c02 8301 0100 7c02 a004 6403  }.t.|.....|...d.
+00000510: a101 7234 6401 7d03 6e12 7c02 6404 6b02  ..r4d.}.n.|.d.k.
+00000520: 7242 6401 7d03 6e04 6405 7d03 7c03 7218  rBd.}.n.d.}.|.r.
+00000530: 7405 a006 7c01 6406 1700 7c02 1700 7c00  t...|.d...|...|.
+00000540: 6406 1700 7c02 1700 a102 0100 7118 6400  d...|.......q.d.
+00000550: 5300 2907 4e54 2901 da08 6578 6973 745f  S.).NT)...exist_
+00000560: 6f6b 7a06 2e69 7079 6e62 7a11 6e6f 7465  okz..ipynbz.note
+00000570: 626f 6f6b 5f73 6574 7570 2e70 7946 fa01  book_setup.pyF..
+00000580: 2f29 0772 0e00 0000 da08 6d61 6b65 6469  /).r......makedi
+00000590: 7273 da07 6c69 7374 6469 72da 0570 7269  rs..listdir..pri
+000005a0: 6e74 da08 656e 6473 7769 7468 7212 0000  nt..endswithr...
+000005b0: 0072 1300 0000 2904 5a07 6e65 775f 6469  .r....).Z.new_di
+000005c0: 725a 0c6f 7269 6769 6e61 6c5f 6469 72da  rZ.original_dir.
+000005d0: 0466 696c 65da 0463 6f6e 7472 0900 0000  .file..contr....
+000005e0: 7209 0000 0072 0a00 0000 da0e 636f 7079  r....r......copy
+000005f0: 5f6e 6f74 6562 6f6f 6b73 2a00 0000 7314  _notebooks*...s.
+00000600: 0000 0000 010e 020e 0108 010a 0106 0108  ................
+00000610: 0106 0204 0204 0172 2700 0000 6302 0000  .......r'...c...
+00000620: 0000 0000 0000 0000 0003 0000 0008 0000  ................
+00000630: 0043 0000 0073 3e00 0000 7400 7c00 6401  .C...s>...t.|.d.
+00000640: 1700 6402 8302 8f1c 7d02 7401 a002 7c01  ..d.....}.t...|.
+00000650: 7c02 a102 0100 5700 6400 0400 0400 8303  |.....W.d.......
+00000660: 0100 6e10 3100 7330 3000 0100 0100 0100  ..n.1.s00.......
+00000670: 5900 0100 6400 5300 2903 4efa 132f 6e6f  Y...d.S.).N../no
+00000680: 7465 626f 6f6b 5f64 6174 612e 6a73 6f6e  tebook_data.json
+00000690: da01 7729 03da 046f 7065 6eda 046a 736f  ..w)...open..jso
+000006a0: 6eda 0464 756d 7029 03da 0964 6972 6563  n..dump)...direc
+000006b0: 746f 7279 da04 6461 7461 da01 6672 0900  tory..data..fr..
+000006c0: 0000 7209 0000 0072 0a00 0000 da13 7772  ..r....r......wr
+000006d0: 6974 655f 6e6f 7465 626f 6f6b 5f6a 736f  ite_notebook_jso
+000006e0: 6e3a 0000 0073 0400 0000 0001 1001 7230  n:...s........r0
+000006f0: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+00000700: 0200 0000 0800 0000 4300 0000 733a 0000  ........C...s:..
+00000710: 0074 007c 0064 0117 0083 018f 1a7d 0174  .t.|.d.......}.t
+00000720: 01a0 027c 01a1 0157 0002 0064 0004 0004  ...|...W...d....
+00000730: 0083 0301 0053 0031 0073 2c30 0001 0001  .....S.1.s,0....
+00000740: 0001 0059 0001 0064 0053 0029 024e 7228  ...Y...d.S.).Nr(
+00000750: 0000 0029 0372 2a00 0000 722b 0000 00da  ...).r*...r+....
+00000760: 046c 6f61 6429 0272 2d00 0000 722f 0000  .load).r-...r/..
+00000770: 0072 0900 0000 7209 0000 0072 0a00 0000  .r....r....r....
+00000780: da12 7265 6164 5f6e 6f74 6562 6f6f 6b5f  ..read_notebook_
+00000790: 6a73 6f6e 3f00 0000 7304 0000 0000 010e  json?...s.......
+000007a0: 0172 3200 0000 6300 0000 0000 0000 0000  .r2...c.........
+000007b0: 0000 0006 0000 0004 0000 0043 0000 0073  ...........C...s
+000007c0: ba00 0000 6401 7d00 7400 6a01 7d01 7402  ....d.}.t.j.}.t.
+000007d0: 6a03 a004 7c01 a101 5c02 7d02 7d03 6402  j...|...\.}.}.d.
+000007e0: 7c03 7600 7258 7c03 a005 a100 6403 7600  |.v.rX|.....d.v.
+000007f0: 7234 7c01 7d00 6e0c 7406 6404 7c01 1600  r4|.}.n.t.d.|...
+00000800: 8301 8201 7402 6a03 a007 7c00 a101 7350  ....t.j...|...sP
+00000810: 4a00 8201 6402 7c00 6602 5300 6405 7c03  J...d.|.f.S.d.|.
+00000820: 7600 72b6 7408 7409 a00a 7c01 a101 6a0b  v.r.t.t...|...j.
+00000830: 6406 1900 8301 7d04 7402 a00c 7c04 a101  d.....}.t...|...
+00000840: 7d05 6407 7c05 7600 728e 7c04 6408 1700  }.d.|.v.r.|.d...
+00000850: 7d00 6409 7c05 7600 729e 7c04 640a 1700  }.d.|.v.r.|.d...
+00000860: 7d00 7c00 73ae 7406 640b 7c04 1600 8301  }.|.s.t.d.|.....
+00000870: 8201 6405 7c00 6602 5300 6401 5300 290c  ..d.|.f.S.d.S.).
+00000880: 7aef 5265 7475 726e 2074 6865 2070 6174  z.Return the pat
+00000890: 6820 746f 2074 6865 2070 7974 686f 6e33  h to the python3
+000008a0: 2069 6e74 6572 7072 6574 6572 2e0a 0a20   interpreter... 
+000008b0: 2020 2055 6e64 6572 206c 696e 7578 2073     Under linux s
+000008c0: 7973 2e65 7865 6375 7461 626c 6520 6973  ys.executable is
+000008d0: 2073 6574 2074 6f20 7468 6520 7079 7468   set to the pyth
+000008e0: 6f6e 3320 696e 7465 7270 7265 7465 7220  on3 interpreter 
+000008f0: 7573 6564 2062 7920 5167 6973 2e0a 2020  used by Qgis..  
+00000900: 2020 486f 7765 7665 722c 2075 6e64 6572    However, under
+00000910: 2057 696e 646f 7773 2f4d 6163 2074 6869   Windows/Mac thi
+00000920: 7320 6973 206e 6f74 2074 6865 2063 6173  s is not the cas
+00000930: 6520 616e 6420 7379 732e 6578 6563 7574  e and sys.execut
+00000940: 6162 6c65 2072 6566 6572 7320 746f 2074  able refers to t
+00000950: 6865 0a20 2020 2051 6769 7320 7374 6172  he.    Qgis star
+00000960: 742d 7570 2073 6372 6970 742e 0a20 2020  t-up script..   
+00000970: 204e da06 7079 7468 6f6e 2902 7a0a 7079   N..python).z.py
+00000980: 7468 6f6e 2e65 7865 7a0b 7079 7468 6f6e  thon.exez.python
+00000990: 332e 6578 657a 2755 6e65 7870 6563 7465  3.exez'Unexpecte
+000009a0: 6420 7661 6c75 6520 666f 7220 7379 732e  d value for sys.
+000009b0: 6578 6563 7574 6162 6c65 3a20 2573 5a04  executable: %sZ.
+000009c0: 7167 6973 7201 0000 007a 0b70 7933 5f65  qgisr....z.py3_e
+000009d0: 6e76 2e62 6174 7a0c 2f70 7933 5f65 6e76  nv.batz./py3_env
+000009e0: 2e62 6174 7a13 7079 7468 6f6e 2d71 6769  .batz.python-qgi
+000009f0: 732d 6c74 722e 6261 747a 142f 7079 7468  s-ltr.batz./pyth
+00000a00: 6f6e 2d71 6769 732d 6c74 722e 6261 747a  on-qgis-ltr.batz
+00000a10: 2a63 6f75 6c64 206e 6f74 2066 696e 6420  *could not find 
+00000a20: 7167 6973 2d70 7974 686f 6e20 6261 7420  qgis-python bat 
+00000a30: 6669 6c65 2069 6e3a 2025 7329 0dda 0373  file in: %s)...s
+00000a40: 7973 da0a 6578 6563 7574 6162 6c65 720e  ys..executabler.
+00000a50: 0000 0072 0f00 0000 da05 7370 6c69 74da  ...r......split.
+00000a60: 056c 6f77 6572 da10 456e 7669 726f 6e6d  .lower..Environm
+00000a70: 656e 7445 7272 6f72 da06 6578 6973 7473  entError..exists
+00000a80: da03 7374 72da 0770 6174 686c 6962 7203  ..str..pathlibr.
+00000a90: 0000 00da 0770 6172 656e 7473 7222 0000  .....parentsr"..
+00000aa0: 0029 065a 0b69 6e74 6572 7072 6574 6572  .).Z.interpreter
+00000ab0: 7235 0000 0072 2d00 0000 da08 6669 6c65  r5...r-.....file
+00000ac0: 6e61 6d65 5a0b 6d61 696e 5f66 6f6c 6465  nameZ.main_folde
+00000ad0: 725a 0c66 6f6c 6465 725f 6669 6c65 7372  rZ.folder_filesr
+00000ae0: 0900 0000 7209 0000 0072 0a00 0000 da17  ....r....r......
+00000af0: 5f67 6574 5f70 7974 686f 6e5f 696e 7465  _get_python_inte
+00000b00: 7270 7265 7465 7244 0000 0073 2e00 0000  rpreterD...s....
+00000b10: 0007 0401 0601 1001 0802 0c01 0602 0201  ................
+00000b20: 06ff 0403 1001 0802 0802 1401 0a02 0801  ................
+00000b30: 0802 0801 0802 0401 0201 06ff 0404 723e  ..............r>
+00000b40: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00000b50: 0100 0000 0400 0000 4300 0000 7330 0000  ........C...s0..
+00000b60: 0074 00a0 01a1 00a0 0264 0164 02a1 027d  .t.......d.d...}
+00000b70: 0074 036a 04a0 057c 0064 0317 00a1 0172  .t.j...|.d.....r
+00000b80: 287c 0064 0317 0053 0064 0053 0064 0053  (|.d...S.d.S.d.S
+00000b90: 0029 044e fa0d 7369 7465 2d70 6163 6b61  .).N..site-packa
+00000ba0: 6765 73da 0753 6372 6970 7473 7a10 2f6a  ges..Scriptsz./j
+00000bb0: 7570 7974 6572 2d6c 6162 2e65 7865 a906  upyter-lab.exe..
+00000bc0: da04 7369 7465 da13 6765 7475 7365 7273  ..site..getusers
+00000bd0: 6974 6570 6163 6b61 6765 73da 0772 6570  itepackages..rep
+00000be0: 6c61 6365 720e 0000 0072 0f00 0000 7239  lacer....r....r9
+00000bf0: 0000 00a9 0172 0f00 0000 7209 0000 0072  .....r....r....r
+00000c00: 0900 0000 720a 0000 00da 1c75 7365 725f  ....r......user_
+00000c10: 696e 7374 616c 6c65 645f 6e6f 7465 626f  installed_notebo
+00000c20: 6f6b 5f70 6174 686c 0000 0073 0800 0000  ok_pathl...s....
+00000c30: 0001 1001 1001 0802 7246 0000 0063 0000  ........rF...c..
+00000c40: 0000 0000 0000 0000 0000 0100 0000 0400  ................
+00000c50: 0000 4300 0000 7330 0000 0074 00a0 01a1  ..C...s0...t....
+00000c60: 00a0 0264 0164 02a1 027d 0074 036a 04a0  ...d.d...}.t.j..
+00000c70: 057c 0064 0317 00a1 0172 287c 0064 0317  .|.d.....r(|.d..
+00000c80: 0053 0064 0053 0064 0053 0029 044e 723f  .S.d.S.d.S.).Nr?
+00000c90: 0000 0072 4000 0000 7a0c 2f69 7079 7468  ...r@...z./ipyth
+00000ca0: 6f6e 2e65 7865 7241 0000 0072 4500 0000  on.exerA...rE...
+00000cb0: 7209 0000 0072 0900 0000 720a 0000 00da  r....r....r.....
+00000cc0: 1b75 7365 725f 696e 7374 616c 6c65 645f  .user_installed_
+00000cd0: 6970 7974 686f 6e5f 7061 7468 7400 0000  ipython_patht...
+00000ce0: 7308 0000 0000 0110 0110 0108 0272 4700  s............rG.
+00000cf0: 0000 da05 6f73 6765 6f46 6302 0000 0000  ....osgeoFc.....
+00000d00: 0000 0000 0000 0005 0000 0003 0000 0043  ...............C
+00000d10: 0000 0073 3c00 0000 7400 8300 5c02 7d02  ...s<...t...\.}.
+00000d20: 7d03 7c00 6401 6b02 721e 7c03 6402 6403  }.|.d.k.r.|.d.d.
+00000d30: 6703 7d04 6e1a 7c01 722e 7c03 7401 8300  g.}.n.|.r.|.t...
+00000d40: 6702 7d04 6e0a 7c03 7402 8300 6702 7d04  g.}.n.|.t...g.}.
+00000d50: 7c04 5300 2904 7aa9 6966 206a 7570 7974  |.S.).z.if jupyt
+00000d60: 6572 2069 7320 696e 7374 616c 6c65 6420  er is installed 
+00000d70: 696e 206f 7367 656f 2c20 7573 6520 6f73  in osgeo, use os
+00000d80: 6765 6f2e 0a20 2020 2069 6620 6a75 7079  geo..    if jupy
+00000d90: 7465 7220 6973 2069 6e73 7461 6c6c 6564  ter is installed
+00000da0: 2069 6e20 7468 6520 7573 6572 2064 6972   in the user dir
+00000db0: 2027 7069 7020 696e 7374 616c 6c20 6a75   'pip install ju
+00000dc0: 7079 7465 7220 2d2d 7573 6572 270a 2020  pyter --user'.  
+00000dd0: 2020 7573 6520 2775 7365 7227 2e0a 0a20    use 'user'... 
+00000de0: 2020 2027 7573 6572 2720 7573 6573 2061     'user' uses a
+00000df0: 6e20 6578 6563 7475 6162 6c65 0a20 2020  n exectuable.   
+00000e00: 2072 4800 0000 7a02 2d6d 7a0b 6a75 7079   rH...z.-mz.jupy
+00000e10: 7465 722d 6c61 6229 0372 3e00 0000 7247  ter-lab).r>...rG
+00000e20: 0000 0072 4600 0000 2905 da08 6c6f 6361  ...rF...)...loca
+00000e30: 7469 6f6e da07 6970 7974 686f 6eda 0673  tion..ipython..s
+00000e40: 7973 7465 6d5a 1270 7974 686f 6e5f 696e  ystemZ.python_in
+00000e50: 7465 7270 7265 7465 72da 0763 6f6d 6d61  terpreter..comma
+00000e60: 6e64 7209 0000 0072 0900 0000 720a 0000  ndr....r....r...
+00000e70: 00da 106e 6f74 6562 6f6f 6b5f 636f 6d6d  ...notebook_comm
+00000e80: 616e 647c 0000 0073 0e00 0000 0007 0a01  and|...s........
+00000e90: 0801 0c07 0401 0c02 0a01 724d 0000 00da  ..........rM....
+00000ea0: 0372 756e 6304 0000 0000 0000 0000 0000  .runc...........
+00000eb0: 0008 0000 000a 0000 0043 0000 0073 0001  .........C...s..
+00000ec0: 0000 6401 6402 8400 7400 6a01 a002 6403  ..d.d...t.j...d.
+00000ed0: a101 a003 7400 6a04 a101 4400 8301 7d04  ....t.j...D...}.
+00000ee0: 7c03 4400 5d36 7d05 7405 7c05 8301 7d05  |.D.]6}.t.|...}.
+00000ef0: 7c05 7c04 7601 7222 7c05 a006 a100 9b00  |.|.v.r"|.......
+00000f00: 7400 6a04 9b00 7400 6a01 6403 1900 9b00  t.j...t.j.d.....
+00000f10: 9d03 7400 6a01 6403 3c00 7122 7407 6404  ..t.j.d.<.q"t.d.
+00000f20: 7400 6a01 a002 6403 a101 a003 7400 6a04  t.j...d.....t.j.
+00000f30: a101 9b00 9d02 8301 0100 7408 7c01 8301  ..........t.|...
+00000f40: 7d06 7c00 728e 7c06 a009 7c00 a101 0100  }.|.r.|...|.....
+00000f50: 7c02 6405 6b02 72cc 740a 6a0b 7c06 6406  |.d.k.r.t.j.|.d.
+00000f60: 6406 6407 6407 6407 6406 740c 740d 4200  d.d.d.d.d.t.t.B.
+00000f70: 6408 8d08 7d07 7407 6409 7c07 6a0e 9b00  d...}.t.d.|.j...
+00000f80: 640a 7c06 9b00 9d04 8301 0100 6e30 7c02  d.|.........n0|.
+00000f90: 640b 6b02 72fc 6700 640c a201 7c06 1700  d.k.r.g.d...|...
+00000fa0: 7d06 740a 6a0f 7c06 6406 640d 8d02 7d07  }.t.j.|.d.d...}.
+00000fb0: 7407 640e 7c06 9b00 9d02 8301 0100 6407  t.d.|.........d.
+00000fc0: 5300 290f 7ae9 6469 7265 6374 6f72 793a  S.).z.directory:
+00000fd0: 0a20 2020 2020 2020 206e 6f74 6562 6f6f  .        noteboo
+00000fe0: 6b73 206f 7065 6e20 696e 2061 2063 6572  ks open in a cer
+00000ff0: 7461 696e 2064 6972 6563 746f 7279 0a20  tain directory. 
+00001000: 2020 206c 6f63 6174 696f 6e3a 0a20 2020     location:.   
+00001010: 2020 2020 2063 616e 2065 6974 6865 7220       can either 
+00001020: 6265 2027 6f73 6765 6f27 206f 7220 2775  be 'osgeo' or 'u
+00001030: 7365 7227 0a20 2020 2020 2020 206f 7065  ser'.        ope
+00001040: 6e20 6a75 7079 7465 7220 6e6f 7465 626f  n jupyter notebo
+00001050: 6f6b 2069 7320 6f73 6765 6f20 6f72 2070  ok is osgeo or p
+00001060: 6572 2d75 7365 722d 696e 7374 616c 6c65  er-user-installe
+00001070: 6420 2e65 7865 0a20 2020 2075 7365 3a0a  d .exe.    use:.
+00001080: 2020 2020 2020 2020 7375 6270 726f 6365          subproce
+00001090: 7373 206d 6f64 6520 2827 706f 7065 6e27  ss mode ('popen'
+000010a0: 206f 7220 2772 756e 2729 0a20 2020 2063   or 'run').    c
+000010b0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+000010c0: 0400 0000 5300 0000 7314 0000 0067 007c  ....S...s....g.|
+000010d0: 005d 0c7d 0174 007c 0183 0191 0271 0453  .].}.t.|.....q.S
+000010e0: 0072 0900 0000 7202 0000 0029 02da 022e  .r....r....)....
+000010f0: 30da 0169 7209 0000 0072 0900 0000 720a  0..ir....r....r.
+00001100: 0000 00da 0a3c 6c69 7374 636f 6d70 3e9b  .....<listcomp>.
+00001110: 0000 00f3 0000 0000 7a1f 6f70 656e 5f73  ........z.open_s
+00001120: 6572 7665 722e 3c6c 6f63 616c 733e 2e3c  erver.<locals>.<
+00001130: 6c69 7374 636f 6d70 3eda 0450 4154 487a  listcomp>..PATHz
+00001140: 0670 6174 6820 3ada 0570 6f70 656e 544e  .path :..popenTN
+00001150: 2907 da05 7368 656c 6cda 1275 6e69 7665  )...shell..unive
+00001160: 7273 616c 5f6e 6577 6c69 6e65 73da 0573  rsal_newlines..s
+00001170: 7464 696e da06 7374 646f 7574 da06 7374  tdin..stdout..st
+00001180: 6465 7272 da09 636c 6f73 655f 6664 73da  derr..close_fds.
+00001190: 0d63 7265 6174 696f 6e66 6c61 6773 7a1d  .creationflagsz.
+000011a0: 5374 6172 7465 6420 7072 6f63 6573 7369  Started processi
+000011b0: 6e67 2077 6974 6820 7069 643a 207a 0d20  ng with pid: z. 
+000011c0: 616e 6420 636f 6d6d 616e 6420 724e 0000  and command rN..
+000011d0: 0029 03da 0573 7461 7274 da03 636d 647a  .)...start..cmdz
+000011e0: 022f 4ba9 0172 5500 0000 7a20 5374 6172  ./K..rU...z Star
+000011f0: 7465 6420 7072 6f63 6573 7369 6e67 2077  ted processing w
+00001200: 6974 6820 636f 6d6d 616e 6420 2910 720e  ith command ).r.
+00001210: 0000 00da 0765 6e76 6972 6f6e da03 6765  .....environ..ge
+00001220: 7472 3600 0000 da07 7061 7468 7365 7072  tr6.....pathsepr
+00001230: 0300 0000 da08 6173 5f70 6f73 6978 7223  ......as_posixr#
+00001240: 0000 0072 4d00 0000 da06 6170 7065 6e64  ...rM.....append
+00001250: da0a 7375 6270 726f 6365 7373 da05 506f  ..subprocess..Po
+00001260: 7065 6eda 1044 4554 4143 4845 445f 5052  pen..DETACHED_PR
+00001270: 4f43 4553 53da 1843 5245 4154 455f 4e45  OCESS..CREATE_NE
+00001280: 575f 5052 4f43 4553 535f 4752 4f55 50da  W_PROCESS_GROUP.
+00001290: 0370 6964 724e 0000 0029 0872 2d00 0000  .pidrN...).r-...
+000012a0: 7249 0000 00da 0375 7365 5a0e 6e6f 7465  rI.....useZ.note
+000012b0: 626f 6f6b 5f70 6174 6873 da05 7061 7468  book_paths..path
+000012c0: 7372 0f00 0000 724c 0000 00da 0770 726f  sr....rL.....pro
+000012d0: 6365 7373 7209 0000 0072 0900 0000 720a  cessr....r....r.
+000012e0: 0000 00da 0b6f 7065 6e5f 7365 7276 6572  .....open_server
+000012f0: 9200 0000 7332 0000 0000 091e 0108 0108  ....s2..........
+00001300: 0108 0124 011e 0108 0204 010a 0208 0104  ...$............
+00001310: 0102 0102 0102 0102 0102 0102 0102 0106  ................
+00001320: f806 0a18 0108 010c 010e 0172 6c00 0000  ...........rl...
+00001330: 6302 0000 0000 0000 0000 0000 0004 0000  c...............
+00001340: 0008 0000 0043 0000 0073 4600 0000 7400  .....C...sF...t.
+00001350: 7c01 8301 7d02 7401 7c00 6401 8302 8f20  |...}.t.|.d.... 
+00001360: 7d03 7c03 a002 6402 a003 7c02 a101 a101  }.|...d...|.....
+00001370: 0100 5700 6400 0400 0400 8303 0100 6e10  ..W.d.........n.
+00001380: 3100 7338 3000 0100 0100 0100 5900 0100  1.s80.......Y...
+00001390: 6400 5300 2903 4e72 2900 0000 fa01 2029  d.S.).Nr)..... )
+000013a0: 0472 4d00 0000 722a 0000 00da 0577 7269  .rM...r*.....wri
+000013b0: 7465 7211 0000 0029 0472 0f00 0000 7249  ter....).r....rI
+000013c0: 0000 0072 4c00 0000 5a08 6261 745f 6669  ...rL...Z.bat_fi
+000013d0: 6c65 7209 0000 0072 0900 0000 720a 0000  ler....r....r...
+000013e0: 00da 1763 7265 6174 655f 636f 6d6d 616e  ...create_comman
+000013f0: 645f 6261 745f 6669 6c65 b800 0000 7306  d_bat_file....s.
+00001400: 0000 0000 0108 020c 0172 6f00 0000 6301  .........ro...c.
+00001410: 0000 0000 0000 0000 0000 000a 0000 0008  ................
+00001420: 0000 0043 0000 0073 1a01 0000 7400 6a01  ...C...s....t.j.
+00001430: 6401 1900 7d01 7c01 6402 1700 7d02 6403  d...}.|.d...}.d.
+00001440: 7d03 7c00 4400 5d20 7d04 7c04 a002 6404  }.|.D.] }.|...d.
+00001450: 6405 a102 7d04 7c03 6406 7c04 9b00 6407  d...}.|.d.|...d.
+00001460: 9d03 1700 7d03 711a 6408 7c03 9b00 6409  ....}.q.d.|...d.
+00001470: 9d03 7d05 7400 6a03 a004 7c02 a101 7384  ..}.t.j...|...s.
+00001480: 7405 640a 640b 640c 8d02 7d06 7c06 640d  t.d.d.d...}.|.d.
+00001490: 1900 640e 1700 7d06 7406 6a07 7c06 640b  ..d...}.t.j.|.d.
+000014a0: 640f 8d02 0100 7408 6410 7c06 8302 0100  d.....t.d.|.....
+000014b0: 6411 7d07 7409 7c02 6412 8302 8f2a 7d08  d.}.t.|.d....*}.
+000014c0: 7c08 4400 5d14 7d09 7c05 7c08 7600 7298  |.D.].}.|.|.v.r.
+000014d0: 640b 7d07 0100 71ae 7198 5700 6413 0400  d.}...q.q.W.d...
+000014e0: 0400 8303 0100 6e10 3100 73c2 3000 0100  ......n.1.s.0...
+000014f0: 0100 0100 5900 0100 7c07 9001 7316 7408  ....Y...|...s.t.
+00001500: 6414 7c05 8302 0100 7409 7c02 6415 8302  d.|.....t.|.d...
+00001510: 8f1e 7d08 7c08 a00a 6416 7c05 1700 a101  ..}.|...d.|.....
+00001520: 0100 5700 6413 0400 0400 8303 0100 6e12  ..W.d.........n.
+00001530: 3100 9001 730c 3000 0100 0100 0100 5900  1...s.0.......Y.
+00001540: 0100 6413 5300 2917 7a36 6164 6473 2065  ..d.S.).z6adds e
+00001550: 7874 7261 206e 6f74 6562 6f6f 6b20 7061  xtra notebook pa
+00001560: 7468 732c 2077 6869 6368 2069 7320 7573  ths, which is us
+00001570: 6564 2069 6e20 7468 6520 706c 7567 696e  ed in the plugin
+00001580: da0b 5553 4552 5052 4f46 494c 457a 2b2f  ..USERPROFILEz+/
+00001590: 2e69 7079 7468 6f6e 2f70 726f 6669 6c65  .ipython/profile
+000015a0: 5f64 6566 6175 6c74 2f69 7079 7468 6f6e  _default/ipython
+000015b0: 5f63 6f6e 6669 672e 7079 7a0a 696d 706f  _config.pyz.impo
+000015c0: 7274 2073 7973 fa01 5c72 2000 0000 7a15  rt sys..\r ...z.
+000015d0: 3b20 7379 732e 7061 7468 2e69 6e73 6572  ; sys.path.inser
+000015e0: 7428 302c 227a 0222 297a 2563 2e49 6e74  t(0,"z.")z%c.Int
+000015f0: 6572 6163 7469 7665 5368 656c 6c41 7070  eractiveShellApp
+00001600: 2e65 7865 635f 6c69 6e65 7320 3d20 5b27  .exec_lines = ['
+00001610: 7a02 275d da04 7573 6572 5429 0172 4a00  z.']..userT).rJ.
+00001620: 0000 e901 0000 007a 0f20 7072 6f66 696c  .......z. profil
+00001630: 6520 6372 6561 7465 725e 0000 007a 1743  e creater^...z.C
+00001640: 7265 6174 696e 6720 7072 6f66 696c 6520  reating profile 
+00001650: 7769 7468 3a20 46da 0172 4e7a 0741 6464  with: F..rNz.Add
+00001660: 696e 673a da01 61da 010a 290b 720e 0000  ing:..a...).r...
+00001670: 0072 5f00 0000 7244 0000 0072 0f00 0000  .r_...rD...r....
+00001680: 7239 0000 0072 4d00 0000 7264 0000 0072  r9...rM...rd...r
+00001690: 4e00 0000 7223 0000 0072 2a00 0000 726e  N...r#...r*...rn
+000016a0: 0000 0029 0a5a 1465 7874 7261 5f6e 6f74  ...).Z.extra_not
+000016b0: 6562 6f6f 6b5f 7061 7468 735a 1175 7365  ebook_pathsZ.use
+000016c0: 725f 7072 6f66 696c 655f 7061 7468 5a14  r_profile_pathZ.
+000016d0: 6970 7974 686f 6e5f 7072 6f66 696c 655f  ipython_profile_
+000016e0: 7061 7468 5a0f 6e62 5f70 6174 685f 636f  pathZ.nb_path_co
+000016f0: 6d6d 616e 6472 0f00 0000 5a09 6e62 5f73  mmandr....Z.nb_s
+00001700: 7472 696e 6772 4c00 0000 7239 0000 005a  tringrL...r9...Z
+00001710: 0c70 726f 6669 6c65 5f63 6f64 6572 5000  .profile_coderP.
+00001720: 0000 7209 0000 0072 0900 0000 720a 0000  ..r....r....r...
+00001730: 00da 1261 6464 5f6e 6f74 6562 6f6f 6b5f  ...add_notebook_
+00001740: 7061 7468 73c0 0000 0073 2e00 0000 0004  paths....s......
+00001750: 0a02 06ff 0204 0401 0801 0c01 1201 0c02  ................
+00001760: 0c02 0c01 0c02 0e01 0a08 0401 0c01 0801  ................
+00001770: 0801 0401 2402 0601 0a01 0c01 7277 0000  ....$.......rw..
+00001780: 0029 0272 4800 0000 4629 0172 4800 0000  .).rH...F).rH...
+00001790: 291c da07 5f5f 646f 635f 5f72 0e00 0000  )...__doc__r....
+000017a0: 7234 0000 0072 6400 0000 723b 0000 0072  r4...rd...r;...r
+000017b0: 0c00 0000 7212 0000 0072 2b00 0000 7242  ....r....r+...rB
+000017c0: 0000 0072 0300 0000 7267 0000 0072 6600  ...r....rg...rf.
+000017d0: 0000 723a 0000 00da 085f 5f66 696c 655f  ..r:.....__file_
+000017e0: 5fda 0670 6172 656e 74da 0861 6273 6f6c  _..parent..absol
+000017f0: 7574 655a 124e 4f54 4542 4f4f 4b5f 4449  uteZ.NOTEBOOK_DI
+00001800: 5245 4354 4f52 5972 0500 0000 7227 0000  RECTORYr....r'..
+00001810: 0072 3000 0000 7232 0000 0072 3e00 0000  .r0...r2...r>...
+00001820: 7246 0000 0072 4700 0000 724d 0000 0072  rF...rG...rM...r
+00001830: 6c00 0000 726f 0000 0072 7700 0000 7209  l...ro...rw...r.
+00001840: 0000 0072 0900 0000 7209 0000 0072 0a00  ...r....r....r..
+00001850: 0000 da08 3c6d 6f64 756c 653e 0300 0000  ....<module>....
+00001860: 732e 0000 0004 0808 0108 0108 0108 0108  s...............
+00001870: 0108 0108 0108 010c 0204 0104 0214 030e  ................
+00001880: 0f0c 1008 0508 0508 2808 0808 080a 1612  ........(.......
+00001890: 260a 08                                  &..
```

### Comparing `hhnk-threedi-tools-2023.2/hhnk_threedi_tools/utils/notebooks/run.py` & `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/notebooks/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,23 @@
         os.remove(self.path)
 
 
 def copy_notebooks(new_dir, original_dir=NOTEBOOK_DIRECTORY):
     os.makedirs(new_dir, exist_ok=True)
 
     for file in os.listdir(original_dir):
+        print(file)
         if file.endswith(".ipynb"):
+            cont=True
+        elif file == "notebook_setup.py":
+            cont=True
+        else:
+            cont=False
+
+        if cont:
             shutil.copy2(original_dir + "/" + file, new_dir + "/" + file)
 
 
 def write_notebook_json(directory, data):
     with open(directory + "/notebook_data.json", "w") as f:
         json.dump(data, f)
 
@@ -176,14 +184,15 @@
 def create_command_bat_file(path, location="osgeo"):
     command = notebook_command(location)
 
     with open(path, "w") as bat_file:
         bat_file.write(" ".join(command))
 
 
+#TODO this doesnt work nicely with other  environments. Prepare for deprecation
 def add_notebook_paths(extra_notebook_paths):
     """adds extra notebook paths, which is used in the plugin"""
 
     # user profile paths
     user_profile_path = os.environ["USERPROFILE"]
     ipython_profile_path = (
         user_profile_path + "/.ipython/profile_default/ipython_config.py"
```

### Comparing `hhnk-threedi-tools-2023.2/hhnk_threedi_tools/utils/queries.py` & `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/queries.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.2/hhnk_threedi_tools/utils/queries_general_checks.py` & `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/queries_general_checks.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.2/hhnk_threedi_tools/variables/api_settings.py` & `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/variables/api_settings.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.2/hhnk_threedi_tools/variables/bank_levels.py` & `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/variables/bank_levels.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.2/hhnk_threedi_tools/variables/database_aliases.py` & `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/variables/database_aliases.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.2/hhnk_threedi_tools/variables/database_variables.py` & `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/variables/database_variables.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.2/hhnk_threedi_tools/variables/model_state.py` & `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/variables/model_state.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.2/hhnk_threedi_tools/variables/one_d_two_d.py` & `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/variables/one_d_two_d.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.2/hhnk_threedi_tools/variables/sqlite.py` & `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/variables/sqlite.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.2/hhnk_threedi_tools/variables/zero_d_one_d.py` & `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/variables/zero_d_one_d.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.2/hhnk_threedi_tools.egg-info/PKG-INFO` & `hhnk-threedi-tools-2023.3/hhnk_threedi_tools.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: hhnk-threedi-tools
-Version: 2023.2
+Version: 2023.3
 Summary: HHNK watersystemen analysis tools
 Home-page: https://github.com/threedi/hhnk-threedi-tools
 Author: Wietse van Gerwen, Laure Ravier
 Author-email: w.vangerwen@hhnk.nl
 Maintainer: Wietse van Gerwen
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/threedi/hhnk-threedi-tools/issues
-Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
+
+UNKNOWN
+
```

### Comparing `hhnk-threedi-tools-2023.2/hhnk_threedi_tools.egg-info/SOURCES.txt` & `hhnk-threedi-tools-2023.3/hhnk_threedi_tools.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -5,22 +5,21 @@
 hhnk_threedi_tools.egg-info/PKG-INFO
 hhnk_threedi_tools.egg-info/SOURCES.txt
 hhnk_threedi_tools.egg-info/dependency_links.txt
 hhnk_threedi_tools.egg-info/top_level.txt
 hhnk_threedi_tools/core/__init__.py
 hhnk_threedi_tools/core/folder_helpers.py
 hhnk_threedi_tools/core/folders.py
+hhnk_threedi_tools/core/migrate_schematisation.py
 hhnk_threedi_tools/core/api/__init__.py
 hhnk_threedi_tools/core/api/calculation.py
-hhnk_threedi_tools/core/api/calculation_functions.py
 hhnk_threedi_tools/core/api/calculation_gui_class.py
 hhnk_threedi_tools/core/api/download_functions.py
 hhnk_threedi_tools/core/api/download_gui_class.py
 hhnk_threedi_tools/core/api/downloader.py
-hhnk_threedi_tools/core/api/read_api_file.py
 hhnk_threedi_tools/core/api/upload_model/__init__.py
 hhnk_threedi_tools/core/api/upload_model/constants.py
 hhnk_threedi_tools/core/api/upload_model/download.py
 hhnk_threedi_tools/core/api/upload_model/login.py
 hhnk_threedi_tools/core/api/upload_model/simulate.py
 hhnk_threedi_tools/core/api/upload_model/threedi_calls.py
 hhnk_threedi_tools/core/api/upload_model/upload.py
@@ -40,15 +39,17 @@
 hhnk_threedi_tools/core/climate_scenarios/klimaatsommen_prep.py
 hhnk_threedi_tools/core/climate_scenarios/maskerkaart.py
 hhnk_threedi_tools/core/climate_scenarios/maskerkaart_raster.py
 hhnk_threedi_tools/core/climate_scenarios/peilgebieden.py
 hhnk_threedi_tools/core/climate_scenarios/ruimtekaart.py
 hhnk_threedi_tools/core/climate_scenarios/schadekaart.py
 hhnk_threedi_tools/core/climate_scenarios/schadekaart_peilgebieden.py
-hhnk_threedi_tools/resources/Thumbs.db
+hhnk_threedi_tools/core/result_rasters/__init__.py
+hhnk_threedi_tools/core/result_rasters/calculate_raster.py
+hhnk_threedi_tools/core/result_rasters/netcdf_to_gridgpkg.py
 hhnk_threedi_tools/resources/__init__.py
 hhnk_threedi_tools/resources/model_settings.xlsx
 hhnk_threedi_tools/resources/model_settings_default.xlsx
 hhnk_threedi_tools/resources/precipitation_frequency.xlsx
 hhnk_threedi_tools/resources/precipitation_zones_hhnk.tif
 hhnk_threedi_tools/resources/__pycache__/__init__.cpython-37.pyc
 hhnk_threedi_tools/resources/__pycache__/__init__.cpython-39.pyc
@@ -64,20 +65,22 @@
 hhnk_threedi_tools/utils/notebooks/01_calculation_gui.ipynb
 hhnk_threedi_tools/utils/notebooks/02_download_gui.ipynb
 hhnk_threedi_tools/utils/notebooks/03_nabewerking_klimaatsommen.ipynb
 hhnk_threedi_tools/utils/notebooks/04_netcdf_naar_raster.ipynb
 hhnk_threedi_tools/utils/notebooks/05_sqlite_create_grid.ipynb
 hhnk_threedi_tools/utils/notebooks/__init__.py
 hhnk_threedi_tools/utils/notebooks/constants.py
+hhnk_threedi_tools/utils/notebooks/notebook_data.json
+hhnk_threedi_tools/utils/notebooks/notebook_setup.py
 hhnk_threedi_tools/utils/notebooks/run.py
-hhnk_threedi_tools/utils/notebooks/test.py
 hhnk_threedi_tools/utils/notebooks/.ipynb_checkpoints/01_calculation_gui-checkpoint.ipynb
 hhnk_threedi_tools/utils/notebooks/.ipynb_checkpoints/02_download_gui-checkpoint.ipynb
 hhnk_threedi_tools/utils/notebooks/__pycache__/__init__.cpython-37.pyc
 hhnk_threedi_tools/utils/notebooks/__pycache__/__init__.cpython-39.pyc
+hhnk_threedi_tools/utils/notebooks/__pycache__/notebook_setup.cpython-39.pyc
 hhnk_threedi_tools/utils/notebooks/__pycache__/run.cpython-37.pyc
 hhnk_threedi_tools/utils/notebooks/__pycache__/run.cpython-39.pyc
 hhnk_threedi_tools/variables/__init__.py
 hhnk_threedi_tools/variables/api_settings.py
 hhnk_threedi_tools/variables/backups_table_names.py
 hhnk_threedi_tools/variables/bank_levels.py
 hhnk_threedi_tools/variables/damo_hdb_datachecker_variables.py
@@ -87,17 +90,15 @@
 hhnk_threedi_tools/variables/default_variables.py
 hhnk_threedi_tools/variables/definitions.py
 hhnk_threedi_tools/variables/model_state.py
 hhnk_threedi_tools/variables/one_d_two_d.py
 hhnk_threedi_tools/variables/sqlite.py
 hhnk_threedi_tools/variables/weirs.py
 hhnk_threedi_tools/variables/zero_d_one_d.py
-tests/__init__.py
-tests/config.py
-tests/rtest_klimaatsommen_prep.py
-tests/rtest_notebooks.py
-tests/set_local_paths.py
-tests/test_bank_level_test.py
+tests/test_bank_level_check.py
 tests/test_folder_structures.py
+tests/test_klimaatsommen_prep.py
 tests/test_one_d_two_d.py
+tests/test_result_rasters.py
+tests/test_schema_migration.py
 tests/test_sqlite.py
 tests/test_zero_d_one_d.py
```

### Comparing `hhnk-threedi-tools-2023.2/tests/rtest_klimaatsommen_prep.py` & `hhnk-threedi-tools-2023.3/tests/test_klimaatsommen_prep.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,54 @@
 # %%
-# -*- coding: utf-8 -*-
-if __name__ == "__main__":
-    import set_local_paths  # add local git repos.
-
 # First-party imports
-import pathlib
 import pandas as pd
-from pathlib import Path
+import shutil
+import pytest
 
 # Local imports
 from hhnk_threedi_tools.core.climate_scenarios.klimaatsommen_prep import KlimaatsommenPrep
 from hhnk_threedi_tools.core.folders import Folders
+from hhnk_threedi_tools.core.folder_helpers import ClimateResult
+import hhnk_research_tools as hrt
 
 
-TEST_MODEL = pathlib.Path(__file__).parent.absolute() / "data/model_test/"
+from tests.config import FOLDER_TEST, TEMP_DIR, TEST_DIRECTORY
 
+def test_klimaatsommenprep_verify():
+    """Raises because not all 18 scenarios downloaded"""
+    with pytest.raises(Exception):
+        klimaatsommenprep = KlimaatsommenPrep(folder=FOLDER_TEST,
+            batch_name="batch_test",
+            cfg_file = 'cfg_lizard.cfg',
+            landuse_file = FOLDER_TEST.model.schema_base.rasters.landuse,
+            verify=True
+        )
 
 def test_klimaatsommenprep():
-
-    folder = Folders(TEST_MODEL)
-
-    SCHADESCHATTER_PATH=Path(r"E:\01.basisgegevens\hhnk_schadeschatter") #TODO naar een localsettings oid verplaatsen?
-
-    klimaatsommenrep = KlimaatsommenPrep(folder=folder,
+    klimaatsommenprep = KlimaatsommenPrep(folder=FOLDER_TEST,
         batch_name="batch_test",
-        cfg_file = SCHADESCHATTER_PATH/'01_data/cfg/cfg_lizard.cfg',
-        landuse_file = r"\\corp.hhnk.nl\data\Hydrologen_data\Data\01.basisgegevens\rasters\landgebruik\landuse2019_tiles\combined_rasters.vrt",
-        SCHADESCHATTER_PATH=SCHADESCHATTER_PATH
+        cfg_file = 'cfg_lizard.cfg',
+        landuse_file = FOLDER_TEST.model.schema_base.rasters.landuse,
+        verify=False
     )
     
-    klimaatsommenrep.run(overwrite=False) #TODO =True, maar test duurt lang
+    #Rebase the batch_fd so it will always create all output.
+    batch_test = TEMP_DIR/f"batch_test_{hrt.get_uuid()}"
+    batch_test = ClimateResult(batch_test)
+    shutil.copytree(src=klimaatsommenprep.batch_fd.downloads.piek_glg_T10.netcdf.pl,
+                    dst=batch_test.downloads.piek_glg_T10.netcdf.pl)
+    klimaatsommenprep.batch_fd = batch_test
+    
+    #Run test
+    klimaatsommenprep.run(overwrite=True, testing=True)
 
+    #check results
     for raster_type in ["depth_max", "damage_total"]:
-        scenario_metadata = pd.read_csv(klimaatsommenrep.info_file[raster_type], sep=";")
-        assertion_metadata = pd.read_csv(klimaatsommenrep.info_file[raster_type].with_stem(f"{raster_type}_info_expected"), sep=";")
+        scenario_metadata = pd.read_csv(klimaatsommenprep.info_file[raster_type], sep=";")
+        assertion_metadata = pd.read_csv(TEST_DIRECTORY/fr"test_klimaatsommen/{raster_type}_info_expected.csv", sep=";")
         # scenario_metadata = damage_data.drop(['Unnamed: 0'], axis=1)
         # damage_data.set_index(['file name'], inplace = True)
 
         pd.testing.assert_frame_equal(scenario_metadata, assertion_metadata)
 
 
 # %%
```

### Comparing `hhnk-threedi-tools-2023.2/tests/test_folder_structures.py` & `hhnk-threedi-tools-2023.3/tests/test_folder_structures.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import shutil
 from pathlib import Path
 from hhnk_threedi_tools.core.folders import Folders
 
 
 SUB_FOLDERS = ["01_source_data", "02_schematisation", "03_3di_results", "04_test_results"]
 
-from .config import FOLDER_TEST, PATH_TEST_MODEL, \
+from tests.config import FOLDER_TEST, PATH_TEST_MODEL, \
                         FOLDER_NEW, PATH_NEW_FOLDER
 
 class TestFolder:
 
     def test_create_project(self):
         """tests if a new project folders are created"""
         # create a project without creating sub-dirs
```

