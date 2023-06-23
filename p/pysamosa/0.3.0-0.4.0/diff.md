# Comparing `tmp/pysamosa-0.3.0.tar.gz` & `tmp/pysamosa-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysamosa-0.3.0.tar", last modified: Fri Jun 16 04:58:39 2023, max compression
+gzip compressed data, was "pysamosa-0.4.0.tar", last modified: Fri Jun 23 09:14:43 2023, max compression
```

## Comparing `pysamosa-0.3.0.tar` & `pysamosa-0.4.0.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-16 04:58:39.907448 pysamosa-0.3.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1829 2023-06-16 04:51:17.000000 pysamosa-0.3.0/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      306 2023-06-16 04:51:17.000000 pysamosa-0.3.0/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)    14290 2023-06-16 04:58:39.907448 pysamosa-0.3.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)    13113 2023-06-16 04:51:17.000000 pysamosa-0.3.0/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-16 04:58:39.843444 pysamosa-0.3.0/notebooks/
--rw-rw-r--   0 travis    (2000) travis    (2000)  1309734 2023-06-16 04:51:17.000000 pysamosa-0.3.0/notebooks/retracking_example.ipynb
--rw-rw-r--   0 travis    (2000) travis    (2000)      132 2023-06-16 04:51:17.000000 pysamosa-0.3.0/pyproject.toml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-16 04:58:39.863445 pysamosa-0.3.0/pysamosa/
--rw-rw-r--   0 travis    (2000) travis    (2000)      184 2023-06-16 04:51:17.000000 pysamosa-0.3.0/pysamosa/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12843 2023-06-16 04:51:17.000000 pysamosa-0.3.0/pysamosa/common_types.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      334 2023-06-16 04:51:17.000000 pysamosa-0.3.0/pysamosa/conf_params.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    26159 2023-06-16 04:51:17.000000 pysamosa-0.3.0/pysamosa/data_access.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3162 2023-06-16 04:51:17.000000 pysamosa-0.3.0/pysamosa/dist2coast.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      462 2023-06-16 04:51:17.000000 pysamosa-0.3.0/pysamosa/download_aux_data.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5229 2023-06-16 04:51:17.000000 pysamosa-0.3.0/pysamosa/l1b_simulator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3086 2023-06-16 04:51:17.000000 pysamosa-0.3.0/pysamosa/leading_edge_detector.py
--rw-rw-r--   0 travis    (2000) travis    (2000)  9928947 2023-06-16 04:51:17.000000 pysamosa-0.3.0/pysamosa/luts_samosa.pickle
--rw-rw-r--   0 travis    (2000) travis    (2000)     6053 2023-06-16 04:51:17.000000 pysamosa-0.3.0/pysamosa/main_coastalffsar.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6164 2023-06-16 04:51:17.000000 pysamosa-0.3.0/pysamosa/main_coral_paper.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1862 2023-06-16 04:51:17.000000 pysamosa-0.3.0/pysamosa/main_cs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1532 2023-06-16 04:51:17.000000 pysamosa-0.3.0/pysamosa/main_s3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1737 2023-06-16 04:51:17.000000 pysamosa-0.3.0/pysamosa/main_s6.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2731 2023-06-16 04:51:17.000000 pysamosa-0.3.0/pysamosa/main_s6jtex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2987 2023-06-16 04:51:17.000000 pysamosa-0.3.0/pysamosa/main_s6jtex_raw_vs_rmc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17889 2023-06-16 04:51:17.000000 pysamosa-0.3.0/pysamosa/model.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1614 2023-06-16 04:51:17.000000 pysamosa-0.3.0/pysamosa/model_helpers.pyx
--rw-rw-r--   0 travis    (2000) travis    (2000)     7209 2023-06-16 04:51:17.000000 pysamosa-0.3.0/pysamosa/montecarlo_simulator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       19 2023-06-16 04:51:17.000000 pysamosa-0.3.0/pysamosa/pysamosa.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1622 2023-06-16 04:51:17.000000 pysamosa-0.3.0/pysamosa/qual_flag_estimator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24082 2023-06-16 04:51:17.000000 pysamosa-0.3.0/pysamosa/retracker.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12275 2023-06-16 04:51:17.000000 pysamosa-0.3.0/pysamosa/retracker_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23266 2023-06-16 04:51:17.000000 pysamosa-0.3.0/pysamosa/retracker_processor.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6887 2023-06-16 04:51:17.000000 pysamosa-0.3.0/pysamosa/rip.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      232 2023-06-16 04:51:17.000000 pysamosa-0.3.0/pysamosa/settings.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3527 2023-06-16 04:51:17.000000 pysamosa-0.3.0/pysamosa/settings_manager.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1684 2023-06-16 04:51:17.000000 pysamosa-0.3.0/pysamosa/simple_logger.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9195 2023-06-16 04:51:17.000000 pysamosa-0.3.0/pysamosa/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       47 2023-06-16 04:51:17.000000 pysamosa-0.3.0/pysamosa/version.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-16 04:58:39.867446 pysamosa-0.3.0/pysamosa.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)    14290 2023-06-16 04:58:39.000000 pysamosa-0.3.0/pysamosa.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1855 2023-06-16 04:58:39.000000 pysamosa-0.3.0/pysamosa.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-16 04:58:39.000000 pysamosa-0.3.0/pysamosa.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-16 04:58:39.000000 pysamosa-0.3.0/pysamosa.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)      165 2023-06-16 04:58:39.000000 pysamosa-0.3.0/pysamosa.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        9 2023-06-16 04:58:39.000000 pysamosa-0.3.0/pysamosa.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      308 2023-06-16 04:51:17.000000 pysamosa-0.3.0/requirements.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-16 04:58:39.867446 pysamosa-0.3.0/scripts/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1671 2023-06-16 04:51:17.000000 pysamosa-0.3.0/scripts/cs_l2_conversion.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-16 04:58:39.895448 pysamosa-0.3.0/scripts/luts/
--rw-rw-r--   0 travis    (2000) travis    (2000)   217134 2023-06-16 04:51:17.000000 pysamosa-0.3.0/scripts/luts/AUX_RLUT_S6A_002.nc
--rw-rw-r--   0 travis    (2000) travis    (2000)   214215 2023-06-16 04:51:17.000000 pysamosa-0.3.0/scripts/luts/AUX_RLUT_S6A_003.nc
--rwxrwxr-x   0 travis    (2000) travis    (2000)  4818008 2023-06-16 04:51:17.000000 pysamosa-0.3.0/scripts/luts/F0.txt
--rwxrwxr-x   0 travis    (2000) travis    (2000)  4827430 2023-06-16 04:51:17.000000 pysamosa-0.3.0/scripts/luts/F1.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    30520 2023-06-16 04:51:17.000000 pysamosa-0.3.0/scripts/luts/LUT_Alpha_P_CS-2.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)   993604 2023-06-16 04:51:17.000000 pysamosa-0.3.0/scripts/luts/S6A_TEST_AUX_FLUT___00000000T000000_99999999T999999_0001.NC
--rw-rw-r--   0 travis    (2000) travis    (2000)    30520 2023-06-16 04:51:17.000000 pysamosa-0.3.0/scripts/luts/alphap_table_SEN3_09_Nov_2017.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     3215 2023-06-16 04:51:17.000000 pysamosa-0.3.0/scripts/luts/convert_luts.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9610 2023-06-16 04:51:17.000000 pysamosa-0.3.0/scripts/thesis_plots.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6110 2023-06-16 04:51:17.000000 pysamosa-0.3.0/scripts/track_browser.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9809 2023-06-16 04:51:17.000000 pysamosa-0.3.0/scripts/track_browser_footprint.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      436 2023-06-16 04:58:39.911449 pysamosa-0.3.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     2361 2023-06-16 04:51:17.000000 pysamosa-0.3.0/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-16 04:58:39.903448 pysamosa-0.3.0/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2023-06-16 04:51:17.000000 pysamosa-0.3.0/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10885 2023-06-16 04:51:17.000000 pysamosa-0.3.0/tests/helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2431 2023-06-16 04:51:17.000000 pysamosa-0.3.0/tests/settings_dumper.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2429 2023-06-16 04:51:17.000000 pysamosa-0.3.0/tests/test_common_types.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3305 2023-06-16 04:51:17.000000 pysamosa-0.3.0/tests/test_dist2coast.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5903 2023-06-16 04:51:17.000000 pysamosa-0.3.0/tests/test_dynamic_fg_epoch.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4328 2023-06-16 04:51:17.000000 pysamosa-0.3.0/tests/test_l1b_sim_retracker.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2093 2023-06-16 04:51:17.000000 pysamosa-0.3.0/tests/test_l1b_simulator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1253 2023-06-16 04:51:17.000000 pysamosa-0.3.0/tests/test_leading_edge_detector.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9363 2023-06-16 04:51:17.000000 pysamosa-0.3.0/tests/test_model.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9434 2023-06-16 04:51:17.000000 pysamosa-0.3.0/tests/test_montecarlo_sim.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8236 2023-06-16 04:51:17.000000 pysamosa-0.3.0/tests/test_retrack_multi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9035 2023-06-16 04:51:17.000000 pysamosa-0.3.0/tests/test_retrack_single.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4791 2023-06-16 04:51:17.000000 pysamosa-0.3.0/tests/test_samplusplus.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1111 2023-06-16 04:51:17.000000 pysamosa-0.3.0/tests/test_utils.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-23 09:14:43.218287 pysamosa-0.4.0/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7651 2023-06-23 09:07:23.000000 pysamosa-0.4.0/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)      306 2023-06-23 09:07:23.000000 pysamosa-0.4.0/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13974 2023-06-23 09:14:43.218287 pysamosa-0.4.0/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12753 2023-06-23 09:07:23.000000 pysamosa-0.4.0/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-23 09:14:43.174284 pysamosa-0.4.0/notebooks/
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1309734 2023-06-23 09:07:23.000000 pysamosa-0.4.0/notebooks/retracking_example.ipynb
+-rw-rw-r--   0 travis    (2000) travis    (2000)      132 2023-06-23 09:07:23.000000 pysamosa-0.4.0/pyproject.toml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-23 09:14:43.198285 pysamosa-0.4.0/pysamosa/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      184 2023-06-23 09:07:23.000000 pysamosa-0.4.0/pysamosa/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12843 2023-06-23 09:07:23.000000 pysamosa-0.4.0/pysamosa/common_types.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      334 2023-06-23 09:07:23.000000 pysamosa-0.4.0/pysamosa/conf_params.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    26159 2023-06-23 09:07:23.000000 pysamosa-0.4.0/pysamosa/data_access.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3162 2023-06-23 09:07:23.000000 pysamosa-0.4.0/pysamosa/dist2coast.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      462 2023-06-23 09:07:23.000000 pysamosa-0.4.0/pysamosa/download_aux_data.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5229 2023-06-23 09:07:23.000000 pysamosa-0.4.0/pysamosa/l1b_simulator.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3086 2023-06-23 09:07:23.000000 pysamosa-0.4.0/pysamosa/leading_edge_detector.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)  9928947 2023-06-23 09:07:23.000000 pysamosa-0.4.0/pysamosa/luts_samosa.pickle
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6053 2023-06-23 09:07:23.000000 pysamosa-0.4.0/pysamosa/main_coastalffsar.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6164 2023-06-23 09:07:23.000000 pysamosa-0.4.0/pysamosa/main_coral_paper.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1862 2023-06-23 09:07:23.000000 pysamosa-0.4.0/pysamosa/main_cs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1532 2023-06-23 09:07:23.000000 pysamosa-0.4.0/pysamosa/main_s3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1737 2023-06-23 09:07:23.000000 pysamosa-0.4.0/pysamosa/main_s6.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2731 2023-06-23 09:07:23.000000 pysamosa-0.4.0/pysamosa/main_s6jtex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2987 2023-06-23 09:07:23.000000 pysamosa-0.4.0/pysamosa/main_s6jtex_raw_vs_rmc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17889 2023-06-23 09:07:23.000000 pysamosa-0.4.0/pysamosa/model.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1614 2023-06-23 09:07:23.000000 pysamosa-0.4.0/pysamosa/model_helpers.pyx
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7209 2023-06-23 09:07:23.000000 pysamosa-0.4.0/pysamosa/montecarlo_simulator.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       19 2023-06-23 09:07:23.000000 pysamosa-0.4.0/pysamosa/pysamosa.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1622 2023-06-23 09:07:23.000000 pysamosa-0.4.0/pysamosa/qual_flag_estimator.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24082 2023-06-23 09:07:23.000000 pysamosa-0.4.0/pysamosa/retracker.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12275 2023-06-23 09:07:23.000000 pysamosa-0.4.0/pysamosa/retracker_helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23266 2023-06-23 09:07:23.000000 pysamosa-0.4.0/pysamosa/retracker_processor.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6887 2023-06-23 09:07:23.000000 pysamosa-0.4.0/pysamosa/rip.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      232 2023-06-23 09:07:23.000000 pysamosa-0.4.0/pysamosa/settings.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3527 2023-06-23 09:07:23.000000 pysamosa-0.4.0/pysamosa/settings_manager.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1684 2023-06-23 09:07:23.000000 pysamosa-0.4.0/pysamosa/simple_logger.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9195 2023-06-23 09:07:23.000000 pysamosa-0.4.0/pysamosa/utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       47 2023-06-23 09:07:23.000000 pysamosa-0.4.0/pysamosa/version.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-23 09:14:43.198285 pysamosa-0.4.0/pysamosa.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13974 2023-06-23 09:14:43.000000 pysamosa-0.4.0/pysamosa.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1855 2023-06-23 09:14:43.000000 pysamosa-0.4.0/pysamosa.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-23 09:14:43.000000 pysamosa-0.4.0/pysamosa.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-23 09:14:43.000000 pysamosa-0.4.0/pysamosa.egg-info/not-zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)      165 2023-06-23 09:14:43.000000 pysamosa-0.4.0/pysamosa.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        9 2023-06-23 09:14:43.000000 pysamosa-0.4.0/pysamosa.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      308 2023-06-23 09:07:23.000000 pysamosa-0.4.0/requirements.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-23 09:14:43.198285 pysamosa-0.4.0/scripts/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1671 2023-06-23 09:07:23.000000 pysamosa-0.4.0/scripts/cs_l2_conversion.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-23 09:14:43.214287 pysamosa-0.4.0/scripts/luts/
+-rw-rw-r--   0 travis    (2000) travis    (2000)   217134 2023-06-23 09:07:23.000000 pysamosa-0.4.0/scripts/luts/AUX_RLUT_S6A_002.nc
+-rw-rw-r--   0 travis    (2000) travis    (2000)   214215 2023-06-23 09:07:23.000000 pysamosa-0.4.0/scripts/luts/AUX_RLUT_S6A_003.nc
+-rwxrwxr-x   0 travis    (2000) travis    (2000)  4818008 2023-06-23 09:07:23.000000 pysamosa-0.4.0/scripts/luts/F0.txt
+-rwxrwxr-x   0 travis    (2000) travis    (2000)  4827430 2023-06-23 09:07:23.000000 pysamosa-0.4.0/scripts/luts/F1.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)    30520 2023-06-23 09:07:23.000000 pysamosa-0.4.0/scripts/luts/LUT_Alpha_P_CS-2.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)   993604 2023-06-23 09:07:23.000000 pysamosa-0.4.0/scripts/luts/S6A_TEST_AUX_FLUT___00000000T000000_99999999T999999_0001.NC
+-rw-rw-r--   0 travis    (2000) travis    (2000)    30520 2023-06-23 09:07:23.000000 pysamosa-0.4.0/scripts/luts/alphap_table_SEN3_09_Nov_2017.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3215 2023-06-23 09:07:23.000000 pysamosa-0.4.0/scripts/luts/convert_luts.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9610 2023-06-23 09:07:23.000000 pysamosa-0.4.0/scripts/thesis_plots.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6110 2023-06-23 09:07:23.000000 pysamosa-0.4.0/scripts/track_browser.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9809 2023-06-23 09:07:23.000000 pysamosa-0.4.0/scripts/track_browser_footprint.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      436 2023-06-23 09:14:43.222287 pysamosa-0.4.0/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2405 2023-06-23 09:07:23.000000 pysamosa-0.4.0/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-23 09:14:43.218287 pysamosa-0.4.0/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2023-06-23 09:07:23.000000 pysamosa-0.4.0/tests/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10885 2023-06-23 09:07:23.000000 pysamosa-0.4.0/tests/helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2431 2023-06-23 09:07:23.000000 pysamosa-0.4.0/tests/settings_dumper.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2429 2023-06-23 09:07:23.000000 pysamosa-0.4.0/tests/test_common_types.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3305 2023-06-23 09:07:23.000000 pysamosa-0.4.0/tests/test_dist2coast.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5903 2023-06-23 09:07:23.000000 pysamosa-0.4.0/tests/test_dynamic_fg_epoch.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4328 2023-06-23 09:07:23.000000 pysamosa-0.4.0/tests/test_l1b_sim_retracker.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2093 2023-06-23 09:07:23.000000 pysamosa-0.4.0/tests/test_l1b_simulator.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1253 2023-06-23 09:07:23.000000 pysamosa-0.4.0/tests/test_leading_edge_detector.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9363 2023-06-23 09:07:23.000000 pysamosa-0.4.0/tests/test_model.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9434 2023-06-23 09:07:23.000000 pysamosa-0.4.0/tests/test_montecarlo_sim.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8236 2023-06-23 09:07:23.000000 pysamosa-0.4.0/tests/test_retrack_multi.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9035 2023-06-23 09:07:23.000000 pysamosa-0.4.0/tests/test_retrack_single.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4791 2023-06-23 09:07:23.000000 pysamosa-0.4.0/tests/test_samplusplus.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1111 2023-06-23 09:07:23.000000 pysamosa-0.4.0/tests/test_utils.py
```

### Comparing `pysamosa-0.3.0/PKG-INFO` & `pysamosa-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pysamosa
-Version: 0.3.0
+Version: 0.4.0
 Summary: PySAMOSA is a software framework for processing open ocean and coastal waveforms from SAR satellite altimetry to measure sea surface heights, wave heights, and wind speed for the oceans and inland water bodies. Satellite altimetry is a space-borne remote sensing technique used for Earth observation.
 Home-page: https://github.com/floschl/pysamosa
 Author: Florian Schlembach
 Author-email: florian.schlembach@tum.de
-License: GNU General Public License v3
+License: GNU Lesser General Public License v3 or later (LGPLv3+)
 Keywords: satellite altimetry retracking samosa+ samosa coastal open ocean sentinel esasar altimetry ff-sar fully focused
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
@@ -265,19 +265,17 @@
 If you use this software or the code, please cite this DOI:
 
 Florian Schlembach; Marcello Passaro. PySAMOSA: An Open-source Software Framework for Retracking SAMOSA-based, Open
 Ocean and Coastal Waveforms of SAR Satellite Altimetry. Zenodo. https://zenodo.org/badge/latestdoi/646028227.
 
 ## Acknowledgement
 
-Many thanks to
-- Salvatore Dinardo for his support in the implementation of the SAMOSA-based and SAMOSA+ [3] retracking algorithms in general, for the generation and provision of the $\alpha_p$ LUT tables
-- EUMETSAT for support in the alignment of the S6-MF retracking algorithm with the baseline processor.
-- Jérôme Benveniste for providing of the SAMOSA Detailed Processing Model (v2.5.2)
-- ESA L2 GPP Project: FF-SAR SAMOSA LUT generation was funded under ESA contract 4000118128/16/NL/AI.
+The authors are grateful to
+
+Salvatore Dinardo for his support in implementing the SAMOSA-based and SAMOSA+ [3] retracking algorithms.
 
 This package was created with [Cookiecutter](https://github.com/audreyr/cookiecutter) and the
 [audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage) project template.
 
 ## References
 
 [1] SAMOSA Detailed Processing Model: Christine Gommenginger, Cristina Martin-Puig, Meric Srokosz, Marco Caparrini, Salvatore Dinardo, Bruno Lucas, Marco Restano, Américo, Ambrózio and Jérôme Benveniste, Detailed Processing Model of the Sentinel-3 SRAL SAR altimeter ocean waveform retracker, Version 2.5.2, 31 October 2017, Under ESA-ESRIN Contract No. 20698/07/I-LG (SAMOSA), Restricted access as defined in the Contract,  Jérôme Benveniste (Jerome.Benvensite@esa.int) pers. comm.
```

### Comparing `pysamosa-0.3.0/README.md` & `pysamosa-0.4.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -243,19 +243,17 @@
 If you use this software or the code, please cite this DOI:
 
 Florian Schlembach; Marcello Passaro. PySAMOSA: An Open-source Software Framework for Retracking SAMOSA-based, Open
 Ocean and Coastal Waveforms of SAR Satellite Altimetry. Zenodo. https://zenodo.org/badge/latestdoi/646028227.
 
 ## Acknowledgement
 
-Many thanks to
-- Salvatore Dinardo for his support in the implementation of the SAMOSA-based and SAMOSA+ [3] retracking algorithms in general, for the generation and provision of the $\alpha_p$ LUT tables
-- EUMETSAT for support in the alignment of the S6-MF retracking algorithm with the baseline processor.
-- Jérôme Benveniste for providing of the SAMOSA Detailed Processing Model (v2.5.2)
-- ESA L2 GPP Project: FF-SAR SAMOSA LUT generation was funded under ESA contract 4000118128/16/NL/AI.
+The authors are grateful to
+
+Salvatore Dinardo for his support in implementing the SAMOSA-based and SAMOSA+ [3] retracking algorithms.
 
 This package was created with [Cookiecutter](https://github.com/audreyr/cookiecutter) and the
 [audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage) project template.
 
 ## References
 
 [1] SAMOSA Detailed Processing Model: Christine Gommenginger, Cristina Martin-Puig, Meric Srokosz, Marco Caparrini, Salvatore Dinardo, Bruno Lucas, Marco Restano, Américo, Ambrózio and Jérôme Benveniste, Detailed Processing Model of the Sentinel-3 SRAL SAR altimeter ocean waveform retracker, Version 2.5.2, 31 October 2017, Under ESA-ESRIN Contract No. 20698/07/I-LG (SAMOSA), Restricted access as defined in the Contract,  Jérôme Benveniste (Jerome.Benvensite@esa.int) pers. comm.
```

### Comparing `pysamosa-0.3.0/notebooks/retracking_example.ipynb` & `pysamosa-0.4.0/notebooks/retracking_example.ipynb`

 * *Files identical despite different names*

### Comparing `pysamosa-0.3.0/pysamosa/common_types.py` & `pysamosa-0.4.0/pysamosa/common_types.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.3.0/pysamosa/data_access.py` & `pysamosa-0.4.0/pysamosa/data_access.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.3.0/pysamosa/dist2coast.py` & `pysamosa-0.4.0/pysamosa/dist2coast.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.3.0/pysamosa/l1b_simulator.py` & `pysamosa-0.4.0/pysamosa/l1b_simulator.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.3.0/pysamosa/leading_edge_detector.py` & `pysamosa-0.4.0/pysamosa/leading_edge_detector.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.3.0/pysamosa/luts_samosa.pickle` & `pysamosa-0.4.0/pysamosa/luts_samosa.pickle`

 * *Files identical despite different names*

### Comparing `pysamosa-0.3.0/pysamosa/main_coastalffsar.py` & `pysamosa-0.4.0/pysamosa/main_coastalffsar.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.3.0/pysamosa/main_coral_paper.py` & `pysamosa-0.4.0/pysamosa/main_coral_paper.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.3.0/pysamosa/main_cs.py` & `pysamosa-0.4.0/pysamosa/main_cs.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.3.0/pysamosa/main_s3.py` & `pysamosa-0.4.0/pysamosa/main_s3.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.3.0/pysamosa/main_s6.py` & `pysamosa-0.4.0/pysamosa/main_s6.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.3.0/pysamosa/main_s6jtex.py` & `pysamosa-0.4.0/pysamosa/main_s6jtex.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.3.0/pysamosa/main_s6jtex_raw_vs_rmc.py` & `pysamosa-0.4.0/pysamosa/main_s6jtex_raw_vs_rmc.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.3.0/pysamosa/model.py` & `pysamosa-0.4.0/pysamosa/model.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.3.0/pysamosa/model_helpers.pyx` & `pysamosa-0.4.0/pysamosa/model_helpers.pyx`

 * *Files identical despite different names*

### Comparing `pysamosa-0.3.0/pysamosa/montecarlo_simulator.py` & `pysamosa-0.4.0/pysamosa/montecarlo_simulator.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.3.0/pysamosa/qual_flag_estimator.py` & `pysamosa-0.4.0/pysamosa/qual_flag_estimator.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.3.0/pysamosa/retracker.py` & `pysamosa-0.4.0/pysamosa/retracker.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.3.0/pysamosa/retracker_helpers.py` & `pysamosa-0.4.0/pysamosa/retracker_helpers.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.3.0/pysamosa/retracker_processor.py` & `pysamosa-0.4.0/pysamosa/retracker_processor.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.3.0/pysamosa/rip.py` & `pysamosa-0.4.0/pysamosa/rip.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.3.0/pysamosa/settings_manager.py` & `pysamosa-0.4.0/pysamosa/settings_manager.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.3.0/pysamosa/simple_logger.py` & `pysamosa-0.4.0/pysamosa/simple_logger.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.3.0/pysamosa/utils.py` & `pysamosa-0.4.0/pysamosa/utils.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.3.0/pysamosa.egg-info/PKG-INFO` & `pysamosa-0.4.0/pysamosa.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pysamosa
-Version: 0.3.0
+Version: 0.4.0
 Summary: PySAMOSA is a software framework for processing open ocean and coastal waveforms from SAR satellite altimetry to measure sea surface heights, wave heights, and wind speed for the oceans and inland water bodies. Satellite altimetry is a space-borne remote sensing technique used for Earth observation.
 Home-page: https://github.com/floschl/pysamosa
 Author: Florian Schlembach
 Author-email: florian.schlembach@tum.de
-License: GNU General Public License v3
+License: GNU Lesser General Public License v3 or later (LGPLv3+)
 Keywords: satellite altimetry retracking samosa+ samosa coastal open ocean sentinel esasar altimetry ff-sar fully focused
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
@@ -265,19 +265,17 @@
 If you use this software or the code, please cite this DOI:
 
 Florian Schlembach; Marcello Passaro. PySAMOSA: An Open-source Software Framework for Retracking SAMOSA-based, Open
 Ocean and Coastal Waveforms of SAR Satellite Altimetry. Zenodo. https://zenodo.org/badge/latestdoi/646028227.
 
 ## Acknowledgement
 
-Many thanks to
-- Salvatore Dinardo for his support in the implementation of the SAMOSA-based and SAMOSA+ [3] retracking algorithms in general, for the generation and provision of the $\alpha_p$ LUT tables
-- EUMETSAT for support in the alignment of the S6-MF retracking algorithm with the baseline processor.
-- Jérôme Benveniste for providing of the SAMOSA Detailed Processing Model (v2.5.2)
-- ESA L2 GPP Project: FF-SAR SAMOSA LUT generation was funded under ESA contract 4000118128/16/NL/AI.
+The authors are grateful to
+
+Salvatore Dinardo for his support in implementing the SAMOSA-based and SAMOSA+ [3] retracking algorithms.
 
 This package was created with [Cookiecutter](https://github.com/audreyr/cookiecutter) and the
 [audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage) project template.
 
 ## References
 
 [1] SAMOSA Detailed Processing Model: Christine Gommenginger, Cristina Martin-Puig, Meric Srokosz, Marco Caparrini, Salvatore Dinardo, Bruno Lucas, Marco Restano, Américo, Ambrózio and Jérôme Benveniste, Detailed Processing Model of the Sentinel-3 SRAL SAR altimeter ocean waveform retracker, Version 2.5.2, 31 October 2017, Under ESA-ESRIN Contract No. 20698/07/I-LG (SAMOSA), Restricted access as defined in the Contract,  Jérôme Benveniste (Jerome.Benvensite@esa.int) pers. comm.
```

### Comparing `pysamosa-0.3.0/pysamosa.egg-info/SOURCES.txt` & `pysamosa-0.4.0/pysamosa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pysamosa-0.3.0/scripts/cs_l2_conversion.py` & `pysamosa-0.4.0/scripts/cs_l2_conversion.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.3.0/scripts/luts/AUX_RLUT_S6A_002.nc` & `pysamosa-0.4.0/scripts/luts/AUX_RLUT_S6A_002.nc`

 * *Files identical despite different names*

### Comparing `pysamosa-0.3.0/scripts/luts/AUX_RLUT_S6A_003.nc` & `pysamosa-0.4.0/scripts/luts/AUX_RLUT_S6A_003.nc`

 * *Files identical despite different names*

### Comparing `pysamosa-0.3.0/scripts/luts/F0.txt` & `pysamosa-0.4.0/scripts/luts/F0.txt`

 * *Files identical despite different names*

### Comparing `pysamosa-0.3.0/scripts/luts/F1.txt` & `pysamosa-0.4.0/scripts/luts/F1.txt`

 * *Files identical despite different names*

### Comparing `pysamosa-0.3.0/scripts/luts/LUT_Alpha_P_CS-2.txt` & `pysamosa-0.4.0/scripts/luts/LUT_Alpha_P_CS-2.txt`

 * *Files identical despite different names*

### Comparing `pysamosa-0.3.0/scripts/luts/S6A_TEST_AUX_FLUT___00000000T000000_99999999T999999_0001.NC` & `pysamosa-0.4.0/scripts/luts/S6A_TEST_AUX_FLUT___00000000T000000_99999999T999999_0001.NC`

 * *Files identical despite different names*

### Comparing `pysamosa-0.3.0/scripts/luts/alphap_table_SEN3_09_Nov_2017.txt` & `pysamosa-0.4.0/scripts/luts/alphap_table_SEN3_09_Nov_2017.txt`

 * *Files identical despite different names*

### Comparing `pysamosa-0.3.0/scripts/luts/convert_luts.py` & `pysamosa-0.4.0/scripts/luts/convert_luts.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.3.0/scripts/thesis_plots.py` & `pysamosa-0.4.0/scripts/thesis_plots.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.3.0/scripts/track_browser.py` & `pysamosa-0.4.0/scripts/track_browser.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.3.0/scripts/track_browser_footprint.py` & `pysamosa-0.4.0/scripts/track_browser_footprint.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.3.0/setup.py` & `pysamosa-0.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,33 +43,33 @@
 setup(
     author="Florian Schlembach",
     author_email="florian.schlembach@tum.de",
     python_requires=">=3.8",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
-        "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
+        "License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
     ],
     description="PySAMOSA is a software framework for processing open ocean and coastal waveforms from SAR satellite altimetry to measure sea surface heights, wave heights, and wind speed for the oceans and inland water bodies. Satellite altimetry is a space-borne remote sensing technique used for Earth observation.",
     install_requires=requirements,
-    license="GNU General Public License v3",
+    license="GNU Lesser General Public License v3 or later (LGPLv3+)",
     long_description=readme,
     long_description_content_type="text/markdown",
     include_package_data=True,
     keywords="satellite altimetry retracking samosa+ samosa coastal open ocean sentinel esa"
     "sar altimetry ff-sar fully focused",
     name="pysamosa",
     packages=find_packages(include=["pysamosa", "pysamosa.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     ext_modules=extensions,
     url="https://github.com/floschl/pysamosa",
-    version="0.3.0",
+    version="0.4.0",
     zip_safe=False,
     setup_requires=[],
 )
```

### Comparing `pysamosa-0.3.0/tests/helpers.py` & `pysamosa-0.4.0/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.3.0/tests/settings_dumper.py` & `pysamosa-0.4.0/tests/settings_dumper.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.3.0/tests/test_common_types.py` & `pysamosa-0.4.0/tests/test_common_types.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.3.0/tests/test_dist2coast.py` & `pysamosa-0.4.0/tests/test_dist2coast.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.3.0/tests/test_dynamic_fg_epoch.py` & `pysamosa-0.4.0/tests/test_dynamic_fg_epoch.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.3.0/tests/test_l1b_sim_retracker.py` & `pysamosa-0.4.0/tests/test_l1b_sim_retracker.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.3.0/tests/test_l1b_simulator.py` & `pysamosa-0.4.0/tests/test_l1b_simulator.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.3.0/tests/test_leading_edge_detector.py` & `pysamosa-0.4.0/tests/test_leading_edge_detector.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.3.0/tests/test_model.py` & `pysamosa-0.4.0/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.3.0/tests/test_montecarlo_sim.py` & `pysamosa-0.4.0/tests/test_montecarlo_sim.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.3.0/tests/test_retrack_multi.py` & `pysamosa-0.4.0/tests/test_retrack_multi.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.3.0/tests/test_retrack_single.py` & `pysamosa-0.4.0/tests/test_retrack_single.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.3.0/tests/test_samplusplus.py` & `pysamosa-0.4.0/tests/test_samplusplus.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.3.0/tests/test_utils.py` & `pysamosa-0.4.0/tests/test_utils.py`

 * *Files identical despite different names*

