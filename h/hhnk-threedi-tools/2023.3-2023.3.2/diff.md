# Comparing `tmp/hhnk-threedi-tools-2023.3.tar.gz` & `tmp/hhnk-threedi-tools-2023.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hhnk-threedi-tools-2023.3.tar", last modified: Fri Jun 23 05:21:49 2023, max compression
+gzip compressed data, was "hhnk-threedi-tools-2023.3.2.tar", last modified: Fri Jun 23 11:30:42 2023, max compression
```

## Comparing `hhnk-threedi-tools-2023.3.tar` & `hhnk-threedi-tools-2023.3.2.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 05:21:44.779554 hhnk-threedi-tools-2023.3/
--rw-rw-rw-   0        0        0      245 2023-06-19 15:02:38.000000 hhnk-threedi-tools-2023.3/MANIFEST.in
--rw-rw-rw-   0        0        0      578 2023-06-23 05:21:49.166687 hhnk-threedi-tools-2023.3/PKG-INFO
--rw-rw-rw-   0        0        0      349 2023-06-12 13:52:12.000000 hhnk-threedi-tools-2023.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-23 05:21:44.801554 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/
--rw-rw-rw-   0        0        0     1509 2023-06-21 07:44:04.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-23 05:21:45.060558 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/
--rw-rw-rw-   0        0        0       50 2021-12-13 08:25:18.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-23 05:21:45.247561 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/api/
--rw-rw-rw-   0        0        0        0 2021-12-13 08:25:18.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/api/__init__.py
--rw-rw-rw-   0        0        0    32989 2023-05-03 08:34:10.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/api/calculation.py
--rw-rw-rw-   0        0        0    82230 2023-06-16 09:23:43.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/api/calculation_gui_class.py
--rw-rw-rw-   0        0        0     2911 2023-05-03 08:34:10.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/api/download_functions.py
--rw-rw-rw-   0        0        0    57886 2023-06-16 09:23:43.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/api/download_gui_class.py
--rw-rw-rw-   0        0        0    29178 2023-05-03 08:34:10.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/api/downloader.py
-drwxrwxrwx   0        0        0        0 2023-06-23 05:21:45.455564 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/api/upload_model/
--rw-rw-rw-   0        0        0        0 2022-08-17 14:12:32.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/api/upload_model/__init__.py
--rw-rw-rw-   0        0        0      871 2022-08-26 12:20:21.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/api/upload_model/constants.py
--rw-rw-rw-   0        0        0     3036 2022-08-26 12:20:21.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/api/upload_model/download.py
--rw-rw-rw-   0        0        0      420 2022-08-26 12:20:21.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/api/upload_model/login.py
--rw-rw-rw-   0        0        0     3742 2023-04-29 07:27:21.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/api/upload_model/simulate.py
--rw-rw-rw-   0        0        0    44747 2022-08-31 12:10:25.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/api/upload_model/threedi_calls.py
--rw-rw-rw-   0        0        0    10753 2023-01-09 08:31:28.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/api/upload_model/upload.py
-drwxrwxrwx   0        0        0        0 2023-06-23 05:21:45.917571 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/checks/
--rw-rw-rw-   0        0        0        0 2021-12-13 08:25:18.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/checks/__init__.py
--rw-rw-rw-   0        0        0    29924 2023-06-21 12:26:28.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/checks/bank_levels.py
--rw-rw-rw-   0        0        0     5352 2023-05-10 08:00:23.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/checks/grid_result_metadata.py
--rw-rw-rw-   0        0        0     5587 2021-12-13 08:25:18.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/checks/model_backup.py
--rw-rw-rw-   0        0        0    13300 2023-06-21 09:41:43.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/checks/model_splitter.py
--rw-rw-rw-   0        0        0    22134 2021-12-13 08:25:18.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/checks/model_state.py
--rw-rw-rw-   0        0        0    17897 2023-06-21 08:08:05.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/checks/one_d_two_d.py
-drwxrwxrwx   0        0        0        0 2023-06-23 05:21:46.048573 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/checks/sqlite/
--rw-rw-rw-   0        0        0        0 2021-12-13 08:25:18.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/checks/sqlite/__init__.py
--rw-rw-rw-   0        0        0    32770 2023-05-26 14:59:07.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/checks/sqlite/sqlite_main.py
--rw-rw-rw-   0        0        0     7858 2023-05-26 15:08:20.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/checks/sqlite/structure_control.py
--rw-rw-rw-   0        0        0    14230 2022-08-26 12:20:21.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/checks/zero_d_one_d.py
-drwxrwxrwx   0        0        0        0 2023-06-23 05:21:46.337577 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/climate_scenarios/
--rw-rw-rw-   0        0        0        0 2022-04-12 14:08:35.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/climate_scenarios/__init__.py
--rw-rw-rw-   0        0        0     6560 2023-01-09 08:37:42.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/climate_scenarios/interpolate_rasters.py
--rw-rw-rw-   0        0        0    11827 2023-06-21 08:08:01.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/climate_scenarios/klimaatsommen_prep.py
--rw-rw-rw-   0        0        0    15484 2021-12-13 08:25:18.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/climate_scenarios/maskerkaart.py
--rw-rw-rw-   0        0        0     1851 2023-05-05 14:49:14.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/climate_scenarios/maskerkaart_raster.py
--rw-rw-rw-   0        0        0     2351 2021-12-13 08:25:18.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/climate_scenarios/peilgebieden.py
--rw-rw-rw-   0        0        0     5343 2023-05-03 08:34:10.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/climate_scenarios/ruimtekaart.py
--rw-rw-rw-   0        0        0     3239 2023-01-23 09:53:44.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/climate_scenarios/schadekaart.py
--rw-rw-rw-   0        0        0     9351 2023-06-13 10:35:59.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/climate_scenarios/schadekaart_peilgebieden.py
--rw-rw-rw-   0        0        0     6203 2023-05-10 08:00:23.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/folder_helpers.py
--rw-rw-rw-   0        0        0    26403 2023-05-24 16:21:17.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/folders.py
--rw-rw-rw-   0        0        0     4555 2023-06-21 06:32:41.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/migrate_schematisation.py
-drwxrwxrwx   0        0        0        0 2023-06-23 05:21:46.493580 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/result_rasters/
--rw-rw-rw-   0        0        0        0 2023-06-13 10:35:59.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/result_rasters/__init__.py
--rw-rw-rw-   0        0        0    10108 2023-06-13 10:35:59.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/result_rasters/calculate_raster.py
--rw-rw-rw-   0        0        0     9480 2023-05-05 12:18:08.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/result_rasters/netcdf_to_gridgpkg.py
-drwxrwxrwx   0        0        0        0 2023-06-23 05:21:46.721583 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/resources/
--rw-rw-rw-   0        0        0        0 2021-12-13 08:25:18.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/resources/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-23 05:21:47.012588 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/resources/__pycache__/
--rw-rw-rw-   0        0        0      167 2022-07-14 07:53:38.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/resources/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0      171 2022-07-06 13:22:12.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/resources/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0    10193 2023-05-10 14:39:34.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/resources/model_settings.xlsx
--rw-rw-rw-   0        0        0     9864 2023-05-10 14:39:34.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/resources/model_settings_default.xlsx
--rw-rw-rw-   0        0        0    12764 2023-01-09 08:28:05.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/resources/precipitation_frequency.xlsx
--rw-rw-rw-   0        0        0  2080345 2021-12-13 08:25:18.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/resources/precipitation_zones_hhnk.tif
-drwxrwxrwx   0        0        0        0 2023-06-23 05:21:47.130590 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/
--rw-rw-rw-   0        0        0        0 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-23 05:21:47.398594 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/__pycache__/
--rw-rw-rw-   0        0        0      163 2022-07-14 07:53:38.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0      167 2022-07-06 13:21:07.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0    14142 2022-07-14 07:53:38.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/__pycache__/queries.cpython-37.pyc
--rw-rw-rw-   0        0        0    15694 2022-07-06 13:21:07.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/__pycache__/queries.cpython-39.pyc
--rw-rw-rw-   0        0        0    12108 2022-07-14 07:53:38.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/__pycache__/queries_general_checks.cpython-37.pyc
--rw-rw-rw-   0        0        0    12291 2022-07-06 13:22:12.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/__pycache__/queries_general_checks.cpython-39.pyc
-drwxrwxrwx   0        0        0        0 2023-06-23 05:21:47.934602 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/notebooks/
-drwxrwxrwx   0        0        0        0 2023-06-23 05:21:48.009603 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/notebooks/.ipynb_checkpoints/
--rw-rw-rw-   0        0        0     1986 2023-01-23 09:53:44.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/notebooks/.ipynb_checkpoints/01_calculation_gui-checkpoint.ipynb
--rw-rw-rw-   0        0        0     5495 2023-04-11 15:21:12.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/notebooks/.ipynb_checkpoints/02_download_gui-checkpoint.ipynb
--rw-rw-rw-   0        0        0     1877 2023-06-21 06:32:41.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/notebooks/01_calculation_gui.ipynb
--rw-rw-rw-   0        0        0     4791 2023-06-21 11:51:11.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/notebooks/02_download_gui.ipynb
--rw-rw-rw-   0        0        0    22514 2023-06-21 08:03:06.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/notebooks/03_nabewerking_klimaatsommen.ipynb
--rw-rw-rw-   0        0        0     6622 2023-06-21 07:58:12.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/notebooks/04_netcdf_naar_raster.ipynb
--rw-rw-rw-   0        0        0     2090 2023-06-21 07:55:43.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/notebooks/05_sqlite_create_grid.ipynb
--rw-rw-rw-   0        0        0        0 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/notebooks/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-23 05:21:48.172606 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/notebooks/__pycache__/
--rw-rw-rw-   0        0        0      179 2022-01-31 10:15:01.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/notebooks/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0      177 2022-06-29 11:24:40.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/notebooks/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0      847 2023-06-21 10:23:54.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/notebooks/__pycache__/notebook_setup.cpython-39.pyc
--rw-rw-rw-   0        0        0     6121 2023-04-25 11:04:59.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/notebooks/__pycache__/run.cpython-37.pyc
--rw-rw-rw-   0        0        0     6291 2023-06-21 06:54:36.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/notebooks/__pycache__/run.cpython-39.pyc
--rw-rw-rw-   0        0        0      308 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/notebooks/constants.py
--rw-rw-rw-   0        0        0      456 2023-06-21 08:09:29.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/notebooks/notebook_data.json
--rw-rw-rw-   0        0        0      595 2023-06-21 10:23:46.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/notebooks/notebook_setup.py
--rw-rw-rw-   0        0        0     7404 2023-06-21 06:32:41.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/notebooks/run.py
--rw-rw-rw-   0        0        0    20400 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/queries.py
--rw-rw-rw-   0        0        0    25714 2022-03-24 14:59:34.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/queries_general_checks.py
-drwxrwxrwx   0        0        0        0 2023-06-23 05:21:44.717553 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/variables/
--rw-rw-rw-   0        0        0        0 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/variables/__init__.py
--rw-rw-rw-   0        0        0     1858 2023-05-10 08:00:23.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/variables/api_settings.py
--rw-rw-rw-   0        0        0      256 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/variables/backups_table_names.py
--rw-rw-rw-   0        0        0     1043 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/variables/bank_levels.py
--rw-rw-rw-   0        0        0      303 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/variables/damo_hdb_datachecker_variables.py
--rw-rw-rw-   0        0        0     1649 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/variables/database_aliases.py
--rw-rw-rw-   0        0        0     2601 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/variables/database_variables.py
--rw-rw-rw-   0        0        0      134 2023-05-06 10:58:04.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/variables/datachecker_variables.py
--rw-rw-rw-   0        0        0      162 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/variables/default_variables.py
--rw-rw-rw-   0        0        0      130 2023-05-06 07:30:57.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/variables/definitions.py
--rw-rw-rw-   0        0        0      618 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/variables/model_state.py
--rw-rw-rw-   0        0        0      953 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/variables/one_d_two_d.py
--rw-rw-rw-   0        0        0      830 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/variables/sqlite.py
--rw-rw-rw-   0        0        0      254 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/variables/weirs.py
--rw-rw-rw-   0        0        0     1767 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools/variables/zero_d_one_d.py
-drwxrwxrwx   0        0        0        0 2023-06-23 05:21:44.928556 hhnk-threedi-tools-2023.3/hhnk_threedi_tools.egg-info/
--rw-rw-rw-   0        0        0      578 2023-06-23 05:21:44.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5227 2023-06-23 05:21:44.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 05:21:44.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-06-23 05:21:44.000000 hhnk-threedi-tools-2023.3/hhnk_threedi_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-23 05:21:49.182115 hhnk-threedi-tools-2023.3/setup.cfg
--rw-rw-rw-   0        0        0     1659 2023-06-21 07:43:33.000000 hhnk-threedi-tools-2023.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-23 05:21:49.136620 hhnk-threedi-tools-2023.3/tests/
--rw-rw-rw-   0        0        0     4361 2023-06-21 12:30:22.000000 hhnk-threedi-tools-2023.3/tests/test_bank_level_check.py
--rw-rw-rw-   0        0        0     2661 2023-06-14 13:34:27.000000 hhnk-threedi-tools-2023.3/tests/test_folder_structures.py
--rw-rw-rw-   0        0        0     2098 2023-06-21 08:04:34.000000 hhnk-threedi-tools-2023.3/tests/test_klimaatsommen_prep.py
--rw-rw-rw-   0        0        0     1843 2023-06-21 08:04:56.000000 hhnk-threedi-tools-2023.3/tests/test_one_d_two_d.py
--rw-rw-rw-   0        0        0     2095 2023-06-21 08:05:17.000000 hhnk-threedi-tools-2023.3/tests/test_result_rasters.py
--rw-rw-rw-   0        0        0     1147 2023-06-21 08:07:12.000000 hhnk-threedi-tools-2023.3/tests/test_schema_migration.py
--rw-rw-rw-   0        0        0     3288 2023-06-21 08:05:53.000000 hhnk-threedi-tools-2023.3/tests/test_sqlite.py
--rw-rw-rw-   0        0        0      977 2023-06-21 08:06:10.000000 hhnk-threedi-tools-2023.3/tests/test_zero_d_one_d.py
+drwxrwxrwx   0        0        0        0 2023-06-23 11:30:30.716282 hhnk-threedi-tools-2023.3.2/
+-rw-rw-rw-   0        0        0      245 2023-06-19 15:02:38.000000 hhnk-threedi-tools-2023.3.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      580 2023-06-23 11:30:42.471664 hhnk-threedi-tools-2023.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0      584 2023-06-23 11:29:23.000000 hhnk-threedi-tools-2023.3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 11:30:30.766282 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/
+-rw-rw-rw-   0        0        0     1511 2023-06-23 11:29:23.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-23 11:30:31.385292 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/
+-rw-rw-rw-   0        0        0       50 2021-12-13 08:25:18.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-23 11:30:32.236305 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/api/
+-rw-rw-rw-   0        0        0        0 2021-12-13 08:25:18.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/api/__init__.py
+-rw-rw-rw-   0        0        0    33298 2023-06-23 11:29:23.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/api/calculation.py
+-rw-rw-rw-   0        0        0    82235 2023-06-23 11:29:23.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/api/calculation_gui_class.py
+-rw-rw-rw-   0        0        0     2911 2023-05-03 08:34:10.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/api/download_functions.py
+-rw-rw-rw-   0        0        0    57886 2023-06-16 09:23:43.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/api/download_gui_class.py
+-rw-rw-rw-   0        0        0    29178 2023-05-03 08:34:10.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/api/downloader.py
+drwxrwxrwx   0        0        0        0 2023-06-23 11:30:33.293321 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/api/upload_model/
+-rw-rw-rw-   0        0        0        0 2022-08-17 14:12:32.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/api/upload_model/__init__.py
+-rw-rw-rw-   0        0        0      871 2022-08-26 12:20:21.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/api/upload_model/constants.py
+-rw-rw-rw-   0        0        0     3036 2022-08-26 12:20:21.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/api/upload_model/download.py
+-rw-rw-rw-   0        0        0      420 2022-08-26 12:20:21.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/api/upload_model/login.py
+-rw-rw-rw-   0        0        0     3742 2023-04-29 07:27:21.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/api/upload_model/simulate.py
+-rw-rw-rw-   0        0        0    44747 2022-08-31 12:10:25.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/api/upload_model/threedi_calls.py
+-rw-rw-rw-   0        0        0    10753 2023-01-09 08:31:28.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/api/upload_model/upload.py
+drwxrwxrwx   0        0        0        0 2023-06-23 11:30:34.692342 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/checks/
+-rw-rw-rw-   0        0        0        0 2021-12-13 08:25:18.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/checks/__init__.py
+-rw-rw-rw-   0        0        0    29924 2023-06-21 12:26:28.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/checks/bank_levels.py
+-rw-rw-rw-   0        0        0     5352 2023-05-10 08:00:23.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/checks/grid_result_metadata.py
+-rw-rw-rw-   0        0        0     5587 2021-12-13 08:25:18.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/checks/model_backup.py
+-rw-rw-rw-   0        0        0    13300 2023-06-21 09:41:43.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/checks/model_splitter.py
+-rw-rw-rw-   0        0        0    22134 2021-12-13 08:25:18.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/checks/model_state.py
+-rw-rw-rw-   0        0        0    17897 2023-06-21 08:08:05.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/checks/one_d_two_d.py
+drwxrwxrwx   0        0        0        0 2023-06-23 11:30:35.339352 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/checks/sqlite/
+-rw-rw-rw-   0        0        0        0 2021-12-13 08:25:18.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/checks/sqlite/__init__.py
+-rw-rw-rw-   0        0        0    32770 2023-05-26 14:59:07.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/checks/sqlite/sqlite_main.py
+-rw-rw-rw-   0        0        0     7858 2023-05-26 15:08:20.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/checks/sqlite/structure_control.py
+-rw-rw-rw-   0        0        0    14230 2022-08-26 12:20:21.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/checks/zero_d_one_d.py
+drwxrwxrwx   0        0        0        0 2023-06-23 11:30:36.166365 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/climate_scenarios/
+-rw-rw-rw-   0        0        0        0 2022-04-12 14:08:35.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/climate_scenarios/__init__.py
+-rw-rw-rw-   0        0        0     6560 2023-01-09 08:37:42.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/climate_scenarios/interpolate_rasters.py
+-rw-rw-rw-   0        0        0    11827 2023-06-21 08:08:01.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/climate_scenarios/klimaatsommen_prep.py
+-rw-rw-rw-   0        0        0    15484 2021-12-13 08:25:18.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/climate_scenarios/maskerkaart.py
+-rw-rw-rw-   0        0        0     1851 2023-05-05 14:49:14.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/climate_scenarios/maskerkaart_raster.py
+-rw-rw-rw-   0        0        0     2351 2021-12-13 08:25:18.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/climate_scenarios/peilgebieden.py
+-rw-rw-rw-   0        0        0     5343 2023-05-03 08:34:10.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/climate_scenarios/ruimtekaart.py
+-rw-rw-rw-   0        0        0     3239 2023-01-23 09:53:44.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/climate_scenarios/schadekaart.py
+-rw-rw-rw-   0        0        0     9351 2023-06-13 10:35:59.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/climate_scenarios/schadekaart_peilgebieden.py
+-rw-rw-rw-   0        0        0     6289 2023-06-23 11:29:23.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/folder_helpers.py
+-rw-rw-rw-   0        0        0    26403 2023-05-24 16:21:17.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/folders.py
+-rw-rw-rw-   0        0        0     4555 2023-06-21 06:32:41.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/migrate_schematisation.py
+drwxrwxrwx   0        0        0        0 2023-06-23 11:30:36.456369 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/result_rasters/
+-rw-rw-rw-   0        0        0        0 2023-06-13 10:35:59.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/result_rasters/__init__.py
+-rw-rw-rw-   0        0        0    10108 2023-06-13 10:35:59.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/result_rasters/calculate_raster.py
+-rw-rw-rw-   0        0        0     9480 2023-05-05 12:18:08.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/result_rasters/netcdf_to_gridgpkg.py
+drwxrwxrwx   0        0        0        0 2023-06-23 11:30:36.775374 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/resources/
+-rw-rw-rw-   0        0        0        0 2021-12-13 08:25:18.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/resources/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-23 11:30:37.513385 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/resources/__pycache__/
+-rw-rw-rw-   0        0        0      167 2022-07-14 07:53:38.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/resources/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0      171 2022-07-06 13:22:12.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/resources/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0    10193 2023-05-10 14:39:34.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/resources/model_settings.xlsx
+-rw-rw-rw-   0        0        0     9864 2023-05-10 14:39:34.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/resources/model_settings_default.xlsx
+-rw-rw-rw-   0        0        0    12764 2023-01-09 08:28:05.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/resources/precipitation_frequency.xlsx
+-rw-rw-rw-   0        0        0  2080345 2021-12-13 08:25:18.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/resources/precipitation_zones_hhnk.tif
+drwxrwxrwx   0        0        0        0 2023-06-23 11:30:37.766389 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/utils/
+-rw-rw-rw-   0        0        0        0 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-23 11:30:38.280397 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/utils/__pycache__/
+-rw-rw-rw-   0        0        0      163 2022-07-14 07:53:38.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/utils/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0      167 2022-07-06 13:21:07.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/utils/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0    14142 2022-07-14 07:53:38.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/utils/__pycache__/queries.cpython-37.pyc
+-rw-rw-rw-   0        0        0    15694 2022-07-06 13:21:07.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/utils/__pycache__/queries.cpython-39.pyc
+-rw-rw-rw-   0        0        0    12108 2022-07-14 07:53:38.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/utils/__pycache__/queries_general_checks.cpython-37.pyc
+-rw-rw-rw-   0        0        0    12291 2022-07-06 13:22:12.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/utils/__pycache__/queries_general_checks.cpython-39.pyc
+drwxrwxrwx   0        0        0        0 2023-06-23 11:30:39.385414 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/utils/notebooks/
+drwxrwxrwx   0        0        0        0 2023-06-23 11:30:39.565417 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/utils/notebooks/.ipynb_checkpoints/
+-rw-rw-rw-   0        0        0     1986 2023-01-23 09:53:44.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/utils/notebooks/.ipynb_checkpoints/01_calculation_gui-checkpoint.ipynb
+-rw-rw-rw-   0        0        0     5495 2023-04-11 15:21:12.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/utils/notebooks/.ipynb_checkpoints/02_download_gui-checkpoint.ipynb
+-rw-rw-rw-   0        0        0     1877 2023-06-21 06:32:41.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/utils/notebooks/01_calculation_gui.ipynb
+-rw-rw-rw-   0        0        0     6095 2023-06-23 11:29:23.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/utils/notebooks/02_download_gui.ipynb
+-rw-rw-rw-   0        0        0    23127 2023-06-23 11:29:23.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/utils/notebooks/03_nabewerking_klimaatsommen.ipynb
+-rw-rw-rw-   0        0        0     6622 2023-06-21 07:58:12.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/utils/notebooks/04_netcdf_naar_raster.ipynb
+-rw-rw-rw-   0        0        0     2090 2023-06-21 07:55:43.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/utils/notebooks/05_sqlite_create_grid.ipynb
+-rw-rw-rw-   0        0        0        0 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/utils/notebooks/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-23 11:30:39.858421 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/utils/notebooks/__pycache__/
+-rw-rw-rw-   0        0        0      179 2022-01-31 10:15:01.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/utils/notebooks/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0      177 2022-06-29 11:24:40.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/utils/notebooks/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0      847 2023-06-21 10:23:54.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/utils/notebooks/__pycache__/notebook_setup.cpython-39.pyc
+-rw-rw-rw-   0        0        0     6121 2023-04-25 11:04:59.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/utils/notebooks/__pycache__/run.cpython-37.pyc
+-rw-rw-rw-   0        0        0     6291 2023-06-21 06:54:36.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/utils/notebooks/__pycache__/run.cpython-39.pyc
+-rw-rw-rw-   0        0        0      308 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/utils/notebooks/constants.py
+-rw-rw-rw-   0        0        0      456 2023-06-21 08:09:29.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/utils/notebooks/notebook_data.json
+-rw-rw-rw-   0        0        0      595 2023-06-21 10:23:46.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/utils/notebooks/notebook_setup.py
+-rw-rw-rw-   0        0        0     7404 2023-06-21 06:32:41.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/utils/notebooks/run.py
+-rw-rw-rw-   0        0        0    20400 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/utils/queries.py
+-rw-rw-rw-   0        0        0    25714 2022-03-24 14:59:34.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/utils/queries_general_checks.py
+drwxrwxrwx   0        0        0        0 2023-06-23 11:30:41.669449 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/variables/
+-rw-rw-rw-   0        0        0        0 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/variables/__init__.py
+-rw-rw-rw-   0        0        0     1858 2023-05-10 08:00:23.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/variables/api_settings.py
+-rw-rw-rw-   0        0        0      256 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/variables/backups_table_names.py
+-rw-rw-rw-   0        0        0     1043 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/variables/bank_levels.py
+-rw-rw-rw-   0        0        0      303 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/variables/damo_hdb_datachecker_variables.py
+-rw-rw-rw-   0        0        0     1649 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/variables/database_aliases.py
+-rw-rw-rw-   0        0        0     2601 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/variables/database_variables.py
+-rw-rw-rw-   0        0        0      134 2023-05-06 10:58:04.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/variables/datachecker_variables.py
+-rw-rw-rw-   0        0        0      162 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/variables/default_variables.py
+-rw-rw-rw-   0        0        0      130 2023-05-06 07:30:57.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/variables/definitions.py
+-rw-rw-rw-   0        0        0      618 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/variables/model_state.py
+-rw-rw-rw-   0        0        0      953 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/variables/one_d_two_d.py
+-rw-rw-rw-   0        0        0      830 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/variables/sqlite.py
+-rw-rw-rw-   0        0        0      254 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/variables/weirs.py
+-rw-rw-rw-   0        0        0     1767 2021-12-13 08:25:22.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/variables/zero_d_one_d.py
+drwxrwxrwx   0        0        0        0 2023-06-23 11:30:31.001286 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools.egg-info/
+-rw-rw-rw-   0        0        0      580 2023-06-23 11:30:28.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5227 2023-06-23 11:30:29.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 11:30:28.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-06-23 11:30:28.000000 hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-23 11:30:42.530080 hhnk-threedi-tools-2023.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     1659 2023-06-21 07:43:33.000000 hhnk-threedi-tools-2023.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 11:30:42.401460 hhnk-threedi-tools-2023.3.2/tests/
+-rw-rw-rw-   0        0        0     4361 2023-06-21 12:30:22.000000 hhnk-threedi-tools-2023.3.2/tests/test_bank_level_check.py
+-rw-rw-rw-   0        0        0     2661 2023-06-14 13:34:27.000000 hhnk-threedi-tools-2023.3.2/tests/test_folder_structures.py
+-rw-rw-rw-   0        0        0     2111 2023-06-23 11:29:24.000000 hhnk-threedi-tools-2023.3.2/tests/test_klimaatsommen_prep.py
+-rw-rw-rw-   0        0        0     1843 2023-06-21 08:04:56.000000 hhnk-threedi-tools-2023.3.2/tests/test_one_d_two_d.py
+-rw-rw-rw-   0        0        0     2095 2023-06-21 08:05:17.000000 hhnk-threedi-tools-2023.3.2/tests/test_result_rasters.py
+-rw-rw-rw-   0        0        0     1147 2023-06-21 08:07:12.000000 hhnk-threedi-tools-2023.3.2/tests/test_schema_migration.py
+-rw-rw-rw-   0        0        0     3288 2023-06-21 08:05:53.000000 hhnk-threedi-tools-2023.3.2/tests/test_sqlite.py
+-rw-rw-rw-   0        0        0      977 2023-06-21 08:06:10.000000 hhnk-threedi-tools-2023.3.2/tests/test_zero_d_one_d.py
```

### Comparing `hhnk-threedi-tools-2023.3/PKG-INFO` & `hhnk-threedi-tools-2023.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hhnk-threedi-tools
-Version: 2023.3
+Version: 2023.3.2
 Summary: HHNK watersystemen analysis tools
 Home-page: https://github.com/threedi/hhnk-threedi-tools
 Author: Wietse van Gerwen, Laure Ravier
 Author-email: w.vangerwen@hhnk.nl
 Maintainer: Wietse van Gerwen
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/threedi/hhnk-threedi-tools/issues
```

### Comparing `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/__init__.py` & `hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,8 +35,8 @@
 from hhnk_threedi_tools.core.checks.model_backup import (
     create_backups,
     select_values_to_update_from_backup,
     update_bank_levels_last_calc,
 )
 
 
-__version__ = '2023.3'
+__version__ = '2023.3.2'
```

### Comparing `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/api/calculation.py` & `hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/api/calculation.py`

 * *Files 1% similar despite different names*

```diff
@@ -234,15 +234,23 @@
             for index, row in hrt.sqlite_table_to_df(
                 database_path=self.sqlite_path, table_name="v2_control_table"
             ).iterrows():
                 action_table_string = row["action_table"]
                 action_table = []
                 action_type = row["action_type"]
                 for entry in action_table_string.split("#"):
-                    measurement = [float(entry.split(";")[0])]
+                    try:
+                        measurement = [float(entry.split(";")[0])]
+                    except ValueError as e:
+                        #Problem with action table 
+                        print(f"""Problem with '{entry}' at index {action_table_string.index(entry)} of the action_table_string for
+{row}
+""")
+                        raise e
+
                     if action_type in ["set_crest_level", "set_pump_capacity"]:
                         action = [float(entry.split(";")[1])]
                     elif action_type == "set_discharge_coefficients":
                         action = [
                             float(entry.split(";")[1].split(" ")[0]),
                             float(entry.split(";")[1].split(" ")[0]),
                         ]
```

### Comparing `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/api/calculation_gui_class.py` & `hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/api/calculation_gui_class.py`

 * *Files 0% similar despite different names*

```diff
@@ -1063,15 +1063,15 @@
 
         output_folder = self.output.subfolder_batch_value.value
         if output_folder == "":
             ready_to_roll=False
             self.add_feedback("ERROR", "No output subfolder selected.")
             
         else:
-            self.output.folder_value_batch.value = self.vars.folder.threedi_results.batch.full_path(output_folder)
+            self.output.folder_value_batch.value = str(self.vars.folder.threedi_results.batch.full_path(output_folder))
             if os.path.exists(self.vars.folder.threedi_results.batch.full_path(output_folder)):
                 self.add_feedback("Warning", "Output folder map already exists!")
 
         # output_folder = self.start.simulation_batch_name_widget.value.replace("{rt}_{gxg}_{rs}","")
         # output_folder = output_folder.replace("({i})","")
         # output_folder = output_folder.replace("  "," ")
         # output_folder=output_folder.format(schema_name=self.model.schema_name_widget.value,
```

### Comparing `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/api/download_functions.py` & `hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/api/download_functions.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/api/download_gui_class.py` & `hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/api/download_gui_class.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/api/downloader.py` & `hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/api/downloader.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/api/upload_model/constants.py` & `hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/api/upload_model/constants.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/api/upload_model/download.py` & `hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/api/upload_model/download.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/api/upload_model/simulate.py` & `hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/api/upload_model/simulate.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/api/upload_model/threedi_calls.py` & `hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/api/upload_model/threedi_calls.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/api/upload_model/upload.py` & `hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/api/upload_model/upload.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/checks/bank_levels.py` & `hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/checks/bank_levels.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/checks/grid_result_metadata.py` & `hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/checks/grid_result_metadata.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/checks/model_backup.py` & `hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/checks/model_backup.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/checks/model_splitter.py` & `hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/checks/model_splitter.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/checks/model_state.py` & `hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/checks/model_state.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/checks/one_d_two_d.py` & `hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/checks/one_d_two_d.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/checks/sqlite/sqlite_main.py` & `hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/checks/sqlite/sqlite_main.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/checks/sqlite/structure_control.py` & `hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/checks/sqlite/structure_control.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/checks/zero_d_one_d.py` & `hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/checks/zero_d_one_d.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/climate_scenarios/interpolate_rasters.py` & `hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/climate_scenarios/interpolate_rasters.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/climate_scenarios/klimaatsommen_prep.py` & `hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/climate_scenarios/klimaatsommen_prep.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/climate_scenarios/maskerkaart.py` & `hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/climate_scenarios/maskerkaart.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/climate_scenarios/maskerkaart_raster.py` & `hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/climate_scenarios/maskerkaart_raster.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/climate_scenarios/peilgebieden.py` & `hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/climate_scenarios/peilgebieden.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/climate_scenarios/ruimtekaart.py` & `hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/climate_scenarios/ruimtekaart.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/climate_scenarios/schadekaart.py` & `hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/climate_scenarios/schadekaart.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/climate_scenarios/schadekaart_peilgebieden.py` & `hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/climate_scenarios/schadekaart_peilgebieden.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/folder_helpers.py` & `hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/folder_helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,36 +11,36 @@
 
 class ClimateResult(hrt.Folder):
     """Individual batch result with download and output folder"""
 
     def __init__(self, base, create=False):
         super().__init__(base, create=create)
 
-        self.downloads = self.ClimateResultDownloads(self.base)
-        self.output = self.ClimateResultOutput(self.base)
+        self.downloads = self.ClimateResultDownloads(self.base, create=create)
+        self.output = self.ClimateResultOutput(self.base, create=create)
 
 
     @property
     def structure(self):
         return f"""  
             {self.space}{self.name}
             {self.space}├── downloads
             {self.space}└── output
                 """
 
 
     class ClimateResultDownloads(hrt.Folder):
-        def __init__(self, base):
-            super().__init__(os.path.join(base, "01_downloads"), create=False)
+        def __init__(self, base, create=False):
+            super().__init__(os.path.join(base, "01_downloads"), create=create)
 
             # Files
             self.names = []  # Initializes names.setter
 
             for name in self.names:
-                setattr(self, name, self.ClimateResultScenario(self.base, name))
+                setattr(self, name, self.ClimateResultScenario(self.base, name, create=create))
 
 
         @property
         def names(self):
             return self._names
 
 
@@ -83,19 +83,19 @@
                 return f"""{self.name} @ {self.path}
                             Folders:\t{self.structure_extra}
                             Files:\t{list(self.files.keys())}
                             Layers:\t{list(self.olayers.keys())}
                         """
 
     class ClimateResultOutput(hrt.Folder):
-        def __init__(self, base):
-            super().__init__(os.path.join(base, "02_output_rasters"), create=False)
+        def __init__(self, base, create):
+            super().__init__(os.path.join(base, "02_output_rasters"), create=create)
 
             # Folders
-            self.temp = self.ClimateResultOutputTemp(self.base)
+            self.temp = self.ClimateResultOutputTemp(self.base, create)
 
             # Files
             self.add_file("maskerkaart", "maskerkaart.shp")
             self.add_file("maskerkaart_diepte_tif", "maskerkaart_diepte.tif", "raster")
             self.add_file("maskerkaart_schade_tif", "maskerkaart_schade.tif", "raster")
             self.add_file("geen_schade_tif", "geen_schade.tif", "raster")
             self.add_file("mask_diepte_plas", "mask_diepte_plas.tif", "raster")
@@ -145,15 +145,15 @@
             return f"""  
                 {self.space}{self.name}
                 {self.space}├── temp
                     """
 
 
         class ClimateResultOutputTemp(hrt.Folder):
-            def __init__(self, base):
-                super().__init__(os.path.join(base, "temp"), create=False)
+            def __init__(self, base, create):
+                super().__init__(os.path.join(base, "temp"), create=create)
 
                 self.add_file("peilgebieden_diepte", "peilgebieden_diepte.tif", "raster")
                 self.add_file("peilgebieden_schade", "peilgebieden_schade.tif", "raster")
                 self.add_file("peilgebieden", "peilgebieden_clipped.shp")
```

### Comparing `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/folders.py` & `hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/folders.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/migrate_schematisation.py` & `hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/migrate_schematisation.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/result_rasters/calculate_raster.py` & `hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/result_rasters/calculate_raster.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/core/result_rasters/netcdf_to_gridgpkg.py` & `hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/core/result_rasters/netcdf_to_gridgpkg.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/resources/model_settings.xlsx` & `hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/resources/model_settings.xlsx`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/resources/model_settings_default.xlsx` & `hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/resources/model_settings_default.xlsx`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/resources/precipitation_frequency.xlsx` & `hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/resources/precipitation_frequency.xlsx`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/resources/precipitation_zones_hhnk.tif` & `hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/resources/precipitation_zones_hhnk.tif`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/__pycache__/queries.cpython-37.pyc` & `hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/utils/__pycache__/queries.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/__pycache__/queries.cpython-39.pyc` & `hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/utils/__pycache__/queries.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/__pycache__/queries_general_checks.cpython-37.pyc` & `hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/utils/__pycache__/queries_general_checks.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/__pycache__/queries_general_checks.cpython-39.pyc` & `hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/utils/__pycache__/queries_general_checks.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/notebooks/.ipynb_checkpoints/01_calculation_gui-checkpoint.ipynb` & `hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/utils/notebooks/.ipynb_checkpoints/01_calculation_gui-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/notebooks/.ipynb_checkpoints/02_download_gui-checkpoint.ipynb` & `hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/utils/notebooks/.ipynb_checkpoints/02_download_gui-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/notebooks/01_calculation_gui.ipynb` & `hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/utils/notebooks/01_calculation_gui.ipynb`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/notebooks/03_nabewerking_klimaatsommen.ipynb` & `hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/utils/notebooks/03_nabewerking_klimaatsommen.ipynb`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997933884297521%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(2, "Zorg dat in de poldermap onder 01. DAMO en HDB een '*

 * *            'folder staat met de naam \'peilgebieden\'.\\n"), (3, "In deze folder moet de shape '*

 * *            "van de peilgebieden. Deze shape moet 'peilgebieden_{Polderclusternaam}.shp' "*

 * *            'heten,\\n")], delete: [5, 4, 2, 1]}}}'}*

```diff
@@ -4,18 +4,16 @@
             "attachments": {},
             "cell_type": "markdown",
             "id": "c1107963",
             "metadata": {},
             "source": [
                 "# Nabewerking Klimaatsommen\n",
                 "\n",
-                "### Draai eerst 03_nabewerking_klimaatsommen_prep.ipynb\n",
-                "\n",
-                "Zorg dat in de poldermap onder 01. DAMO en HDB een mapje staat met de naam 'peilgebieden'.\n",
-                "In dit mapje mapje moet de shape van de peilgebieden. Deze shape moet 'peilgebieden_Polderclusternaam.shp' heten,\n",
+                "Zorg dat in de poldermap onder 01. DAMO en HDB een folder staat met de naam 'peilgebieden'.\n",
+                "In deze folder moet de shape van de peilgebieden. Deze shape moet 'peilgebieden_{Polderclusternaam}.shp' heten,\n",
                 "dus bijvoorbeeld 'peilgebieden_Eijerland.shp'. In de kolom 'name' moet de naam van de polder staan.\n",
                 "Dit laatste is van belang wanneer meerdere polders in \u00e9\u00e9n poldercluster gezamelijk zijn doorgerekend.\n",
                 "Maak een kopie van je datachecker output: fixeddrainagelevelarea. Dat werkt.\n"
             ]
         },
         {
             "cell_type": "code",
```

### Comparing `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/notebooks/04_netcdf_naar_raster.ipynb` & `hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/utils/notebooks/04_netcdf_naar_raster.ipynb`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/notebooks/05_sqlite_create_grid.ipynb` & `hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/utils/notebooks/05_sqlite_create_grid.ipynb`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/notebooks/__pycache__/notebook_setup.cpython-39.pyc` & `hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/utils/notebooks/__pycache__/notebook_setup.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/notebooks/__pycache__/run.cpython-37.pyc` & `hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/utils/notebooks/__pycache__/run.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/notebooks/__pycache__/run.cpython-39.pyc` & `hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/utils/notebooks/__pycache__/run.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/notebooks/notebook_setup.py` & `hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/utils/notebooks/notebook_setup.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/notebooks/run.py` & `hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/utils/notebooks/run.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/queries.py` & `hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/utils/queries.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/utils/queries_general_checks.py` & `hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/utils/queries_general_checks.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/variables/api_settings.py` & `hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/variables/api_settings.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/variables/bank_levels.py` & `hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/variables/bank_levels.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/variables/database_aliases.py` & `hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/variables/database_aliases.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/variables/database_variables.py` & `hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/variables/database_variables.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/variables/model_state.py` & `hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/variables/model_state.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/variables/one_d_two_d.py` & `hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/variables/one_d_two_d.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/variables/sqlite.py` & `hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/variables/sqlite.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/hhnk_threedi_tools/variables/zero_d_one_d.py` & `hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools/variables/zero_d_one_d.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/hhnk_threedi_tools.egg-info/PKG-INFO` & `hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hhnk-threedi-tools
-Version: 2023.3
+Version: 2023.3.2
 Summary: HHNK watersystemen analysis tools
 Home-page: https://github.com/threedi/hhnk-threedi-tools
 Author: Wietse van Gerwen, Laure Ravier
 Author-email: w.vangerwen@hhnk.nl
 Maintainer: Wietse van Gerwen
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/threedi/hhnk-threedi-tools/issues
```

### Comparing `hhnk-threedi-tools-2023.3/hhnk_threedi_tools.egg-info/SOURCES.txt` & `hhnk-threedi-tools-2023.3.2/hhnk_threedi_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/setup.py` & `hhnk-threedi-tools-2023.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/tests/test_bank_level_check.py` & `hhnk-threedi-tools-2023.3.2/tests/test_bank_level_check.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/tests/test_folder_structures.py` & `hhnk-threedi-tools-2023.3.2/tests/test_folder_structures.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/tests/test_klimaatsommen_prep.py` & `hhnk-threedi-tools-2023.3.2/tests/test_klimaatsommen_prep.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         cfg_file = 'cfg_lizard.cfg',
         landuse_file = FOLDER_TEST.model.schema_base.rasters.landuse,
         verify=False
     )
     
     #Rebase the batch_fd so it will always create all output.
     batch_test = TEMP_DIR/f"batch_test_{hrt.get_uuid()}"
-    batch_test = ClimateResult(batch_test)
+    batch_test = ClimateResult(batch_test, create=True)
     shutil.copytree(src=klimaatsommenprep.batch_fd.downloads.piek_glg_T10.netcdf.pl,
                     dst=batch_test.downloads.piek_glg_T10.netcdf.pl)
     klimaatsommenprep.batch_fd = batch_test
     
     #Run test
     klimaatsommenprep.run(overwrite=True, testing=True)
```

### Comparing `hhnk-threedi-tools-2023.3/tests/test_one_d_two_d.py` & `hhnk-threedi-tools-2023.3.2/tests/test_one_d_two_d.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/tests/test_result_rasters.py` & `hhnk-threedi-tools-2023.3.2/tests/test_result_rasters.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/tests/test_schema_migration.py` & `hhnk-threedi-tools-2023.3.2/tests/test_schema_migration.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/tests/test_sqlite.py` & `hhnk-threedi-tools-2023.3.2/tests/test_sqlite.py`

 * *Files identical despite different names*

### Comparing `hhnk-threedi-tools-2023.3/tests/test_zero_d_one_d.py` & `hhnk-threedi-tools-2023.3.2/tests/test_zero_d_one_d.py`

 * *Files identical despite different names*

