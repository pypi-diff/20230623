# Comparing `tmp/instamatic-1.9.0.tar.gz` & `tmp/instamatic-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instamatic-1.9.0.tar", last modified: Fri May 19 06:34:15 2023, max compression
+gzip compressed data, was "instamatic-2.0.0.tar", last modified: Fri Jun 23 09:49:20 2023, max compression
```

## Comparing `instamatic-1.9.0.tar` & `instamatic-2.0.0.tar`

### file list

```diff
@@ -1,252 +1,255 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:15.033219 instamatic-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-19 06:33:59.000000 instamatic-1.9.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-19 06:33:59.000000 instamatic-1.9.0/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-19 06:33:59.000000 instamatic-1.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-19 06:34:15.033219 instamatic-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-19 06:33:59.000000 instamatic-1.9.0/THANKS.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:14.997219 instamatic-1.9.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-05-19 06:33:59.000000 instamatic-1.9.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    14113 2023-05-19 06:33:59.000000 instamatic-1.9.0/docs/config.md
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-05-19 06:33:59.000000 instamatic-1.9.0/docs/formats.md
--rw-r--r--   0 runner    (1001) docker     (123)     8498 2023-05-19 06:33:59.000000 instamatic-1.9.0/docs/gui.md
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-05-19 06:33:59.000000 instamatic-1.9.0/docs/make_programs_md.py
--rw-r--r--   0 runner    (1001) docker     (123)    20542 2023-05-19 06:33:59.000000 instamatic-1.9.0/docs/programs.md
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-05-19 06:33:59.000000 instamatic-1.9.0/docs/setup.md
--rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-05-19 06:33:59.000000 instamatic-1.9.0/docs/tem_api.md
--rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-05-19 06:33:59.000000 instamatic-1.9.0/docs/tvips.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:14.997219 instamatic-1.9.0/instamatic/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:15.001219 instamatic-1.9.0/instamatic/TEMController/
--rw-r--r--   0 runner    (1001) docker     (123)    24729 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/TEMController/TEMController.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/TEMController/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/TEMController/deflectors.py
--rw-r--r--   0 runner    (1001) docker     (123)    15842 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/TEMController/fei_microscope.py
--rw-r--r--   0 runner    (1001) docker     (123)    12269 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/TEMController/fei_simu_microscope.py
--rw-r--r--   0 runner    (1001) docker     (123)    19453 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/TEMController/jeol_microscope.py
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/TEMController/lenses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/TEMController/microscope.py
--rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/TEMController/microscope_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17131 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/TEMController/simu_microscope.py
--rw-r--r--   0 runner    (1001) docker     (123)    10899 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/TEMController/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/TEMController/states.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6001 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/acquire_at_items.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/banner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/browser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:15.001219 instamatic-1.9.0/instamatic/calibrate/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/calibrate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10800 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/calibrate/calibrate_beamshift.py
--rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/calibrate/calibrate_brightness.py
--rw-r--r--   0 runner    (1001) docker     (123)    12279 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/calibrate/calibrate_directbeam.py
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/calibrate/calibrate_imageshift12.py
--rw-r--r--   0 runner    (1001) docker     (123)    13839 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/calibrate/calibrate_stage_lowmag.py
--rw-r--r--   0 runner    (1001) docker     (123)     8724 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/calibrate/calibrate_stage_mag1.py
--rw-r--r--   0 runner    (1001) docker     (123)    16127 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/calibrate/calibrate_stagematrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/calibrate/center_z.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/calibrate/filenames.py
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/calibrate/fit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:15.009219 instamatic-1.9.0/instamatic/camera/
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/camera/CCDCOM.h
--rw-r--r--   0 runner    (1001) docker     (123)    22528 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/camera/CCDCOM2_x64_gatan.dll
--rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/camera/CCDCOM2_x64_simulation.dll
--rw-r--r--   0 runner    (1001) docker     (123)    17920 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/camera/CCDCOM2_x86_gatan.dll
--rw-r--r--   0 runner    (1001) docker     (123)     8704 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/camera/CCDCOM2_x86_simulation.dll
--rw-r--r--   0 runner    (1001) docker     (123)    55808 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/camera/EMCameraObj.dll
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/camera/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/camera/camera.py
--rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/camera/camera_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18921 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/camera/camera_emmenu.py
--rw-r--r--   0 runner    (1001) docker     (123)     7844 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/camera/camera_gatan.py
--rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/camera/camera_gatan2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7802 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/camera/camera_merlin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/camera/camera_serval.py
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/camera/camera_simu.py
--rw-r--r--   0 runner    (1001) docker     (123)    10687 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/camera/camera_timepix.py
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/camera/fakevideostream.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/camera/gatansocket3.md
--rw-r--r--   0 runner    (1001) docker     (123)    25990 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/camera/gatansocket3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/camera/merlin_io.py
--rw-r--r--   0 runner    (1001) docker     (123)  1231360 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/camera/mpxhwrelaxd.dll
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/camera/timepix.lockfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:15.009219 instamatic-1.9.0/instamatic/camera/tpx/
--rw-r--r--   0 runner    (1001) docker     (123)   262144 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/camera/tpx/171207_with_flatfield.bpc
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/camera/tpx/171207_with_flatfield.bpc.dacs
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/camera/tpx/HW.dacs
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/camera/tpx/config.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/camera/videostream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:15.009219 instamatic-1.9.0/instamatic/config/
--rw-r--r--   0 runner    (1001) docker     (123)     8057 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:15.013219 instamatic-1.9.0/instamatic/config/alignments/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/config/alignments/neutral.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5743 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/config/autoconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:15.013219 instamatic-1.9.0/instamatic/config/calibration/
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/config/calibration/orius.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/config/calibration/simulate.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/config/calibration/timepix.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/config/calibration/tvips-f416.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:15.013219 instamatic-1.9.0/instamatic/config/camera/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/config/camera/merlin.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/config/camera/orius.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/config/camera/serval.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/config/camera/simulate.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/config/camera/simulateDLL.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/config/camera/timepix.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/config/camera/tvips-f416.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/config/camera/tvips-xf416.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/config/config_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/config/defaults.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:15.013219 instamatic-1.9.0/instamatic/config/microscope/
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/config/microscope/fei_simu.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/config/microscope/fei_themisZ.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/config/microscope/jeol-1400.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/config/microscope/jeol.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/config/microscope/simulate.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:15.013219 instamatic-1.9.0/instamatic/config/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/config/scripts/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/config/settings.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/config/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:15.013219 instamatic-1.9.0/instamatic/experiments/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/experiments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:15.013219 instamatic-1.9.0/instamatic/experiments/autocred/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/experiments/autocred/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    64484 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/experiments/autocred/experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:15.013219 instamatic-1.9.0/instamatic/experiments/cred/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/experiments/cred/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17207 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/experiments/cred/experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:15.017219 instamatic-1.9.0/instamatic/experiments/cred_gatan/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/experiments/cred_gatan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15867 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/experiments/cred_gatan/experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:15.017219 instamatic-1.9.0/instamatic/experiments/cred_tvips/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/experiments/cred_tvips/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20761 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/experiments/cred_tvips/experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:15.017219 instamatic-1.9.0/instamatic/experiments/red/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/experiments/red/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/experiments/red/experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:15.017219 instamatic-1.9.0/instamatic/experiments/serialed/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/experiments/serialed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21939 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/experiments/serialed/experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:15.017219 instamatic-1.9.0/instamatic/formats/
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/formats/adscimage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/formats/csvIO.py
--rw-r--r--   0 runner    (1001) docker     (123)    22681 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/formats/mrc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/formats/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/formats/xdscbf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/goniotool.py
--rw-r--r--   0 runner    (1001) docker     (123)     6978 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/gridmontage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:15.021219 instamatic-1.9.0/instamatic/gui/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/gui/about_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)    14841 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/gui/autocred_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/gui/base_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/gui/console_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/gui/cred_fei_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)    10230 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/gui/cred_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)    13898 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/gui/cred_tvips_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)    11528 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/gui/ctrl_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)    15000 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/gui/debug_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/gui/defocus_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/gui/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/gui/io_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/gui/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/gui/machine_learning_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/gui/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/gui/mpl_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/gui/red_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/gui/sed_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     9705 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/gui/videostream_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/imreg.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/montage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:15.021219 instamatic-1.9.0/instamatic/neural_network/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/neural_network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/neural_network/neural_network.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/neural_network/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/neural_network/preprocess_SerialRED.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:15.025219 instamatic-1.9.0/instamatic/processing/
--rw-r--r--   0 runner    (1001) docker     (123)    26808 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/processing/ImgConversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/processing/ImgConversionDM.py
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/processing/ImgConversionTPX.py
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/processing/ImgConversionTVIPS.py
--rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/processing/XDS_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/processing/XDS_templateDM.py
--rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/processing/XDS_templateTPX.py
--rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/processing/XDS_templateTVIPS.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/processing/find_crystals.py
--rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/processing/find_crystals_ilastik.py
--rw-r--r--   0 runner    (1001) docker     (123)     6409 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/processing/find_holes.py
--rw-r--r--   0 runner    (1001) docker     (123)     7936 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/processing/flatfield.py
--rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/processing/stretch_correction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:15.025219 instamatic-1.9.0/instamatic/server/
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/server/TEMServer_FEI.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/server/cam_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/server/cam_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/server/dials_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/server/goniotool_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/server/serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/server/tem_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/server/tem_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    10924 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/server/vm_ubuntu_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/server/xds_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     8921 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:15.025219 instamatic-1.9.0/instamatic/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/utils/beamstop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/utils/high_precision_timers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/utils/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/utils/singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/utils/spinbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     8539 2023-05-19 06:33:59.000000 instamatic-1.9.0/instamatic/utils/xds_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:15.001219 instamatic-1.9.0/instamatic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-19 06:34:14.000000 instamatic-1.9.0/instamatic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-05-19 06:34:14.000000 instamatic-1.9.0/instamatic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 06:34:14.000000 instamatic-1.9.0/instamatic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-05-19 06:34:14.000000 instamatic-1.9.0/instamatic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 06:34:14.000000 instamatic-1.9.0/instamatic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-19 06:34:14.000000 instamatic-1.9.0/instamatic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-19 06:34:14.000000 instamatic-1.9.0/instamatic.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:15.029219 instamatic-1.9.0/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)     8197 2023-05-19 06:33:59.000000 instamatic-1.9.0/notebooks/data_collection.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-05-19 06:33:59.000000 instamatic-1.9.0/notebooks/grid_montage_collection.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    13148 2023-05-19 06:33:59.000000 instamatic-1.9.0/notebooks/montage_processing.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11766 2023-05-19 06:33:59.000000 instamatic-1.9.0/notebooks/nav.nav
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-19 06:33:59.000000 instamatic-1.9.0/notebooks/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-05-19 06:33:59.000000 instamatic-1.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-19 06:33:59.000000 instamatic-1.9.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:15.029219 instamatic-1.9.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 06:33:59.000000 instamatic-1.9.0/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-05-19 06:33:59.000000 instamatic-1.9.0/scripts/browser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-19 06:33:59.000000 instamatic-1.9.0/scripts/center_images_smv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-05-19 06:33:59.000000 instamatic-1.9.0/scripts/diagnose_beam_drift.py
--rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-05-19 06:33:59.000000 instamatic-1.9.0/scripts/learn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-19 06:33:59.000000 instamatic-1.9.0/scripts/make_interval_movie.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-05-19 06:33:59.000000 instamatic-1.9.0/scripts/make_serialed_movie.py
--rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-05-19 06:33:59.000000 instamatic-1.9.0/scripts/process_dm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-05-19 06:33:59.000000 instamatic-1.9.0/scripts/process_tpx.py
--rw-r--r--   0 runner    (1001) docker     (123)     8790 2023-05-19 06:33:59.000000 instamatic-1.9.0/scripts/process_tvips.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-19 06:33:59.000000 instamatic-1.9.0/scripts/viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-05-19 06:34:15.033219 instamatic-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 06:33:59.000000 instamatic-1.9.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-19 06:33:59.000000 instamatic-1.9.0/setup_win.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:15.029219 instamatic-1.9.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:15.029219 instamatic-1.9.0/tests/config/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:15.033219 instamatic-1.9.0/tests/config/calibration/
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-19 06:33:59.000000 instamatic-1.9.0/tests/config/calibration/test.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:15.033219 instamatic-1.9.0/tests/config/camera/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-19 06:33:59.000000 instamatic-1.9.0/tests/config/camera/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-19 06:33:59.000000 instamatic-1.9.0/tests/config/defaults.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:34:15.033219 instamatic-1.9.0/tests/config/microscope/
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-19 06:33:59.000000 instamatic-1.9.0/tests/config/microscope/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-19 06:33:59.000000 instamatic-1.9.0/tests/config/settings.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-19 06:33:59.000000 instamatic-1.9.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-19 06:33:59.000000 instamatic-1.9.0/tests/test_camera.py
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-05-19 06:33:59.000000 instamatic-1.9.0/tests/test_ctrl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-05-19 06:33:59.000000 instamatic-1.9.0/tests/test_experiments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-19 06:33:59.000000 instamatic-1.9.0/tests/test_formats.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-19 06:33:59.000000 instamatic-1.9.0/tests/test_grid_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-19 06:33:59.000000 instamatic-1.9.0/tests/test_merlin_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.093809 instamatic-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-23 09:49:10.000000 instamatic-2.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-23 09:49:10.000000 instamatic-2.0.0/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-23 09:49:10.000000 instamatic-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-06-23 09:49:20.093809 instamatic-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-23 09:49:10.000000 instamatic-2.0.0/THANKS.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.049809 instamatic-2.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-23 09:49:10.000000 instamatic-2.0.0/docs/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-23 09:49:10.000000 instamatic-2.0.0/docs/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)   284790 2023-06-23 09:49:10.000000 instamatic-2.0.0/docs/banner.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14386 2023-06-23 09:49:10.000000 instamatic-2.0.0/docs/config.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-06-23 09:49:10.000000 instamatic-2.0.0/docs/formats.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8548 2023-06-23 09:49:10.000000 instamatic-2.0.0/docs/gui.md
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-23 09:49:10.000000 instamatic-2.0.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-06-23 09:49:10.000000 instamatic-2.0.0/docs/make_programs_md.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-06-23 09:49:10.000000 instamatic-2.0.0/docs/merlin.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-06-23 09:49:10.000000 instamatic-2.0.0/docs/network.md
+-rw-r--r--   0 runner    (1001) docker     (123)    20578 2023-06-23 09:49:10.000000 instamatic-2.0.0/docs/programs.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-06-23 09:49:10.000000 instamatic-2.0.0/docs/setup.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8975 2023-06-23 09:49:10.000000 instamatic-2.0.0/docs/tem_api.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-06-23 09:49:10.000000 instamatic-2.0.0/docs/tvips.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-06-23 09:49:10.000000 instamatic-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-23 09:49:10.000000 instamatic-2.0.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.049809 instamatic-2.0.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:10.000000 instamatic-2.0.0/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-06-23 09:49:10.000000 instamatic-2.0.0/scripts/browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-06-23 09:49:10.000000 instamatic-2.0.0/scripts/center_images_smv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-06-23 09:49:10.000000 instamatic-2.0.0/scripts/diagnose_beam_drift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-06-23 09:49:10.000000 instamatic-2.0.0/scripts/learn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-06-23 09:49:10.000000 instamatic-2.0.0/scripts/make_interval_movie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-06-23 09:49:10.000000 instamatic-2.0.0/scripts/make_serialed_movie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-06-23 09:49:10.000000 instamatic-2.0.0/scripts/process_dm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-06-23 09:49:10.000000 instamatic-2.0.0/scripts/process_tpx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8790 2023-06-23 09:49:10.000000 instamatic-2.0.0/scripts/process_tvips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-06-23 09:49:10.000000 instamatic-2.0.0/scripts/viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 09:49:20.093809 instamatic-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.041809 instamatic-2.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.053809 instamatic-2.0.0/src/instamatic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.057809 instamatic-2.0.0/src/instamatic/TEMController/
+-rw-r--r--   0 runner    (1001) docker     (123)    26129 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/TEMController/TEMController.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/TEMController/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/TEMController/deflectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15098 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/TEMController/fei_microscope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12272 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/TEMController/fei_simu_microscope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19456 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/TEMController/jeol_microscope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/TEMController/lenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/TEMController/microscope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/TEMController/microscope_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17133 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/TEMController/simu_microscope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11126 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/TEMController/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/TEMController/states.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6001 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/acquire_at_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/banner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/browser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.057809 instamatic-2.0.0/src/instamatic/calibrate/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/calibrate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10802 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/calibrate/calibrate_beamshift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/calibrate/calibrate_brightness.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12279 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/calibrate/calibrate_directbeam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/calibrate/calibrate_imageshift12.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13839 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/calibrate/calibrate_stage_lowmag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8724 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/calibrate/calibrate_stage_mag1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16130 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/calibrate/calibrate_stagematrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/calibrate/center_z.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/calibrate/filenames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/calibrate/fit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.065809 instamatic-2.0.0/src/instamatic/camera/
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/camera/CCDCOM.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22528 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/camera/CCDCOM2_x64_gatan.dll
+-rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/camera/CCDCOM2_x64_simulation.dll
+-rw-r--r--   0 runner    (1001) docker     (123)    17920 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/camera/CCDCOM2_x86_gatan.dll
+-rw-r--r--   0 runner    (1001) docker     (123)     8704 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/camera/CCDCOM2_x86_simulation.dll
+-rw-r--r--   0 runner    (1001) docker     (123)    55808 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/camera/EMCameraObj.dll
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/camera/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/camera/camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/camera/camera_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19013 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/camera/camera_emmenu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/camera/camera_gatan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/camera/camera_gatan2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14378 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/camera/camera_merlin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/camera/camera_serval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/camera/camera_simu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10738 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/camera/camera_timepix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/camera/fakevideostream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/camera/gatansocket3.md
+-rw-r--r--   0 runner    (1001) docker     (123)    25990 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/camera/gatansocket3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/camera/merlin_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1231360 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/camera/mpxhwrelaxd.dll
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/camera/timepix.lockfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.065809 instamatic-2.0.0/src/instamatic/camera/tpx/
+-rw-r--r--   0 runner    (1001) docker     (123)   262144 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/camera/tpx/171207_with_flatfield.bpc
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/camera/tpx/171207_with_flatfield.bpc.dacs
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/camera/tpx/HW.dacs
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/camera/tpx/config.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5965 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/camera/videostream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.069809 instamatic-2.0.0/src/instamatic/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     8057 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.069809 instamatic-2.0.0/src/instamatic/config/alignments/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/config/alignments/neutral.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/config/autoconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.069809 instamatic-2.0.0/src/instamatic/config/calibration/
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/config/calibration/orius.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/config/calibration/simulate.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/config/calibration/timepix.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/config/calibration/tvips-f416.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.069809 instamatic-2.0.0/src/instamatic/config/camera/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/config/camera/merlin.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/config/camera/orius.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/config/camera/serval.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/config/camera/simulate.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/config/camera/simulateDLL.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/config/camera/timepix.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/config/camera/tvips-f416.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/config/camera/tvips-xf416.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/config/config_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/config/defaults.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.069809 instamatic-2.0.0/src/instamatic/config/microscope/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/config/microscope/fei_simu.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/config/microscope/fei_themisZ.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/config/microscope/jeol-1400.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/config/microscope/jeol.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/config/microscope/simulate.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.073809 instamatic-2.0.0/src/instamatic/config/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/config/scripts/close_down.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/config/scripts/focus_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/config/scripts/hello_world.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/config/scripts/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/config/scripts/search_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/config/settings.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/config/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.073809 instamatic-2.0.0/src/instamatic/experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/experiments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.073809 instamatic-2.0.0/src/instamatic/experiments/autocred/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/experiments/autocred/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64494 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/experiments/autocred/experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.073809 instamatic-2.0.0/src/instamatic/experiments/cred/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/experiments/cred/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17207 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/experiments/cred/experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.073809 instamatic-2.0.0/src/instamatic/experiments/cred_gatan/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/experiments/cred_gatan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15871 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/experiments/cred_gatan/experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.073809 instamatic-2.0.0/src/instamatic/experiments/cred_tvips/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/experiments/cred_tvips/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20753 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/experiments/cred_tvips/experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.073809 instamatic-2.0.0/src/instamatic/experiments/red/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/experiments/red/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/experiments/red/experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.073809 instamatic-2.0.0/src/instamatic/experiments/serialed/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/experiments/serialed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21941 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/experiments/serialed/experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.077809 instamatic-2.0.0/src/instamatic/formats/
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/formats/adscimage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/formats/csvIO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22681 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/formats/mrc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/formats/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/formats/xdscbf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/goniotool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/gridmontage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.081809 instamatic-2.0.0/src/instamatic/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/gui/about_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14841 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/gui/autocred_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/gui/base_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/gui/console_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/gui/cred_fei_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10230 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/gui/cred_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13899 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/gui/cred_tvips_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11528 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/gui/ctrl_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15000 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/gui/debug_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/gui/defocus_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/gui/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/gui/io_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/gui/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/gui/machine_learning_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/gui/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/gui/mpl_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/gui/red_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/gui/sed_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9705 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/gui/videostream_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/imreg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/montage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.085809 instamatic-2.0.0/src/instamatic/neural_network/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/neural_network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/neural_network/neural_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/neural_network/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/neural_network/preprocess_SerialRED.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1503408 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/neural_network/weights-py2.p
+-rw-r--r--   0 runner    (1001) docker     (123)  1020951 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/neural_network/weights-py3.p
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.089809 instamatic-2.0.0/src/instamatic/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)    26808 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/processing/ImgConversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/processing/ImgConversionDM.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/processing/ImgConversionTPX.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/processing/ImgConversionTVIPS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/processing/XDS_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/processing/XDS_templateDM.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/processing/XDS_templateTPX.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/processing/XDS_templateTVIPS.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/processing/find_crystals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/processing/find_crystals_ilastik.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6409 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/processing/find_holes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7936 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/processing/flatfield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/processing/stretch_correction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.089809 instamatic-2.0.0/src/instamatic/server/
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/server/TEMServer_FEI.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/server/cam_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7106 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/server/cam_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/server/dials_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/server/goniotool_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/server/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/server/tem_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/server/tem_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10924 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/server/vm_ubuntu_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/server/xds_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8921 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.089809 instamatic-2.0.0/src/instamatic/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/utils/beamstop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/utils/high_precision_timers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/utils/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/utils/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/utils/spinbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8539 2023-06-23 09:49:10.000000 instamatic-2.0.0/src/instamatic/utils/xds_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.053809 instamatic-2.0.0/src/instamatic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-06-23 09:49:20.000000 instamatic-2.0.0/src/instamatic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7892 2023-06-23 09:49:20.000000 instamatic-2.0.0/src/instamatic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 09:49:20.000000 instamatic-2.0.0/src/instamatic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-23 09:49:20.000000 instamatic-2.0.0/src/instamatic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-23 09:49:20.000000 instamatic-2.0.0/src/instamatic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-23 09:49:20.000000 instamatic-2.0.0/src/instamatic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.093809 instamatic-2.0.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.093809 instamatic-2.0.0/tests/config/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.093809 instamatic-2.0.0/tests/config/calibration/
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-23 09:49:10.000000 instamatic-2.0.0/tests/config/calibration/test.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.093809 instamatic-2.0.0/tests/config/camera/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-23 09:49:10.000000 instamatic-2.0.0/tests/config/camera/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-23 09:49:10.000000 instamatic-2.0.0/tests/config/defaults.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:49:20.093809 instamatic-2.0.0/tests/config/microscope/
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-23 09:49:10.000000 instamatic-2.0.0/tests/config/microscope/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-23 09:49:10.000000 instamatic-2.0.0/tests/config/settings.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-23 09:49:10.000000 instamatic-2.0.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-23 09:49:10.000000 instamatic-2.0.0/tests/test_camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-06-23 09:49:10.000000 instamatic-2.0.0/tests/test_ctrl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-23 09:49:10.000000 instamatic-2.0.0/tests/test_experiments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-23 09:49:10.000000 instamatic-2.0.0/tests/test_formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-23 09:49:10.000000 instamatic-2.0.0/tests/test_grid_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-23 09:49:10.000000 instamatic-2.0.0/tests/test_merlin_io.py
```

### Comparing `instamatic-1.9.0/.pre-commit-config.yaml` & `instamatic-2.0.0/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 # See https://pre-commit.com for more information
 # See https://pre-commit.com/hooks.html for more hooks
 repos:
--   repo: https://github.com/pre-commit/pre-commit-hooks
+  - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
-    -   id: trailing-whitespace
+      - id: trailing-whitespace
         args: [--markdown-linebreak-ext=md]
-    -   id: end-of-file-fixer
-    -   id: check-yaml
-    -   id: check-docstring-first
-    -   id: check-builtin-literals
-    -   id: check-ast
-    -   id: check-merge-conflict
-    -   id: debug-statements
-    -   id: double-quote-string-fixer
-    # -   id: check-json
-    # -   id: check-added-large-files
--   repo: https://github.com/myint/docformatter
-    rev: v1.6.0
+      - id: end-of-file-fixer
+      - id: check-yaml
+      - id: check-docstring-first
+      - id: check-builtin-literals
+      - id: check-ast
+      - id: check-merge-conflict
+      - id: debug-statements
+      - id: double-quote-string-fixer
+    #   - id: check-json
+    #   - id: check-added-large-files
+  - repo: https://github.com/stefsmeets/nbcheckorder/
+    rev: v0.2.0
     hooks:
-    -   id: docformatter
--   repo: https://github.com/pre-commit/mirrors-autopep8
+      - id: nbcheckorder
+  - repo: https://github.com/myint/docformatter
+    rev: v1.7.2
+    hooks:
+      - id: docformatter
+  - repo: https://github.com/pre-commit/mirrors-autopep8
     rev: v2.0.2
     hooks:
-    -   id: autopep8
+      - id: autopep8
         args: ['--in-place', '--ignore=E501,W504']
--   repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: 'v0.0.261'
+  - repo: https://github.com/charliermarsh/ruff-pre-commit
+    rev: 'v0.0.272'
     hooks:
-    -   id: ruff
+      - id: ruff
         args: [--fix]
--   repo: https://github.com/kynan/nbstripout
-    rev: 0.6.1
-    hooks:
-    -   id: nbstripout
-        files: ".ipynb"
```

### Comparing `instamatic-1.9.0/LICENCE` & `instamatic-2.0.0/LICENCE`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/MANIFEST.in` & `instamatic-2.0.0/MANIFEST.in`

 * *Files 13% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 include docs/*.py
 include requirements.txt
 include scripts/*.py
 include setup_win.bat
 include tests/*.py
 include tests/config/*.yaml
 include tests/config/*/*.yaml
-include instamatic/camera/*.dll
-include instamatic/camera/*.h
-include instamatic/camera/*.lockfile
-include instamatic/camera/*.md
-include instamatic/camera/tpx/*.bpc
-include instamatic/camera/tpx/*.dacs
-include instamatic/camera/tpx/*.txt
-include instamatic/config/*.yaml
-include instamatic/config/alignments/*.yaml
-include instamatic/config/calibration/*.yaml
-include instamatic/config/camera/*.yaml
-include instamatic/config/microscope/*.yaml
-include instamatic/config/scripts/*.md
-include instamatic.neural_network/*.p
+include src/instamatic/camera/*.dll
+include src/instamatic/camera/*.h
+include src/instamatic/camera/*.lockfile
+include src/instamatic/camera/*.md
+include src/instamatic/camera/tpx/*.bpc
+include src/instamatic/camera/tpx/*.dacs
+include src/instamatic/camera/tpx/*.txt
+include src/instamatic/config/*.yaml
+include src/instamatic/config/alignments/*.yaml
+include src/instamatic/config/calibration/*.yaml
+include src/instamatic/config/camera/*.yaml
+include src/instamatic/config/microscope/*.yaml
+include src/instamatic/config/scripts/*.md
+include src/instamatic/neural_network/*.p
```

### Comparing `instamatic-1.9.0/PKG-INFO` & `instamatic-2.0.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: instamatic
-Version: 1.9.0
+Version: 2.0.0
 Summary: Python program for automated electron diffraction data collection
-Home-page: http://github.com/instamatic-dev/instamatic
-Author: Stef Smeets
-Author-email: s.smeets@esciencecenter.nl
-License: UNKNOWN
-Project-URL: Bug Tracker, http://github.com/instamatic-dev/instamatic/issues
-Project-URL: Documentation, https://instamatic.readthedocs.io/
+Author-email: Stef Smeets <s.smeets@esciencecenter.nl>
+License: BSD License
+Project-URL: homepage, https://github.com/instamatic-dev/instamatic
+Project-URL: issues, http://github.com/instamatic-dev/instamatic/issues
+Project-URL: documentation, https://instamatic.readthedocs.io
+Project-URL: changelog, https://github.com/instamatic-dev/instamatic/releases
 Keywords: electron-crystallography,electron-microscopy,electron-diffraction,serial-crystallography,3D-electron-diffraction,micro-ed,data-collection,automation
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Software Development :: Libraries
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: develop
 Provides-Extra: serval
+Provides-Extra: docs
+Provides-Extra: publishing
 License-File: LICENCE
-
-UNKNOWN
-
```

### Comparing `instamatic-1.9.0/THANKS.md` & `instamatic-2.0.0/THANKS.md`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/docs/config.md` & `instamatic-2.0.0/docs/config.md`

 * *Files 8% similar despite different names*

```diff
@@ -22,103 +22,100 @@
 
 You can run:
 ```bash
 instamatic.autoconfig.exe
 ```
 To help generate some of the input files (in particular templates for the microscope/calibration files).
 
-Examples of configuration files can be found [here](https://github.com/instamatic-dev/instamatic/tree/master/instamatic/config).
+Examples of configuration files can be found [here](https://github.com/instamatic-dev/instamatic/tree/main/src/instamatic/config).
 
 ## settings.yaml
 
 This is the global configuration file for `instamatic`. It defines which microscope / camera setup to use through the `microscope`, `camera`, and `calibration` settings.
 
-**microscope**  
-Name of the microscope calibration file use. For example, if this is set to `jeol-2100`, instamatic will look for the config file `jeol-2100.yaml` in the `config/microscope` directory.
+**microscope**
+: Name of the microscope calibration file use. For example, if this is set to `jeol-2100`, instamatic will look for the config file `jeol-2100.yaml` in the `config/microscope` directory.
 
-**camera**  
-Name of the camera file to use. Instamatic will look for the corresponding `.yaml` in the `config/camera` directory.
+**camera**
+: Name of the camera file to use. Instamatic will look for the corresponding `.yaml` in the `config/camera` directory.
 
-**calibration**  
-Name of the calibration file to use. Instamatic will look for the corresponding `.yaml` file in the `config/calibration` directory.
+**calibration**
+: Name of the calibration file to use. Instamatic will look for the corresponding `.yaml` file in the `config/calibration` directory.
 
 **simulate**
-Run instamatic in simulation mode. This simulates the connection to the microscope and the camera.
+: Run instamatic in simulation mode. This simulates the connection to the microscope and the camera.
 
-**data_directory**  
-Default path to where data should be stored, i.e. `C:/instamatic`.
+**data_directory**
+: Default path to where data should be stored, i.e. `C:/instamatic`.
 
-**flatfield**  
-Path to tiff file containing flatfield, i.e. `C:/instamatic/flatfield.tiff`. Leave blank if no flatfield should be applied.
+**flatfield**
+: Path to tiff file containing flatfield, i.e. `C:/instamatic/flatfield.tiff`. Leave blank if no flatfield should be applied.
 
-**use_tem_server**  
-Use the tem server with the given host/port below. If instamatic cannot find the tem server, it will start a new temserver in a subprocess. The tem server can be started using `instamatic.temserver.exe`. This helps to isolate the microscope communication. Instamatic will connect to the server via sockets. The main advantage is that a socket client can be run in a thread, whereas a COM connection makes problems if it is not in main thread.
+**use_tem_server**
+: Use the tem server with the given host/port below. If instamatic cannot find the tem server, it will start a new temserver in a subprocess. The tem server can be started using `instamatic.temserver.exe`. This helps to isolate the microscope communication. Instamatic will connect to the server via sockets. The main advantage is that a socket client can be run in a thread, whereas a COM connection makes problems if it is not in main thread.
 
-**tem_server_host**  
-Set this to `localhost` if the TEM server is run locally. To make a remote connection over the network, use `'0.0.0.0'` on the server (start using `instamatic.temserver.exe`, and the ip address of the server on the client.
+**tem_server_host**
+: Set this to `localhost` if the TEM server is run locally. To make a remote connection over the network, use `'0.0.0.0'` on the server (start using `instamatic.temserver.exe`, and the ip address of the server on the client.
 
-**tem_server_port**  
-The server port, default: `8088`.
+**tem_server_port**
+: The server port, default: `8088`.
 
 **tem_require_admin**
-Some microscopes require admin rights to access their API, set `tem_require_admin: True` to enable some checks for admin rights and request UAC elevation before enabling the connection. Default: `False`.
+: Some microscopes require admin rights to access their API, set `tem_require_admin: True` to enable some checks for admin rights and request UAC elevation before enabling the connection. Default: `False`.
 
-**use_cam_server**  
-Use the cam server with the given host/port below. If instamatic cannot find the cam server, it will start a new camserver in a subprocess. The cam server can be started using `instamatic.camserver.exe`. This helps to isolate the camera communication from the main program. Instamatic will connect to the server via sockets. The main advantage is that a socket client can be run in a thread, whereas a COM connection makes problems if it is not in main thread.
+**use_cam_server**
+: Use the cam server with the given host/port below. If instamatic cannot find the cam server, it will start a new camserver in a subprocess. The cam server can be started using `instamatic.camserver.exe`. This helps to isolate the camera communication from the main program. Instamatic will connect to the server via sockets. The main advantage is that a socket client can be run in a thread, whereas a COM connection makes problems if it is not in main thread.
 
-**cam_server_host**  
-Set this to `localhost` if the cam server is run locally. To make a remote connection over the network, use `'0.0.0.0'` on the server (start using `instamatic.camserver.exe`), and the ip address of the server on the client.
+**cam_server_host**
+: Set this to `localhost` if the cam server is run locally. To make a remote connection over the network, use `'0.0.0.0'` on the server (start using `instamatic.camserver.exe`), and the ip address of the server on the client.
 
-**cam_server_port**  
-The server port, default: `8087`.
+**cam_server_port**
+: The server port, default: `8087`.
 
-**cam_use_shared_memory**  
-Use [shared memory interface](https://docs.python.org/3/library/multiprocessing.shared_memory.html) for fast IPC of image data if the camera interface runs on the same computer as `instamatic` (Python 3.8+ only).
+**cam_use_shared_memory**
+: Use [shared memory interface](https://docs.python.org/3/library/multiprocessing.shared_memory.html) for fast IPC of image data if the camera interface runs on the same computer as `instamatic` (Python 3.8+ only).
 
-**indexing_server_exe**  
-After data are collected, the path where the data are saved can be sent to this program via a socket connection for automated data processing. Available are the dials indexing server (`instamatic.dialsserver.exe`) and the XDS indexing server (`instamatic.xdsserver.exe`).
+**indexing_server_exe**
+: After data are collected, the path where the data are saved can be sent to this program via a socket connection for automated data processing. Available are the dials indexing server (`instamatic.dialsserver.exe`) and the XDS indexing server (`instamatic.xdsserver.exe`).
 
-**indexing_server_host**  
-IP to use for the indexing server, similar to above.
+**indexing_server_host**
+: IP to use for the indexing server, similar to above.
 
-**indexing_server_port**  
-Port to use for the indexing server, default: `8089`.
+**indexing_server_port**
+: Port to use for the indexing server, default: `8089`.
 
-**dials_script**  
-The script that is run when the dials indexing server is used..
+**dials_script**
+: The script that is run when the dials indexing server is used..
 
-**cred_relax_beam_before_experiment**  
-Relax the beam before a CRED experiment (for testing only), default: `false`.
+**cred_relax_beam_before_experiment**
+: Relax the beam before a CRED experiment (for testing only), default: `false`.
 
-**cred_track_stage_positions**  
-Track the stage position during a CRED experiment (for testing only), default: `false`.
+**cred_track_stage_positions**
+: Track the stage position during a CRED experiment (for testing only), default: `false`.
 
-**modules**  
-List of modules to load for the GUI, must be one of {`cred`, `cred_tvips`, `cred_fei`, `sed`, `autocred`, `red`, `machine_learning`, `ctrl`, `debug`, `about`, `io`}.
-
-**Goniotool settings**  
-For JEOL only, automatically set the rotation speed via Goniotool (`instamatic.goniotool.exe`). These variables set up the remote connection.
+**modules**
+: List of modules to load for the GUI, must be one of {`cred`, `cred_tvips`, `cred_fei`, `sed`, `autocred`, `red`, `machine_learning`, `ctrl`, `debug`, `about`, `io`}.
 
+**Goniotool settings**
+: For JEOL only, automatically set the rotation speed via Goniotool (`instamatic.goniotool.exe`). These variables set up the remote connection.
 ```yaml
-`use_goniotool: False
-`goniotool_server_host: 'localhost'
-`goniotool_server_port: 8090
+use_goniotool: False
+goniotool_server_host: 'localhost'
+goniotool_server_port: 8090
 ```
 
-**FEI server settings**  
-Define here the host/port for InsteaDMatic to control the rotation speed on a FEI/TFS system. `InsteaDMatic` connects to an instance of `instamatic.temserver_fei.exe` running on this address,, which in turn connects to the microscope.
-
+**FEI server settings**
+: Define here the host/port for InsteaDMatic to control the rotation speed on a FEI/TFS system. `InsteaDMatic` connects to an instance of `instamatic.temserver_fei.exe` running on this address,, which in turn connects to the microscope.
 ```yaml
 fei_server_host: '192.168.12.1'
 fei_server_port: 8091
 ```
 
-**VM indexing server (XDS)**  
-Automatically submit the data to an indexing server running in a VM (VirtualBox).
-
+**VM indexing server (XDS)**
+: Automatically submit the data to an indexing server running in a VM (VirtualBox).
 ```yaml
 use_VM_server_exe: False
 VM_server_exe: 'instamatic.VMserver.exe'
 VM_server_host: 'localhost'
 VM_server_port: 8092
 VM_ID: "Ubuntu 14.04.3"
 VM_USERNAME: "lab6"
@@ -147,116 +144,110 @@
         +-- rot90: dict
         +-- pixelsize: dict
         +-- stagematrix: dict
 ```
 
 Here, `mag` can be any of the mag modes, i.e. `mag1`, `lowmag`, `samag`. Each child item contains some info about the orientation and size of the camera.
 
-**name**  
-Name of the corresponding camera interface. This variable is not used currently in the code.
-
-**diff/pixelsize**  
-Give here a list of camera lengths (as reported by the TEM) and the corresponding pixel dimensions in reciprocal angstrom (px/Å), separated by a `:`, for example:
+**name**
+: Name of the corresponding camera interface. This variable is not used currently in the code.
 
+**diff/pixelsize**
+: Give here a list of camera lengths (as reported by the TEM) and the corresponding pixel dimensions in reciprocal angstrom (px/Å), separated by a `:`, for example:
 ```yaml
 diff:
   pixelsize:
     150: 0.02942304
     200: 0.02206728
     250: 0.017653824
 ```
 
 **mag/flipud**
-Flip the images around the horizontal axes. This is used to globally modify all images taken by the camera using `ctrl.get_image()` or `ctrl.get_rotated_image()` to make them in line with the fluorescence screen or otherwise. Default: False.
+: Flip the images around the horizontal axes. This is used to globally modify all images taken by the camera using `ctrl.get_image()` or `ctrl.get_rotated_image()` to make them in line with the fluorescence screen or otherwise. Default: False.
 
 **mag/fliplr**
-Similar to above, except that the images are flipped around the vertical axis. Default: False.
+: Similar to above, except that the images are flipped around the vertical axis. Default: False.
 
 **mag/rot90**
-Similar to above, this defines a rotation to be applied to every image. This was implemented to circumvent an issue on our TEM where images where the lenses incurred a -90 degrees rotation from lowmag 250x to 1000x. If not defined, the default is 0.
-
+: Similar to above, this defines a rotation to be applied to every image. This was implemented to circumvent an issue on our TEM where images where the lenses incurred a -90 degrees rotation from lowmag 250x to 1000x. If not defined, the default is 0.
 ```yaml
 lowmag:
   rot90:
     150: 0
     200: 0
     250: 3
 ```
 
-**mag/pixelsize**  
-Give here the magnification and pixel size for images taken in lowmag/mag1 mode in nanometer (nm), for example:
-
+**mag/pixelsize**
+: Give here the magnification and pixel size for images taken in lowmag/mag1 mode in nanometer (nm), for example:
 ```yaml
 lowmag:
   pixelsize:
     150: 77.71
     200: 59.31
     250: 45.36
 ```
 
-**mag/stagematrix**  
-This is a mapping of the pixel coordinates to the stage coordinates. These are used to convert from detected shifts in pixel coordinates (i.e. using cross correlation) to the corresponding translation of the stage. They can be calibrated using `instamatic.calibrate_stagematrix.exe`.
-
-The stagematrix is the *inverse* of the one defined using SerialEM (`StageToCameraMatrix` in `SerialEMCalibration.txt`) via _Calibration_ > _Image & Stage Shift_ > _Stage Shift_ ([link](http://bio3d.colorado.edu/SerialEM/betaHlp/html/menu_calibration.htm#hid_calibration_stageshift)). Note that the stagematrix is dependent on the orientation of the images.
+**mag/stagematrix**
+: This is a mapping of the pixel coordinates to the stage coordinates. These are used to convert from detected shifts in pixel coordinates (i.e. using cross correlation) to the corresponding translation of the stage. They can be calibrated using `instamatic.calibrate_stagematrix.exe`.
 
+: The stagematrix is the *inverse* of the one defined using SerialEM (`StageToCameraMatrix` in `SerialEMCalibration.txt`) via _Calibration_ > _Image & Stage Shift_ > _Stage Shift_ ([link](http://bio3d.colorado.edu/SerialEM/betaHlp/html/menu_calibration.htm#hid_calibration_stageshift)). Note that the stagematrix is dependent on the orientation of the images.
 ```yaml
 mag:
   stagematrix:
     250: [ 0.276258, -21.935572, 22.306572, 0.565116 ]
     300: [ 0.331509, -26.322686, 26.767886, 0.678139 ]
     400: [ 0.442012, -35.096915, 35.690515, 0.904185 ]
 ```
 
 ## camera.yaml:
 
 This file holds the specifications of the camera. This file is must be located the `config/camera` directory, and can have any name as defined in `settings.yaml`.
 
-**interface**  
-Give the interface of the camera interface to connect to, for example: `timepix`/`emmenu`/`simulate`/`gatan`/'merlin'. Leave blank to load the camera specs, but do not load the camera module (this also turns off the videostream gui).
+**interface**
+: Give the interface of the camera interface to connect to, for example: `timepix`/`emmenu`/`simulate`/`gatan`/`merlin`. Leave blank or set to `None` to load the camera specs, but do not load the camera module (this also turns off the videostream gui).
 
-**default_binsize**  
-Set the default binsize, default: `1`.
+**default_binsize**
+: Set the default binsize, default: `1`.
 
-**default_exposure**  
-Set the default exposure in seconds, i.e. `0.02`.
+**default_exposure**
+: Set the default exposure in seconds, i.e. `0.02`.
 
-**dimensions**  
-Give the dimensions of the camera at binning 1, for example: `[516, 516]`.
+**dimensions**
+: Give the dimensions of the camera at binning 1, for example: `[516, 516]`.
 
-**dynamic_range**  
-Give the maximum counts of the camera, for example: `11800`. This is used for the contrast in the liveview and the flatfield collection.
+**dynamic_range**
+: Give the maximum counts of the camera, for example: `11800`. This is used for the contrast in the liveview and the flatfield collection.
 
-**physical_pixelsize**  
-The physical size of a pixel in millimeter, for example: `0.055`.
+**physical_pixelsize**
+: The physical size of a pixel in millimeter, for example: `0.055`.
 
-**possible_binsizes**  
-Give here a list of possible binnings, for example: `[1]` or `[1, 2, 4]`.
+**possible_binsizes**
+: Give here a list of possible binnings, for example: `[1]` or `[1, 2, 4]`.
 
-**camera_rotation_vs_stage_xy**  
-In radians, give here the rotation of the position of the rotation axis with respect to the horizontal. Used for diffraction only. Corresponds to the rotation axis in RED and PETS, for example: `-2.24`. You can find the rotation axis for your setup using the script `edtools.find_rotation_axis` available from [here](https://github.com/instamatic-dev/edtools#find_rotation_axispy).
+**camera_rotation_vs_stage_xy**
+: In radians, give here the rotation of the position of the rotation axis with respect to the horizontal. Used for diffraction only. Corresponds to the rotation axis in RED and PETS, for example: `-2.24`. You can find the rotation axis for your setup using the script `edtools.find_rotation_axis` available from [here](https://github.com/instamatic-dev/edtools#find_rotation_axispy).
 
-**stretch_amplitude**  
-Use `instamatic.stretch_correction` to characterize the lens distortion. The numbers here are used to calculate the XCORR/YCORR maps. The amplitude is the percentage difference between the maximum and minimum eigenvectors of the ellipsoid, i.e. if the amplitude is `2.43`, eig(max)/eig(min) = 1.0243. You can use the program `instamatic.stretch_correction` available [here](https://github.com/instamatic-dev/instamatic/blob/master/docs/programs.md#instamaticstretch_correction) on some powder patterns to define these numbers.
+**stretch_amplitude**
+: Use `instamatic.stretch_correction` to characterize the lens distortion. The numbers here are used to calculate the XCORR/YCORR maps. The amplitude is the percentage difference between the maximum and minimum eigenvectors of the ellipsoid, i.e. if the amplitude is `2.43`, eig(max)/eig(min) = 1.0243. You can use the program `instamatic.stretch_correction` available [here](https://github.com/instamatic-dev/instamatic/blob/main/docs/programs.md#instamaticstretch_correction) on some powder patterns to define these numbers.
 
-**stretch_azimuth**  
-The azimuth is gives the direction of the maximum eigenvector with respect to the horizontal X-axis (pointing right) in degrees, for example: `83.37`.
+**stretch_azimuth**
+: The azimuth is gives the direction of the maximum eigenvector with respect to the horizontal X-axis (pointing right) in degrees, for example: `83.37`.
 
-**correction_ratio**  
-Set the correction ratio for the cross pixels in the Timepix detector, default: 3.
-
-**calib_beamshift**  
-Set up the grid and stepsize for the calibration of the beam shift in SerialED. The calibration will run a grid of `stepsize` by `stepsize` points, with steps of `stepsize`. The stepsize must be given corresponding to 2500x, and instamatic will then adjust the stepsize depending on the actual magnification, if needed. For example:
+**correction_ratio**
+: Set the correction ratio for the cross pixels in the Timepix detector, default: 3.
 
+**calib_beamshift**
+: Set up the grid and stepsize for the calibration of the beam shift in SerialED. The calibration will run a grid of `stepsize` by `stepsize` points, with steps of `stepsize`. The stepsize must be given corresponding to 2500x, and instamatic will then adjust the stepsize depending on the actual magnification, if needed. For example:
 ```yaml
 {gridsize: 5, stepsize: 500}
 ```
 
-**calib_directbeam**  
-Set up the grid and stepsize for the calibration of the direct beam in diffraction mode, for example:
-
+**calib_directbeam**
+: Set up the grid and stepsize for the calibration of the direct beam in diffraction mode, for example:
 ```yaml
   BeamShift: {gridsize: 5, stepsize: 300}
   DiffShift: {gridsize: 5, stepsize: 300}
 ```
 
 ## microscope.yaml
 
@@ -267,35 +258,42 @@
     +-- interface: str
     +-- wavelength: float
     +-- ranges
         +-- diff: list
         +-- mag: list
 ```
 
-**interface**  
-Defines the the microscope interface to use, i.e. 'jeol', 'fei', 'simulate'.
+**interface**
+: Defines the the microscope interface to use, i.e. 'jeol', 'fei', 'simulate'.
 
-**wavelength**  
-The wavelength of the microscope in Ansgtroms. This is used to generate some of the output files after data collection, i.e. for 120kV: `0.033492`, 200kV: `0.025079`, or 300 kV: `0.019687`. A useful website to calculate the de Broglie wavelength can be found [here](https://www.ou.edu/research/electron/bmz5364/calc-kv.html).
+**wavelength**
+: The wavelength of the microscope in Ansgtroms. This is used to generate some of the output files after data collection, i.e. for 120kV: `0.033492`, 200kV: `0.025079`, or 300 kV: `0.019687`. A useful website to calculate the de Broglie wavelength can be found [here](https://www.ou.edu/research/electron/bmz5364/calc-kv.html).
 
 **ranges**
-In the child items, all the magnification ranges must be defined. They can be obtained through the API using: `ctrl.magnification.get_ranges()`. This will step through all the magnifications and return them as a dictionary.
-
-**range/diff**  
-List here the available camera lengths available on the microscope in ascending order:
+: In the child items, all the magnification ranges must be defined. They can be obtained through the API using: `ctrl.magnification.get_ranges()`. This will step through all the magnifications and return them as a dictionary.
 
+**ranges/diff**
+: List here the available camera lengths available on the microscope in ascending order:
 ```yaml
 ranges:
   diff: [150, 200, 250, 300, 400, 500, 600, 800, 1000,
     1200, 1500, 2000, 2500, 3000, 3500, 4000, 4500]
 ```
 
-**ranges/mag**  
-Here, mag must be one of the known mag ranges, i.e. `lowmag`, `mag1`, `samag`. What follows is a list of all available magnifications on the microscope in ascending order, for example:
+!!! note
+
+    For FEI/TFS machines, use `range/D` instead of `ranges/diff`.
+
+**ranges/mag**
+: Here, mag must be one of the known mag ranges, i.e. `lowmag`, `mag1`, `samag`. What follows is a list of all available magnifications on the microscope in ascending order, for example:
 ```yaml
 ranges:
   mag1: [2000, 2500, 3000, 4000, 5000, 6000, 8000, 10000,
     12000, 15000, 20000, 25000, 30000, 40000, 50000, 60000,
     80000, 100000, 120000, 150000, 200000, 250000, 300000,
     400000, 500000, 600000, 800000, 1000000, 1200000,
     1500000, 2000000]
 ```
+
+!!! note
+
+    For FEI/TFS machines, the ranges are instead set as: `LM` (lowmag), `Mi` (low/intermediate mag), `SA` (high mag), `Mh` (highest mag), and `D` (diffraction mode).
```

### Comparing `instamatic-1.9.0/docs/formats.md` & `instamatic-2.0.0/docs/formats.md`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/docs/gui.md` & `instamatic-2.0.0/docs/gui.md`

 * *Files 5% similar despite different names*

```diff
@@ -18,57 +18,57 @@
 Module: `io`
 
 This panel deals with input and output of the experimental data.
 
 ![Input and output](images/gui_io.png)
 
 **Directory**  
-Root directory to work in. By default this is `C:/instamatic/$date/`
+: Root directory to work in. By default this is `C:/instamatic/$date/`
 
 **Sample name and number**  
-This determines the subdirectory where experimental data are stored.
+: This determines the subdirectory where experimental data are stored.
 The number is automatically incremented when a new experiment is started. Data are never overwritten.
 
 **Flatfield**  
-Here the path to the flatfield image can be specified. The default
+: Here the path to the flatfield image can be specified. The default
 value is read from `config/settings.yaml` and can be left blank if no flatfield should be used.
 
 **Open work directory**  
-Open the current work directory, which is a combination of the root
+: Open the current work directory, which is a combination of the root
 directory, sample name, and experiment number. In this case `C:/instamatic/work_2017-11-19/experiment_1`. All experimental data for the current experiment will be saved here.
 
 **Open config directory**  
-By default `%APPDATA%/instamatic/`. The configuration files for the
+: By default `%APPDATA%/instamatic/`. The configuration files for the
 microscope, camera, and calibration files go here.
 
 **Delete last experiment**  
-Sometimes, a data collection will go wrong... Pressing this button will
+: Sometimes, a data collection will go wrong... Pressing this button will
 mark the last experiment directy for deletion. It will not actually delete anything, but you will at least know which ones to delete afterwards :-)
 
 
 ## Console
 
 Module: `console`
 
 If enabled, this panel logs the console output.
 
 **Test**  
-Print a test message.
+: Print a test message.
 
 **Clear**  
-Clears the console.
+: Clears the console.
 
 **Export**  
-Opens a file browser to export the console output to a text file
+: Opens a file browser to export the console output to a text file
 
 **Capture**  
-Check this toggle to redirect the output from `stdout`.
+: Check this toggle to redirect the output from `stdout`.
 
 **Timestamp**  
-Check this toggle to prepend timestamps to each message.
+: Check this toggle to prepend timestamps to each message.
 
 ![Console](images/gui_console.png)
 
 
 ## SerialED data collection
 
 Module: `sed`
@@ -76,84 +76,84 @@
 Serial electron diffraction (serialED) is a technique to collect diffraction data on a large number of crystals. One diffraction pattern per crystal is collected. These can then be combined for structure determination, or used for screening/phase analysis.
 
 ![serial electron diffraction pane](images/gui_serialed.png)
 
 Data collection can be started from the ‘serialED’ tab by pressing the ‘Start Collection’ button. Follow the instructions in the terminal to setup and calibrate the experiment.
 
 **Scan area**  
-Radius for the area to scan area for crystals (in micrometer).
+: Radius for the area to scan area for crystals (in micrometer).
 
 **Exp. time image**  
-Exposure time for images.
+: Exposure time for images.
 
 **Exp. time diff**  
-Exposure time for diffraction pattern.
+: Exposure time for diffraction pattern.
 
 **Brightness**  
-Default value for the brightness of the focused beam.
+: Default value for the brightness of the focused beam.
 
 **Spot size**  
-Spot size to use.
+: Spot size to use.
 
 
 ## cRED data collection
 
 Module: `cred`
 
 Continuous RED (cRED) data collection can be started from the `cRED` tab.
 
 The data collection procedure can be initiated by pressing ‘Start Collection’. The program will then wait for the rotation to start. The moment the pedal is pressed to start the rotation, the program will start the data collection with the specified options. Do not release your foot until after you press ‘Stop Collection’. This will signal the program to stop data collection, and write the images. Images are written in TIFF, MRC, and SMV format. Input files for REDp (.ed3d) and XDS (XDS.INP) are also written.
 
 ![Continous rotation electron diffraction pane](images/gui_cred.png)
 
 **Exposure time**  
-change the data collection time for each image.
+: change the data collection time for each image.
 
 **Beam unblanker**  
-If this option is selected, the beam will be automatically unblanked
+: If this option is selected, the beam will be automatically unblanked
 when data collection starts, and blanked after data collection has finished (i.e. after ‘Stop Collection’ has been pressed)
 
 ### Image interval
 
 With this feature, an image of the crystal will be shown every N frames. This is useful to control the position of the crystal in the beam for more reliable and reproducable data collections. This is achieved by applying a small defocus (diffraction focus) to every Nth image. a small defocus of the diffraction focus. If the defocus is large enough, this will show a view of the crystal in the aperture.
 
 **Enable Image interval**  
-This option will enable the image interval.
+: This option will enable the image interval.
 
 **Image interval**  
-Change the interval at which the image will be defocused. For example,
+: Change the interval at which the image will be defocused. For example,
 if the value is 10, then every 10th image will be defocused.
 
 **Diff. defocus**  
-This is the defocus value to apply. It is better not to make this value
+: This is the defocus value to apply. It is better not to make this value
 too large, because the larger the difference with the proper diffraction focus, the longer the lenses need to recover. The microscope has to switch to the defocus value, take an image, and back within the time it takes to collect a single image (i.e. 0.5 s in this example).
 
 **Toggle defocus**  
-This toggle applies the defocus value, which is used for checking. It
+: This toggle applies the defocus value, which is used for checking. It
 does not affect the data collection.
 
 Other specific cRED modules: `cred_fei`, `cred_tvips`, `autocred`
 
 
 ## RED data collection
 
 Module: `red`
 
 Simple module to collect electron diffraction using discrete rotation steps.
 
 Pressing `Start Collection` will collect a series of frames with the given tilt step and range. The data collection is then paused, enabling the user to recenter the crystal or finalize the data collection. The program will automatically switch to diffraction mode if it is in image mode, and go back to image mode afterwards. Pressing `Continue` will continue from the current point, and collect another series of frames with the given tilt range. Pressing `Finalize` will, not unsurprisingly, finalize the data collection, save the data, and write any input files.
 
 **Exposure time**  
-The exposure time for each frame in seconds
+: The exposure time for each frame in seconds
 
 **Tilt range**  
-The total tilt range for the next sequence in degrees
+: The total tilt range for the next sequence in degrees
 
 **Step size**  
-The step size in degrees
+: The step size in degrees
 
 Data are output to `.tiff` and `.mrc`, including input files to read the data in PETS and REDp.
 
 
 ## Machine learning
 
 Module: `machine_learning`
```

### Comparing `instamatic-1.9.0/docs/make_programs_md.py` & `instamatic-2.0.0/docs/make_programs_md.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/docs/programs.md` & `instamatic-2.0.0/docs/programs.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,192 +1,240 @@
 # Programs and scripts
 
 There are several programs coming with `instamatic`. These docs are autogenerated from the program description (*i.e.* `instamatic -h`).
 
-- **Main**
-  + [instamatic](#instamatic) (`instamatic.main:main`)
-  + [instamatic.controller](#instamaticcontroller) (`instamatic.TEMController.TEMController:main_entry`)
-- **Experiments**
-  + [instamatic.serialed](#instamaticserialed) (`instamatic.experiments.serialed.experiment:main`)
-  + [instamatic.camera](#instamaticcamera) (`instamatic.camera.camera:main_entry`)
-- **Calibrate**
-  + [instamatic.calibrate_stage_lowmag](#instamaticcalibrate_stage_lowmag) (`instamatic.calibrate.calibrate_stage_lowmag:main_entry`)
-  + [instamatic.calibrate_stage_mag1](#instamaticcalibrate_stage_mag1) (`instamatic.calibrate.calibrate_stage_mag1:main_entry`)
-  + [instamatic.calibrate_beamshift](#instamaticcalibrate_beamshift) (`instamatic.calibrate.calibrate_beamshift:main_entry`)
-  + [instamatic.calibrate_directbeam](#instamaticcalibrate_directbeam) (`instamatic.calibrate.calibrate_directbeam:main_entry`)
-  + [instamatic.calibrate_stagematrix](#instamaticcalibrate_stagematrix) (`instamatic.calibrate.calibrate_stagematrix:main_entry`)
-  + [instamatic.flatfield](#instamaticflatfield) (`instamatic.processing.flatfield:main_entry`)
-  + [instamatic.stretch_correction](#instamaticstretch_correction) (`instamatic.processing.stretch_correction:main_entry`)
-- **Tools**
-  + [instamatic.browser](#instamaticbrowser) (`scripts.browser:main`)
-  + [instamatic.viewer](#instamaticviewer) (`scripts.viewer:main`)
-  + [instamatic.defocus_helper](#instamaticdefocus_helper) (`instamatic.gui.defocus_button:main`)
-  + [instamatic.find_crystals](#instamaticfind_crystals) (`instamatic.processing.find_crystals:main_entry`)
-  + [instamatic.find_crystals_ilastik](#instamaticfind_crystals_ilastik) (`instamatic.processing.find_crystals_ilastik:main_entry`)
-  + [instamatic.learn](#instamaticlearn) (`scripts.learn:main_entry`)
-- **Server**
-  + [instamatic.temserver](#instamatictemserver) (`instamatic.server.tem_server:main`)
-  + [instamatic.camserver](#instamaticcamserver) (`instamatic.server.cam_server:main`)
-  + [instamatic.dialsserver](#instamaticdialsserver) (`instamatic.server.dials_server:main`)
-  + [instamatic.VMserver](#instamaticVMserver) (`instamatic.server.vm_ubuntu_server:main`)
-  + [instamatic.xdsserver](#instamaticxdsserver) (`instamatic.server.xds_server:main`)
-  + [instamatic.temserver_fei](#instamatictemserver_fei) (`instamatic.server.TEMServer_FEI:main`)
-  + [instamatic.goniotoolserver](#instamaticgoniotoolserver) (`instamatic.server.goniotool_server:main`)
-- **Setup**
-  + [instamatic.autoconfig](#instamaticautoconfig) (`instamatic.config.autoconfig:main`)
-  + [instamatic.install](#instamaticinstall) (Cmder)
+**Main**
+
+These are the main tools to work with instamatic.
+
+- [instamatic](#instamatic) (`instamatic.main:main`)
+- [instamatic.controller](#instamaticcontroller) (`instamatic.TEMController.TEMController:main_entry`)
+
+**Experiments**
+
+These are specialized programs to run a particular subroutine of instamatic.
+
+- [instamatic.serialed](#instamaticserialed) (`instamatic.experiments.serialed.experiment:main`)
+- [instamatic.camera](#instamaticcamera) (`instamatic.camera.camera:main_entry`)
+
+**Calibrate**
+
+These tools help calibrate instamatic for some experiments.
+
+- [instamatic.calibrate_stage_lowmag](#instamaticcalibrate_stage_lowmag) (`instamatic.calibrate.calibrate_stage_lowmag:main_entry`)
+- [instamatic.calibrate_stage_mag1](#instamaticcalibrate_stage_mag1) (`instamatic.calibrate.calibrate_stage_mag1:main_entry`)
+- [instamatic.calibrate_beamshift](#instamaticcalibrate_beamshift) (`instamatic.calibrate.calibrate_beamshift:main_entry`)
+- [instamatic.calibrate_directbeam](#instamaticcalibrate_directbeam) (`instamatic.calibrate.calibrate_directbeam:main_entry`)
+- [instamatic.calibrate_stagematrix](#instamaticcalibrate_stagematrix) (`instamatic.calibrate.calibrate_stagematrix:main_entry`)
+- [instamatic.flatfield](#instamaticflatfield) (`instamatic.processing.flatfield:main_entry`)
+- [instamatic.stretch_correction](#instamaticstretch_correction) (`instamatic.processing.stretch_correction:main_entry`)
+
+**Tools**
+
+Arbitrary tools for viewing, analyzing, or working with instamatic data.
+
+- [instamatic.browser](#instamaticbrowser) (`scripts.browser:main`)
+- [instamatic.viewer](#instamaticviewer) (`scripts.viewer:main`)
+- [instamatic.defocus_helper](#instamaticdefocus_helper) (`instamatic.gui.defocus_button:main`)
+- [instamatic.find_crystals](#instamaticfind_crystals) (`instamatic.processing.find_crystals:main_entry`)
+- [instamatic.find_crystals_ilastik](#instamaticfind_crystals_ilastik) (`instamatic.processing.find_crystals_ilastik:main_entry`)
+- [instamatic.learn](#instamaticlearn) (`scripts.learn:main_entry`)
+
+**Server**
+
+Instamatic has several servers built-in that can be used to communicate over a socket or network interface.
+
+- [instamatic.temserver](#instamatictemserver) (`instamatic.server.tem_server:main`)
+- [instamatic.camserver](#instamaticcamserver) (`instamatic.server.cam_server:main`)
+- [instamatic.dialsserver](#instamaticdialsserver) (`instamatic.server.dials_server:main`)
+- [instamatic.VMserver](#instamaticVMserver) (`instamatic.server.vm_ubuntu_server:main`)
+- [instamatic.xdsserver](#instamaticxdsserver) (`instamatic.server.xds_server:main`)
+- [instamatic.temserver_fei](#instamatictemserver_fei) (`instamatic.server.TEMServer_FEI:main`)
+- [instamatic.goniotoolserver](#instamaticgoniotoolserver) (`instamatic.server.goniotool_server:main`)
+
+**Setup**
+
+Help set up instamatic.
+
+- [instamatic.autoconfig](#instamaticautoconfig) (`instamatic.config.autoconfig:main`)
 
 
 ## instamatic
 
 Start instamatic with various functions (see below). If no arguments are given, start the instamatic GUI. The GUI is modular and can be defined using the config system. The GUI can be used to control the microscope and run the experiments. The GUI itself is further described on the GUI page.
 
 **Usage:**  
 ```bash
 instamatic [-h] [-s SCRIPT] [-n NAV_FILE] [-a] [-l LOCATE] [-o SHOW]
            [-i]
 ```
 **Optional arguments:**  
-`-h`, `--help`:  
-show this help message and exit  
-`-s SCRIPT`, `--script SCRIPT`:  
- Run the script given  
-`-n NAV_FILE`, `--nav NAV_FILE`:  
- Load the given .nav file  
-`-a`, `--acquire_at_items`:  
- Run the script file `--script` at every point marked with `Acquire` in the nav file `--nav`.  
-`-l LOCATE`, `--locate LOCATE`:  
- Locate a requested directory and exit, i.e. `config`, `data`, `scripts`, `base`, 'work`, `logs`  
-`-o SHOW`, `--open SHOW`:  
-Open the requested directory and exit, see `--locate`.  
-`-i`, `--info`:  
-Show info about the current instamatic installation.  
+
+`-h`, `--help`
+: Show this help message and exit  
+
+`-s SCRIPT`, `--script SCRIPT`
+:  Run the script given  
+
+`-n NAV_FILE`, `--nav NAV_FILE`
+:  Load the given .nav file  
+
+`-a`, `--acquire_at_items`
+:  Run the script file `--script` at every point marked with `Acquire` in the nav file `--nav`.  
+
+`-l LOCATE`, `--locate LOCATE`
+:  Locate a requested directory and exit, i.e. `config`, `data`, `scripts`, `base`, `work`, `logs`  
+
+`-o SHOW`, `--open SHOW`
+: Open the requested directory and exit, see `--locate`.  
+
+`-i`, `--info`
+: Show info about the current instamatic installation.  
 
 
 ## instamatic.controller
 
 Connect to the microscope and camera, and open an IPython terminal to interactively control the microscope. Useful for testing! It initializes the TEMController (accessible through the `ctrl` variable) using the parameters given in the `config`.
 
 **Usage:**  
 ```bash
 instamatic.controller [-h] [-u] [-c TEM_NAME] [-t CAM_NAME]
 ```
 **Optional arguments:**  
-`-h`, `--help`:  
-show this help message and exit  
-`-u`, `--simulate`:  
-Simulate microscope connection (default: False)  
-`-c TEM_NAME`, `--camera TEM_NAME`:  
- Camera configuration to load.  
-`-t CAM_NAME`, `--tem CAM_NAME`:  
- TEM configuration to load.  
+
+`-h`, `--help`
+: Show this help message and exit  
+
+`-u`, `--simulate`
+: Simulate microscope connection (default: False)  
+
+`-c TEM_NAME`, `--camera TEM_NAME`
+:  Camera configuration to load.  
+
+`-t CAM_NAME`, `--tem CAM_NAME`
+:  TEM configuration to load.  
 
 
 ## instamatic.serialed
 
 Command line program to run the serial ED data collection routine.
 
 **Usage:**  
 ```bash
 instamatic.serialed [-h]
 ```
 **Optional arguments:**  
-`-h`, `--help`:  
-show this help message and exit  
+
+`-h`, `--help`
+: Show this help message and exit  
 
 
 ## instamatic.camera
 
 Simple program to acquire image data from the camera.
 
 **Usage:**  
 ```bash
 instamatic.camera [-h] [-b N] [-e N] [-o image.png] [-d] [-s]
 ```
 **Optional arguments:**  
-`-h`, `--help`:  
-show this help message and exit  
-`-b N`, `--binsize N`:  
-Binsize to use. Must be one of 1, 2, or 4 (default 1)  
-`-e N`, `--exposure N`:  
-Exposure time (default 0.5)  
-`-o image.png`, `--out image.png`:  
- Where to store image  
-`-d`, `--display`:  
-Show the image (default True)  
-`-s`, `--series`:  
-Enable mode to take a series of images (default False)  
+
+`-h`, `--help`
+: Show this help message and exit  
+
+`-b N`, `--binsize N`
+: Binsize to use. Must be one of 1, 2, or 4 (default 1)  
+
+`-e N`, `--exposure N`
+: Exposure time (default 0.5)  
+
+`-o image.png`, `--out image.png`
+:  Where to store image  
+
+`-d`, `--display`
+: Show the image (default True)  
+
+`-s`, `--series`
+: Enable mode to take a series of images (default False)  
 
 
 ## instamatic.calibrate_stage_lowmag
 
 Program to calibrate the lowmag mode (100x) of the microscope (Deprecated).
 
 **Usage:**  
 ```bash
 instamatic.calibrate_stage_lowmag [-h] [IMG [IMG ...]]
 ```
 **Positional arguments:**  
-`IMG`:  
-Perform calibration using pre-collected images. The first image must be the center image used as the reference position. The other images are cross-correlated to this image to calibrate the translations. If no arguments are given, run the live calibration routine.  
+
+`IMG`
+: Perform calibration using pre-collected images. The first image must be the center image used as the reference position. The other images are cross-correlated to this image to calibrate the translations. If no arguments are given, run the live calibration routine.  
 
 **Optional arguments:**  
-`-h`, `--help`:  
-show this help message and exit  
+
+`-h`, `--help`
+: Show this help message and exit  
 
 
 ## instamatic.calibrate_stage_mag1
 
 Program to calibrate the mag1 mode of the microscope (Deprecated).
 
 **Usage:**  
 ```bash
 instamatic.calibrate_stage_mag1 [-h] [IMG [IMG ...]]
 ```
 **Positional arguments:**  
-`IMG`:  
-Perform calibration using pre-collected images. The first image must be the center image used as the reference position. The other images are cross-correlated to this image to calibrate the translations. If no arguments are given, run the live calibration routine.  
+
+`IMG`
+: Perform calibration using pre-collected images. The first image must be the center image used as the reference position. The other images are cross-correlated to this image to calibrate the translations. If no arguments are given, run the live calibration routine.  
 
 **Optional arguments:**  
-`-h`, `--help`:  
-show this help message and exit  
+
+`-h`, `--help`
+: Show this help message and exit  
 
 
 ## instamatic.calibrate_beamshift
 
 Program to calibrate the beamshift of the microscope (Deprecated).
 
 **Usage:**  
 ```bash
 instamatic.calibrate_beamshift [-h] [IMG [IMG ...]]
 ```
 **Positional arguments:**  
-`IMG`:  
-Perform calibration using pre-collected images. The first image must be the center image used as the reference position. The other images are cross-correlated to this image to calibrate the translations. If no arguments are given, run the live calibration routine.  
+
+`IMG`
+: Perform calibration using pre-collected images. The first image must be the center image used as the reference position. The other images are cross-correlated to this image to calibrate the translations. If no arguments are given, run the live calibration routine.  
 
 **Optional arguments:**  
-`-h`, `--help`:  
-show this help message and exit  
+
+`-h`, `--help`
+: Show this help message and exit  
 
 
 ## instamatic.calibrate_directbeam
 
 Program to calibrate the diffraction shift (PLA) to correct for beamshift movements (Deprecated).
 
 **Usage:**  
 ```bash
 instamatic.calibrate_directbeam [-h] [IMG [IMG ...]]
 ```
 **Positional arguments:**  
-`IMG`:  
-Perform calibration using pre-collected images. They must be formatted as such: DiffShift:pattern.tiff BeamShift:pattern.tiff, where `pattern` is a globbing pattern that finds the images corresponding to the key BeamShift or DiffShift. The first image must be the center image used as the reference position. The other images are cross-correlated to this image to calibrate the translations. If no arguments are given, run the live calibration routine.  
+
+`IMG`
+: Perform calibration using pre-collected images. They must be formatted as such: DiffShift:pattern.tiff BeamShift:pattern.tiff, where `pattern` is a globbing pattern that finds the images corresponding to the key BeamShift or DiffShift. The first image must be the center image used as the reference position. The other images are cross-correlated to this image to calibrate the translations. If no arguments are given, run the live calibration routine.  
 
 **Optional arguments:**  
-`-h`, `--help`:  
-show this help message and exit  
+
+`-h`, `--help`
+: Show this help message and exit  
 
 
 ## instamatic.calibrate_stagematrix
 
 Run the stagematrix calibration routine for all magnifications
 specified. Return the updates values for the configuration file.
 
@@ -198,32 +246,41 @@
 **Usage:**  
 ```bash
 instamatic.calibrate_stagematrix [-h] [-m MODE] [-k K [K ...]] [-A]
                                  [-v X] [-l STAGE_LENGTH] [-a N] [-b N]
                                  [-s]
 ```
 **Optional arguments:**  
-`-h`, `--help`:  
-show this help message and exit  
-`-m MODE`, `--mode MODE`:  
-Select the imaging mode (mag1/mag2/lowmag/samag). If `all` is specified, all imaging modes+mags are calibrated.If the imaging mode and magnification are not given, the currentvalues are used.  
-`-k K [K ...]`, `--mag K [K ...]`:  
- Select the imaging magnification(s).  
-`-A`, `--all_mags`:  
-Run calibration routine for all mags over selected mode.  
-`-v X`, `--overlap X`:  
-Specify the approximate overlap between images for cross correlation.  
-`-l STAGE_LENGTH`, `--stage_length STAGE_LENGTH`:  
- Specify the minimum length (in stage coordinates) the calibration should cover.  
-`-a N`, `--min_n_steps N`:  
- Specify the minimum number of steps to take along X and Y for the calibration.  
-`-b N`, `--max_n_steps N`:  
- Specify the maximum number of steps to take along X and Y for the calibration. This is used for higher magnifications.  
-`-s`, `--save`:  
-Save the data to the data directory [C:\instamatic].  
+
+`-h`, `--help`
+: Show this help message and exit  
+
+`-m MODE`, `--mode MODE`
+: Select the imaging mode (mag1/mag2/lowmag/samag). If `all` is specified, all imaging modes+mags are calibrated.If the imaging mode and magnification are not given, the currentvalues are used.  
+
+`-k K [K ...]`, `--mag K [K ...]`
+:  Select the imaging magnification(s).  
+
+`-A`, `--all_mags`
+: Run calibration routine for all mags over selected mode.  
+
+`-v X`, `--overlap X`
+: Specify the approximate overlap between images for cross correlation.  
+
+`-l STAGE_LENGTH`, `--stage_length STAGE_LENGTH`
+:  Specify the minimum length (in stage coordinates) the calibration should cover.  
+
+`-a N`, `--min_n_steps N`
+:  Specify the minimum number of steps to take along X and Y for the calibration.  
+
+`-b N`, `--max_n_steps N`
+:  Specify the maximum number of steps to take along X and Y for the calibration. This is used for higher magnifications.  
+
+`-s`, `--save`
+: Save the data to the data directory [C:\instamatic].  
 
 
 ## instamatic.flatfield
 
 This is a program that can collect and apply flatfield/darkfield corrections [link](https://en.wikipedia.org/wiki/Flat-field_correction). To do so, use a spread, bright beam on a hole in the carbon, or a clear piece of carbon film, and run:
 
     instamatic.flatfield --collect
@@ -237,45 +294,53 @@
 **Usage:**  
 ```bash
 instamatic.flatfield [-h] [-f flatfield.tiff] [-d darkfield.tiff]
                      [-o DRC] [-c]
                      [image.tiff [image.tiff ...]]
 ```
 **Positional arguments:**  
-`image.tiff`:  
-Image file paths/pattern  
+
+`image.tiff`
+: Image file paths/pattern  
 
 **Optional arguments:**  
-`-h`, `--help`:  
-show this help message and exit  
-`-f flatfield.tiff`, `--flatfield flatfield.tiff`:  
- Path to flatfield file  
-`-d darkfield.tiff`, `--darkfield darkfield.tiff`:  
- Path to darkfield file  
-`-o DRC`, `--output DRC`:  
-Output directory for image files  
-`-c`, `--collect`:  
-Collect flatfield/darkfield images on microscope  
+
+`-h`, `--help`
+: Show this help message and exit  
+
+`-f flatfield.tiff`, `--flatfield flatfield.tiff`
+:  Path to flatfield file  
+
+`-d darkfield.tiff`, `--darkfield darkfield.tiff`
+:  Path to darkfield file  
+
+`-o DRC`, `--output DRC`
+: Output directory for image files  
+
+`-c`, `--collect`
+: Collect flatfield/darkfield images on microscope  
 
 
 ## instamatic.stretch_correction
 
 Program to determine the stretch correction from a series of powder diffraction patterns (collected on a gold or aluminium powder). It will open a GUI to interactively identify the powder rings, and calculate the orientation (azimuth) and extent (amplitude) of the long axis compared to the short axis. These can be used in the `config` under `camera.stretch_azimuth` and `camera.stretch_percentage`.
 
 **Usage:**  
 ```bash
 instamatic.stretch_correction [-h] powder_pattern.tiff
 ```
 **Positional arguments:**  
-`powder_pattern.tiff`:  
-Diffraction pattern (TIFF) from a nanocrystalline powder showing Debye-Scherrer rings.  
+
+`powder_pattern.tiff`
+: Diffraction pattern (TIFF) from a nanocrystalline powder showing Debye-Scherrer rings.  
 
 **Optional arguments:**  
-`-h`, `--help`:  
-show this help message and exit  
+
+`-h`, `--help`
+: Show this help message and exit  
 
 
 ## instamatic.browser
 
 Program for browsing through electron diffraction images collected by `instamatic`.
 
 Example:
@@ -283,69 +348,77 @@
     instamatic.browser images/*.tiff -r results.csv
 
 **Usage:**  
 ```bash
 instamatic.browser [-h] [-s] [FILE]
 ```
 **Positional arguments:**  
-`FILE`:  
-File pattern to image files  
+
+`FILE`
+: File pattern to image files  
 
 **Optional arguments:**  
-`-h`, `--help`:  
-show this help message and exit  
-`-s`, `--stitch`:  
-Stitch images together.  
+
+`-h`, `--help`
+: Show this help message and exit  
+
+`-s`, `--stitch`
+: Stitch images together.  
 
 
 ## instamatic.viewer
 
 Simple image viewer to open any image collected collected using instamatic. Supported formats include `TIFF`, `MRC`, [`HDF5`](http://www.h5py.org/), and [`SMV`](https://strucbio.biologie.uni-konstanz.de/ccp4wiki/index.php/SMV_file_format).
 
 **Usage:**  
 ```bash
 instamatic.viewer [-h] IMG
 ```
 **Positional arguments:**  
-`IMG`:  
-Image to display (TIFF, HDF5, MRC, SMV).  
+
+`IMG`
+: Image to display (TIFF, HDF5, MRC, SMV).  
 
 **Optional arguments:**  
-`-h`, `--help`:  
-show this help message and exit  
+
+`-h`, `--help`
+: Show this help message and exit  
 
 
 ## instamatic.defocus_helper
 
 Tiny button to focus and defocus the diffraction pattern.
 
 **Usage:**  
 ```bash
 instamatic.defocus_helper [-h]
 ```
 **Optional arguments:**  
-`-h`, `--help`:  
-show this help message and exit  
+
+`-h`, `--help`
+: Show this help message and exit  
 
 
 ## instamatic.find_crystals
 
 Find crystals in images.
 
 **Usage:**  
 ```bash
 instamatic.find_crystals [-h] [IMG [IMG ...]]
 ```
 **Positional arguments:**  
-`IMG`:  
-Images to find crystals in.  
+
+`IMG`
+: Images to find crystals in.  
 
 **Optional arguments:**  
-`-h`, `--help`:  
-show this help message and exit  
+
+`-h`, `--help`
+: Show this help message and exit  
 
 
 ## instamatic.find_crystals_ilastik
 
 Find crystals in images using Ilastik.
 
 Takes a `.nav` file and `.mrc` file as input.
@@ -357,45 +430,54 @@
 **Usage:**  
 ```bash
 instamatic.find_crystals_ilastik [-h] [-n <path>] [-m <path>]
                                  [-c <name>] [-f D] [-d <path>]
                                  [--mapscaleind]
 ```
 **Optional arguments:**  
-`-h`, `--help`:  
-show this help message and exit  
-`-n <path>`, `--nav <path>`, `--nav_location <path>`:  
- The full path to the .nav file. Enter as raw string  
-`-m <path>`, `--mrc <path>`, `--mrc_location <path>`:  
- The full path to the .mrc file (not the global map). Enter as raw string  
-`-c <name>`, `--classifier <name>`:  
- Use the classifier as defined in /classifiers/classifiers.yaml  
-`-f D`, `--filter_dist D`, `--filter_distance D`:  
- Specify what distance the crystals should be separated  
-`-d <path>`, `--output <path>`, `--output_name <path>`:  
- The destination of the .nav file created  
-`--mapscaleind`:  
-Generate `MapScaleInd.yaml` for `predicrystal` from config.  
+
+`-h`, `--help`
+: Show this help message and exit  
+`-
+n <path>`, `--nav <path>`, `--nav_location <path>`
+  :  The full path to the .nav file. Enter as raw string  
+`-
+m <path>`, `--mrc <path>`, `--mrc_location <path>`
+  :  The full path to the .mrc file (not the global map). Enter as raw string  
+`-
+c <name>`, `--classifier <name>`
+  :  Use the classifier as defined in /classifiers/classifiers.yaml  
+
+`-f D`, `--filter_dist D`, `--filter_distance D`
+:  Specify what distance the crystals should be separated  
+`-
+d <path>`, `--output <path>`, `--output_name <path>`
+  :  The destination of the .nav file created  
+
+`--mapscaleind`
+: Generate `MapScaleInd.yaml` for `predicrystal` from config.  
 
 
 ## instamatic.learn
 
 Predict whether a crystal is of good or bad quality by its diffraction pattern.
 
 **Usage:**  
 ```bash
 instamatic.learn [-h] PAT
 ```
 **Positional arguments:**  
-`PAT`:  
-File pattern to glob for images (HDF5), i.e. `images/*.h5`.  
+
+`PAT`
+: File pattern to glob for images (HDF5), i.e. `images/*.h5`.  
 
 **Optional arguments:**  
-`-h`, `--help`:  
-show this help message and exit  
+
+`-h`, `--help`
+: Show this help message and exit  
 
 
 ## instamatic.temserver
 
 Connects to the TEM and starts a server for microscope communication. Opens a socket on port localhost:8088.
 
 This program initializes a connection to the TEM as defined in the config. On some setups it must be run in admin mode in order to establish a connection (on JEOL TEMs, wait for the beep!). The purpose of this program is to isolate the microscope connection in a separate process for improved stability of the interface in case instamatic crashes or is started and stopped frequently. For running the GUI, the temserver is required. Another reason is that it allows for remote connections from different PCs. The connection goes over a TCP socket.
@@ -411,18 +493,20 @@
 The response is returned as a serialized object.
 
 **Usage:**  
 ```bash
 instamatic.temserver [-h] [-t MICROSCOPE]
 ```
 **Optional arguments:**  
-`-h`, `--help`:  
-show this help message and exit  
-`-t MICROSCOPE`, `--microscope MICROSCOPE`:  
- Override microscope to use.  
+
+`-h`, `--help`
+: Show this help message and exit  
+
+`-t MICROSCOPE`, `--microscope MICROSCOPE`
+:  Override microscope to use.  
 
 
 ## instamatic.camserver
 
 Connects to the camera and starts a server for camera communication. Opens a socket on port localhost:8087.
 
 This program initializes a connection to the camera as defined in the config. This separates the communication from the main process and allows for remote connections from different PCs. The connection goes over a TCP socket.
@@ -438,18 +522,20 @@
 The response is returned as a pickle object.
 
 **Usage:**  
 ```bash
 instamatic.camserver [-h] [-c CAMERA]
 ```
 **Optional arguments:**  
-`-h`, `--help`:  
-show this help message and exit  
-`-c CAMERA`, `--camera CAMERA`:  
- Override camera to use.  
+
+`-h`, `--help`
+: Show this help message and exit  
+
+`-c CAMERA`, `--camera CAMERA`
+:  Override camera to use.  
 
 
 ## instamatic.dialsserver
 
 Starts a simple server to send indexing jobs to. Runs `-h` for every job sent to it. Opens a socket on port localhost:8089.
 
 The data sent to the server is a dict containing the following elements:
@@ -460,16 +546,17 @@
 - `osc`: Oscillation range in degrees (float)
 
 **Usage:**  
 ```bash
 instamatic.dialsserver [-h]
 ```
 **Optional arguments:**  
-`-h`, `--help`:  
-show this help message and exit  
+
+`-h`, `--help`
+: Show this help message and exit  
 
 
 ## instamatic.VMserver
 
 The script sets up socket connection between `instamatic` and `VirtualBox` software via `virtualbox` python API. Therefore, `VirtualBox` and the corresponding SDK need to be installed before running this command. This script is developed particularly for the possibility of running `XDS` under windows 7 or newer, a system which a lot of TEM computers may be using.
 
 After installation of VirtualBox and the corresponding SDK, `XDS` needs to be installed correctly in the guest Ubuntu system. In addition, a shared folder between `VirtualBox` and windows system needs to be set up properly in order for the server to work.
@@ -478,52 +565,59 @@
 
 **Usage:**  
 ```bash
 instamatic.VMserver [-h] [-shelxt] [-c a b c al be ga] [-s SPGR]
                     [-m Xn [Ym ...]]
 ```
 **Optional arguments:**  
-`-h`, `--help`:  
-show this help message and exit  
-`-shelxt`:  
-Run SHELXT when xds ASCII HKL file is generated.  
-`-c a b c al be ga`, `--unitcell a b c al be ga`:  
- Six numbers of the unit cell parameters.  
-`-s SPGR`, `--spgr SPGR`:  
-Space group.  
-`-m Xn [Ym ...]`, `--composition Xn [Ym ...]`:  
- Unit cell composition, i.e. `-m H2 O1`.  
+
+`-h`, `--help`
+: Show this help message and exit  
+
+`-shelxt`
+: Run SHELXT when xds ASCII HKL file is generated.  
+
+`-c a b c al be ga`, `--unitcell a b c al be ga`
+:  Six numbers of the unit cell parameters.  
+
+`-s SPGR`, `--spgr SPGR`
+: Space group.  
+
+`-m Xn [Ym ...]`, `--composition Xn [Ym ...]`
+:  Unit cell composition, i.e. `-m H2 O1`.  
 
 
 ## instamatic.xdsserver
 
 Starts a simple XDS server to send indexing jobs to. Runs XDS for every job sent to it. Opens a socket on port localhost:8089.
 
 The data sent to the server as a bytes string containing the data path (must contain `cRED_log.txt`).
 
 **Usage:**  
 ```bash
 instamatic.xdsserver [-h]
 ```
 **Optional arguments:**  
-`-h`, `--help`:  
-show this help message and exit  
+
+`-h`, `--help`
+: Show this help message and exit  
 
 
 ## instamatic.temserver_fei
 
-Utility script to enable rotation control from a dmscript. See [https://github.com/instamatic-dev/instamatic/tree/master/dmscript] for usage.
+Utility script to enable rotation control from a dmscript. See [https://github.com/instamatic-dev/InsteaDMatic] for usage.
 
 **Usage:**  
 ```bash
 instamatic.temserver_fei [-h]
 ```
 **Optional arguments:**  
-`-h`, `--help`:  
-show this help message and exit  
+
+`-h`, `--help`
+: Show this help message and exit  
 
 
 ## instamatic.goniotoolserver
 
 Connects to `Goniotool.exe` and starts a server for network communication. Opens a socket on port localhost:8090.
 
 The host and port are defined in `config/settings.yaml`.
@@ -537,32 +631,25 @@
 The response is returned as a pickle object.
 
 **Usage:**  
 ```bash
 instamatic.goniotoolserver [-h]
 ```
 **Optional arguments:**  
-`-h`, `--help`:  
-show this help message and exit  
+
+`-h`, `--help`
+: Show this help message and exit  
 
 
 ## instamatic.autoconfig
 
 This tool will help to set up the configuration files for `instamatic`.
 It establishes a connection to the microscope and reads out the camera lengths and magnification ranges.
 
 **Usage:**  
 ```bash
 instamatic.autoconfig [-h]
 ```
 **Optional arguments:**  
-`-h`, `--help`:  
-show this help message and exit  
-
-
-## instamatic.install
-
-This script sets up the paths for `instamatic`. It is necessary to run it at after first installation, and sometimes when the program is updated, or when the instamatic directory has moved.
-
-Usage:
 
-    instamatic.install
+`-h`, `--help`
+: Show this help message and exit
```

### Comparing `instamatic-1.9.0/docs/setup.md` & `instamatic-2.0.0/docs/setup.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,70 +1,72 @@
 # Setting up Instamatic
 
 Download the latest zip package from the [releases page](https://github.com/instamatic-dev/instamatic/releases). This installation is fully portable, and can be copied directly to the microscope computer.
 
-Running the program `start_Cmder` will run a terminal which has already been set up.
-
 ## JEOL
 
 If you are using a JEOL TEM, make sure `instamatic` is installed on a computer with the TEMCOM interface. This is usually already installed on the camera PC. It can also be installed on the microscope control PC.
 
 ## FEI
 
 For FEI microscopes, `instamatic` must be installed on the microscope control PC. Alternatively, it can be installed on both the microscope PC and the camera PC, running `instamatic.temserver` on the microscope PC, and establishing a connection over the local network. See the config documentation for how to set this up.
 
 ## Development version
 
-The latest, bleeding edge development version of `instamatic` is available from [here](https://github.com/instamatic-dev/instamatic/archive/master.zip).
-
-If you run the portable installation, just extract and replace the `instamatic` directory in the root directory of the installation (the one that contains `start_Cmder.exe`). Make sure to delete the old one before.
+The latest development version of `instamatic` is available from [here](https://github.com/instamatic-dev/instamatic/archive/main.zip).
 
 If you want to install `instamatic` into your own python installation, just extract and run:
 
 ```bash
-pip install -r requirements.txt
-python setup.py install
+pip install -e .
 ```
 
 ## Setting up the config files
 
 Normally `instamatic` is not very fussy about starting up, but it may complain if you try to run some commands where it is missing some information from the config.
 
-The easiest way to get started is to run:
-```bash
-instamatic.autoconfig.exe
-```
-To help generate some of the input files (in particular templates for the microscope/calibration files). This should give you a working setup for the microscope.
-
 In order of priority:
 
-1. __Initialize the config directory__  
-   If you are running the portable installation, you can skip this step. Otherwise, if you are running instamatic for the first time, it will set up the config directory. Simply run `instamatic`. It should say that it sets up the config directory and tell the path where the data are.
+### __1. Initialize the config directory__  
+   If you are running instamatic for the first time, it will set up the config directory. Simply run `instamatic`. It should say that it sets up the config directory and tell the path where the data are.
+
+### __2. Set up the microscope interface__  
+   Go to the config directory from the first step.
 
-2. __Set up the microscope interface__  
    In `config/settings.yaml` define the camera interface you want to use. You can use the autoconfig tool or one of the example files and modify those. You can name these files anything you want, as long as the name under `microscope` matches the filename in `config/microscope`
 
-3. __Set up the magnifications and camera lengths__  
-   In the config file, i.e `config/microscope/jeol.yaml`, set the correct camera lengths (`range_diff`) and magnifications for your microscopes (`range_lowmag` and `range_mag1`). Also make sure you set the wavelength. Again, the autoconfig tool is your best friend, otherwise, the way to get those numbers is to simply write them down as you turn the magnification knob on the microcope.
+### __3. Set up the magnifications and camera lengths__  
+   In the config file, i.e `config/microscope/jeol.yaml`, set the correct camera lengths (`ranges/diff`) and magnifications for your microscopes (`ranges/lowmag` and `ranges/mag1`). Also make sure you set the wavelength. Again, the autoconfig tool is your best friend, otherwise, the way to get those numbers is to simply write them down as you turn the magnification knob on the microcope.
 
-4. __Set up the camera interface__  
+### __4. Set up the camera interface__  
    Specify the file you want to use for the camera interface, i.e. `camera: timepix` points to `config/camera/timepix.yaml`. In this file, make sure that the interface is set to your camera type and update the numbers as specified in the config documentation. If you do not want to set up the camera interface at this moment, you can use `camera: simulate` to fake the camera connection.
 
-5. __Make the calibration table__  
+### __5. Make the calibration table__  
    For each of the magnfications defined in `config/microscope/jeol.yaml`, specify the pixel sizes in the file defined by `calibration: jeol`, corresponding to the file `calibration/jeol.yaml`. For starters, you can simply set the calibration values to 1.0.
 
-6. __Test if it works__  
+### __6. Test if it works__  
    Run `instamatic.temcontroller` to start a IPython shell that initializes the connection. It should run with no crashes or warnings.
 
-7. __Update `settings.yaml`__  
+### __7. Update `settings.yaml`__  
    There are a few more choices to make in `instamatic/settings.yaml`. If you use a TVIPS camera, make sure you put `use_cam_server: true`.
 
-It is often a good idea to run the camserver and temserver in a different terminal window by running `instamatic.temserver` / `instamatic.camserver` if you specified this in `settings.yaml`.
 
-## Other directories
+It is recommended to run the temserver in a different terminal window by running `instamatic.temserver` if you specified this in `settings.yaml`. This helps maintain the microscope connection in case you want to restart instamatic. In some cases it is also worth to do this for the camera (or necessary in case of TVIPS) using `instamatic.camserver`.
+
+## Automatic config generation
+
+The easiest way to get started is to run:
+
+```bash
+instamatic.autoconfig.exe
+```
+
+To help generate some of the input files (in particular templates for the microscope/calibration files). This should give you a working setup for the microscope.
+
+## Installing the Gatan CCD plugin
+
+To work with the gatan camera, instamatic needs a plugin for GMS.
+For this, instamatic depends on the RED CCD Plugin. You can download it [here](https://zenodo.org/record/2545322).
+
+The plugin can be found in the package `REDc.rar`, in `.\CCD_plugins\Gatan\Normal Gatan cameras\REDCCDPlugin`.
 
-- `cmder`: Contains the [Cmder](https://cmder.net/) software package. The file `cmder\config\user-profile.ps1` can be used to set up the environment variables, and extra programs can go into `cmder\bin`.
-- `config`: Contains all the config files for instamatic
-- `instamatic`: Source code for `instamatic`. Replace this directory if you want to update `instamatic`.
-- `logs`: Log files from `instamatic` are stored here.
-- `python36`: This contains the portable [python](https://www.python.org/) installation and libraries
-- `scripts`: The instamatic GUI picks up scripts from this directory.
+Place `REDCCDPlugin.dll` in your Gatan plugin directory, which can usually be found here: `C:\Program files\Gatan\DigitalMicrgraph\Plugins`. For more information, have a look at the RED installation instructions manual.
```

### Comparing `instamatic-1.9.0/docs/tem_api.md` & `instamatic-2.0.0/docs/tem_api.md`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 ```python
 ctrl = TEMController.initialize(tem_name='jeol', cam_name=None)
 ```
 
 Once a `ctrl` (control) object has been initialized, it becomes possible to play around with the lenses and stage interactively. Type `ctrl.` and hit `tab` to see the autocomplete options. Or write use `?` to request the doc string for a function (e.g. `TEMController.initialize?`).
 
-Based on this you can write your own python scripts to control the microscope and/or camera. See in `instamatic/instamatic/experiments/cred/experiment.py` for an idea how this is used. All the microscope control interface can be found in `instamatic/TEMController/`
+Based on this you can write your own python scripts to control the microscope and/or camera. See in `src/instamatic/experiments/cred/experiment.py` for an idea how this is used. All the microscope control interface can be found in `src/instamatic/TEMController/`
 
 The `ctrl` object allows full control over the electron microscope. For example, to read out the position of the sample stage:
 ```python
 xy = ctrl.stage.xy
 print(xy)
 ```
 To move to a different position:
```

### Comparing `instamatic-1.9.0/docs/tvips.md` & `instamatic-2.0.0/docs/tvips.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-## cRED data collection with TVIPS
+# TVIPS cRED
 
 Module: `cred_tvips`
 
 This module can be used for cRED/SerialRED data collection using a TVIPS camera. It can be enabled by adding the `cred_tvips` module to the `modules` section in the [settings](config.md).
 
 `Instamatic` communicates with EMMENU to start and stop image acquisition. EMMENU must be running before `instamatic` is started. In EMMENU the correct camera profile should be selected (one with shutterless acquisition) before data collection is started. A navigator (`.nav`) file can be given to enable serial data collection on a large number of crystals.
 
@@ -10,83 +10,83 @@
 
 The python script [process_tvips.py](../scripts/process_tvips.py) can be used to convert the data to MRC or SMV format, with input files for [REDp](https://zenodo.org/record/2545322) (.ed3d) and [XDS](http://xds.mpimf-heidelberg.mpg.de/) (XDS.INP).
 
 Data collection was tested and developed on a JEOL 1400 with F416 camera.
 
 ![TVIPS ED data collection pane](images/gui_tvips_annotated.png)
 
-#### 1. Console window
+## 1. Console window
 
 Shows the program output, see: [Console](gui.md#console).
 
-#### 2. Input/output
+## 2. Input/output
 
 Contronls where the data are stored. For more information, see: [Data i/o](gui.md#Data-io).
 
 
-#### 3. Experimental parameters
+## 3. Experimental parameters
 
-**Target angle**  
-The angle the goniometer should rotate to starting from the current angle. Pressing **invert** willl invert the angle (*i.e.* 40° to -40°).
+Target angle
+: The angle the goniometer should rotate to starting from the current angle. Pressing <kbd>invert</kbd> will invert the angle (*i.e.* 40° to -40°).
 
-If you check **Manual rotation control**, the target angle will be blanked and instead the rotation is controlled manually (*e.g.* via the panel or foot controls). `Instamatic` will then automatically terminate the experiment once it notices that rotation has stopped.
+: If you check <kbd>Manual rotation control</kbd>, the target angle will be blanked and instead the rotation is controlled manually (*e.g.* via the panel or foot controls). `Instamatic` will then automatically terminate the experiment once it notices that rotation has stopped.
 
-**Diff defocus**  
-This is the defocus value to apply to the diffraction focus. This is used to quickly toggle to a *view* of the crystal without toggling the mode, which may introduce not refocus to the same position because of lens hysteresis. Check the **Toggle diff defocus** box to toggle between the focused/defocused mode. Pressing **Reset** will return to the original value.
+Diff defocus
+: This is the defocus value to apply to the diffraction focus. This is used to quickly toggle to a *view* of the crystal without toggling the mode, which may introduce not refocus to the same position because of lens hysteresis. Check the <kbd>Toggle diff defocus</kbd> box to toggle between the focused/defocused mode. Pressing <kbd>Reset</kbd> will return to the original value.
 
-**Exposure**  
-The exposure time for each frame in milliseconds. Ideally, this should be set so that a single frame covers ~0.2-0.3°, but the added overhead from the camera should also be taken into account.
+Exposure
+: The exposure time for each frame in milliseconds. Ideally, this should be set so that a single frame covers ~0.2-0.3°, but the added overhead from the camera should also be taken into account.
 
-**Mode**  
-Select the mode to collect data in, *e.g.* to do continuous real space tomography.
+Mode
+: Select the mode to collect data in, *e.g.* to do continuous real space tomography.
 
-#### 4. Start/stop the experiment
+## 4. Start/stop the experiment
 
-These are the controls to collect a cRED data set from a single particle. To prepare the TEM for acquisition, press **Get Ready**. This will move to the right angle, turn off the beam blank, start the live view in EMMENU, etc. There will be a message once the TEM is ready.
+These are the controls to collect a cRED data set from a single particle. To prepare the TEM for acquisition, press <kbd>Get Ready</kbd>. This will move to the right angle, turn off the beam blank, start the live view in EMMENU, etc. There will be a message once the TEM is ready.
 
-Press **Acquire** to start the acquisition. The TEM will rotate to the specified angle, and automatically stop once finished. Pressing **Finalize** will unlock the interface so a new experiment can be started.
+Press <kbd>Acquire</kbd> to start the acquisition. The TEM will rotate to the specified angle, and automatically stop once finished. Pressing <kbd>Finalize</kbd> will unlock the interface so a new experiment can be started.
 
-#### 5. Start serial acquisition
+## 5. Start serial acquisition
 
 This button starts a serial acquisition using the instruction file given below. Once started, it can only be interrupted by pressing `Ctrl-C` in the terminal.
 
 The instruction file must be a `.nav` file compatible with [SerialEM](https://bio3d.colorado.edu/SerialEM/).
 
 Data will be collected at every position with the `Acquire` flag set.
 
-#### 6. Other controls
+## 6. Other controls
 
-**Toggle DIFF**  
-Toggles between diffraction (DIFF) and mag (MAG1) mode.
+Toggle DIFF
+: Toggles between diffraction (DIFF) and mag (MAG1) mode.
 
-**Toggle screen**  
-Moves the fluorescent screen up/down.
+Toggle screen
+: Moves the fluorescent screen up/down.
 
-**Toggle beamblank**  
-Toggle the beam blank. If the beam is blanked when the experiment is started, it will automatically unblank and re-blank afterwards.
+Toggle beamblank
+: Toggle the beam blank. If the beam is blanked when the experiment is started, it will automatically unblank and re-blank afterwards.
 
-**Start live view**  
-Start the live view in EMMENU.
+Start live view
+: Start the live view in EMMENU.
 
-**Stop live view**  
-Stop the live view in EMMENU.
+Stop live view
+: Stop the live view in EMMENU.
 
-**Search**  
-Switch the microscope to search mode. Internally, these are defined as [`instamatic` scripts](https://github.com/instamatic-dev/instamatic/tree/master/instamatic/config/scripts) and can therefore be easily modified. The parameters of the search mode are defined in `$instamatic\scripts\search_mode.py`, for example to put the screen down, unblank the beam, and switch to MAG1 mode:
+Search
+: Switch the microscope to search mode. Internally, these are defined as [`instamatic` scripts](https://github.com/instamatic-dev/instamatic/tree/main/src/instamatic/config/scripts) and can therefore be easily modified. The parameters of the search mode are defined in `$instamatic\scripts\search_mode.py`, for example to put the screen down, unblank the beam, and switch to MAG1 mode:
 
 ```python
 ctrl.screen.down()
 ctrl.beam.unblank()
 ctrl.mode.set('mag1')
 ```
 
-**Focus**  
-Switch the microscope to focus mode. The parameters of the search mode are defined in `$instamatic\scripts\focus_mode.py`, for example to put the screen up, blank the beam, and switch to DIFF mode:
+Focus
+: Switch the microscope to focus mode. The parameters of the search mode are defined in `$instamatic\scripts\focus_mode.py`, for example to put the screen up, blank the beam, and switch to DIFF mode:
 
 ```python
 ctrl.screen.up()
 ctrl.beam.blank()
 ctrl.mode.set('diff')
 ```
 
-**Get Image**  
-Acquire and store a single image. It will be available in the EMMENU image buffer.
+Get Image
+: Acquire and store a single image. It will be available in the EMMENU image buffer.
```

### Comparing `instamatic-1.9.0/instamatic/TEMController/TEMController.py` & `instamatic-2.0.0/src/instamatic/TEMController/TEMController.py`

 * *Files 3% similar despite different names*

```diff
@@ -267,15 +267,15 @@
             Affine transformation matrix to convert from stage to pixel coordinates
         """
         if not mode:
             mode = self.mode.get()
         if not mag:
             mag = self.magnification.value
         if not binning:
-            binning = self.cam.getBinning()
+            binning = self.cam.get_binning()
 
         stagematrix = config.calibration[mode]['stagematrix'][mag]
         stagematrix = np.array(stagematrix).reshape(2, 2) * binning  # um -> nm
 
         return stagematrix
 
     def align_to(self,
@@ -516,15 +516,15 @@
             Image binning.
 
         Returns
         -------
         arr : np.array
             Image as 2D numpy array.
         """
-        return self.cam.getImage(exposure=exposure, binsize=binsize)
+        return self.cam.get_image(exposure=exposure, binsize=binsize)
 
     def get_future_image(self, exposure: float = None, binsize: int = None) -> 'future':
         """Simplified function equivalent to `get_image` that returns the raw
         image as a future. This makes the data acquisition call non-blocking.
 
         Parameters
         ----------
@@ -641,29 +641,74 @@
         h['ImageExposureTime'] = exposure
         h['ImageBinsize'] = binsize
         h['ImageResolution'] = arr.shape
         # k['ImagePixelsize'] = config.calibration[mode]['pixelsize'][mag] * binsize
         # k['ImageRotation'] = config.calibration[mode]['rotation'][mag]
         h['ImageComment'] = comment
         h['ImageCameraName'] = self.cam.name
-        h['ImageCameraDimensions'] = self.cam.getCameraDimensions()
+        h['ImageCameraDimensions'] = self.cam.get_camera_dimensions()
 
         if verbose:
             print(f'Image acquired - shape: {arr.shape}, size: {arr.nbytes / 1024:.0f} kB')
 
         if out:
             write_tiff(out, arr, header=h)
 
         if plot:
             import matplotlib.pyplot as plt
             plt.imshow(arr)
             plt.show()
 
         return arr, h
 
+    def get_movie(self,
+                  n_frames: int,
+                  *,
+                  exposure: float = None,
+                  binsize: int = None,
+                  out: str = None) -> Tuple[np.ndarray]:
+        """Collect a stack of images using the camera's movie mode, if
+        available.
+
+        This minimizes the gap between frames.
+
+        Parameters
+        ----------
+        n_frames : int
+            Number of frames to collect
+        exposure : float, optional
+            Exposure time in seconds
+        binsize : int, optional
+            Binning to use for the image, must be 1, 2, or 4, etc
+        out : str, optional
+            Path or filename to which the image/header is saved (defaults to tiff)
+
+        Returns
+        -------
+        stack : Tuple[np.ndarray]
+            List of numpy arrays with image data.
+        """
+        if not self.cam:
+            raise AttributeError(f"{self.__class__.__name__} object has no attribute 'cam' (Camera has not been initialized)")
+
+        if not binsize:
+            binsize = self.cam.default_binsize
+        if not exposure:
+            exposure = self.cam.default_exposure
+
+        if self.autoblank:
+            self.beam.unblank()
+
+        stack = self.cam.get_movie(n_frames=n_frames, exposure=exposure, binsize=binsize)
+
+        if self.autoblank:
+            self.beam.blank()
+
+        return stack
+
     def store_diff_beam(self, name: str = 'beam', save_to_file: bool = False):
         """Record alignment for current diffraction beam. Stores Guntilt (for
         dose control), diffraction focus, spot size, brightness, and the
         function mode.
 
         Restore the alignment using:     `ctrl.restore("beam")`
         """
@@ -720,19 +765,19 @@
         formatter_class=argparse.RawDescriptionHelpFormatter)
 
     parser.add_argument('-u', '--simulate',
                         action='store_true', dest='simulate',
                         help='Simulate microscope connection (default: False)')
 
     parser.add_argument('-c', '--camera',
-                        action='store', type=str, dest='tem_name',
+                        action='store', type=str, dest='cam_name',
                         help='Camera configuration to load.')
 
     parser.add_argument('-t', '--tem',
-                        action='store', type=str, dest='cam_name',
+                        action='store', type=str, dest='tem_name',
                         help='TEM configuration to load.')
 
     parser.set_defaults(
         simulate=False,
         tem_name=default_tem,
         cam_name=default_cam,
     )
```

### Comparing `instamatic-1.9.0/instamatic/TEMController/deflectors.py` & `instamatic-2.0.0/src/instamatic/TEMController/deflectors.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,66 +1,76 @@
 from collections import namedtuple
 from typing import Tuple
 
 DeflectorTuple = namedtuple('DeflectorTuple', ['x', 'y'])
 
 
 class Deflector:
-    """Generic microscope deflector object defined by X/Y values Must be
-    subclassed to set the self._getter, self._setter functions."""
+    """Generic microscope deflector object defined by X/Y values.
+
+    Must be subclassed to set the `self._getter`, `self._setter`
+    functions.
+    """
 
     def __init__(self, tem):
         super().__init__()
         self._tem = tem
         self._getter = None
         self._setter = None
         self.key = 'def'
 
     def __repr__(self):
         x, y = self.get()
         return f'{self.name}(x={x}, y={y})'
 
     @property
     def name(self) -> str:
+        """Return name of the deflector."""
         return self.__class__.__name__
 
     def set(self, x: int, y: int):
+        """Set the X and Y values of the deflector."""
         self._setter(x, y)
 
     def get(self) -> Tuple[int, int]:
+        """Get X and Y values of the deflector."""
         return DeflectorTuple(*self._getter())
 
     @property
     def x(self) -> int:
+        """Get/set X value."""
         x, y = self.get()
         return x
 
     @x.setter
     def x(self, value: int):
         self.set(value, self.y)
 
     @property
     def y(self) -> int:
+        """Get/set Y value."""
         x, y = self.get()
         return y
 
     @y.setter
     def y(self, value: int):
         self.set(self.x, value)
 
     @property
     def xy(self) -> Tuple[int, int]:
+        """Get/set x and y values as a tuple."""
         return self.get()
 
     @xy.setter
     def xy(self, values: Tuple[int, int]):
         x, y = values
         self.set(x=x, y=y)
 
     def neutral(self):
+        """Return deflector to stored neutral values."""
         self._tem.setNeutral(self.key)
 
 
 class GunShift(Deflector):
     """GunShift control."""
 
     def __init__(self, tem):
```

### Comparing `instamatic-1.9.0/instamatic/TEMController/fei_microscope.py` & `instamatic-2.0.0/src/instamatic/TEMController/fei_microscope.py`

 * *Files 17% similar despite different names*

```diff
@@ -24,103 +24,29 @@
 # 0.10: 2.91
 # 0.05: 1.48
 # 0.04: 1.18
 # 0.03: 0.888
 # 0.02: 0.593
 # 0.01: 0.297
 
-
 FUNCTION_MODES = {0: 'LM', 1: 'Mi', 2: 'SA', 3: 'Mh', 4: 'LAD', 5: 'D'}
 
-MagnificationMapping = {
-    1: 45,
-    2: 58,
-    3: 73,
-    4: 89,
-    5: 115,
-    6: 145,
-    7: 185,
-    8: 235,
-    9: 300,
-    10: 380,
-    11: 470,
-    12: 600,
-    13: 760,
-    14: 950,
-    15: 1200,
-    16: 1550,
-    17: 3400,
-    18: 4400,
-    19: 5600,
-    20: 7200,
-    21: 8800,
-    22: 11500,
-    23: 14500,
-    24: 18500,
-    25: 24000,
-    26: 30000,
-    27: 38000,
-    28: 49000,
-    29: 61000,
-    30: 77000,
-    31: 100000,
-    32: 130000,
-    33: 165000,
-    34: 215000,
-    35: 265000,
-    36: 340000,
-    37: 430000,
-    38: 550000,
-    39: 700000,
-    40: 890000,
-    41: 1150000,
-    42: 1250000,
-    43: 960000,
-    44: 750000,
-    45: 600000,
-    46: 470000,
-    47: 360000,
-    48: 285000,
-    49: 225000,
-    50: 175000,
-    51: 145000,
-    52: 115000,
-    53: 89000,
-    54: 66000,
-    55: 52000,
-    56: 41000,
-    57: 32000,
-    58: 26000,
-    59: 21000,
-    60: 8300,
-    61: 6200,
-    62: 3100}
-
-CameraLengthMapping = {
-    1: 34,
-    2: 42,
-    3: 53,
-    4: 68,
-    5: 90,
-    6: 115,
-    7: 140,
-    8: 175,
-    9: 215,
-    10: 265,
-    11: 330,
-    12: 420,
-    13: 530,
-    14: 680,
-    15: 830,
-    16: 1050,
-    17: 1350,
-    18: 1700,
-    19: 2100,
-    20: 2700,
-    21: 3700}
+
+def get_magnification_mapping():
+    functions = ('LM', 'Mi', 'SA', 'Mh')
+    values = (val for function in functions for val in config.microscope.ranges[function])
+    return {num + 1: val for num, val in enumerate(values)}
+
+
+def get_camera_length_mapping():
+    return {num + 1: val for num, val in enumerate(config.microscope.ranges['D'])}
+
+
+MagnificationMapping = get_magnification_mapping()
+CameraLengthMapping = get_camera_length_mapping()
 
 
 class FEIMicroscope:
     """Python bindings to the FEI microscope using the COM interface."""
 
     def __init__(self, name='fei'):
         super().__init__()
@@ -152,15 +78,15 @@
             t += 1
             if t > 3:
                 print(f'Waiting for microscope, t = {t}s')
             if t > 30:
                 raise TEMCommunicationError('Cannot establish microscope connection (timeout).')
 
         logger.info('Microscope connection established')
-        atexit.register(self.releaseConnection)
+        atexit.register(self.release_connection)
 
         self.name = name
         self.FUNCTION_MODES = FUNCTION_MODES
 
         self.FunctionMode_value = 0
 
         self.goniostopped = self.stage.Status
@@ -184,15 +110,15 @@
             ind = self.proj.MagnificationIndex
             return MagnificationMapping[ind]
         else:
             ind = self.proj.CameraLengthIndex
             return CameraLengthMapping[ind]
 
     def setMagnification(self, value):
-        """value has to be the index."""
+        """Value has to be the index."""
         if self.tom.Projection.Mode != 1:
             ind = [key for key, v in MagnificationMapping.items() if v == value][0]
             try:
                 self.proj.MagnificationIndex = ind
             except ValueError:
                 pass
         else:
@@ -209,19 +135,19 @@
 
         self.tom.Stage.Speed = value
 
     def getStageSpeed(self):
         return self.tom.Stage.Speed
 
     def getStagePosition(self):
-        """return numbers in microns, angles in degs."""
+        """Return numbers in microns, angles in degs."""
         return self.stage.Position.X * 1e6, self.stage.Position.Y * 1e6, self.stage.Position.Z * 1e6, self.stage.Position.A / pi * 180, self.stage.Position.B / pi * 180
 
     def setStagePosition(self, x=None, y=None, z=None, a=None, b=None, wait=True, speed=1):
-        """x, y, z in the system are in unit of meters, angles in radians."""
+        """X, y, z in the system are in unit of meters, angles in radians."""
         pos = self.stage.Position
         axis = 0
 
         if speed > 1 or speed < 0:
             raise FEIValueError(f'setStageSpeed value must be between 0 and 1. Input: {speed}')
 
         self.tom.Stage.Speed = speed
@@ -259,15 +185,15 @@
 
     def getGunShift(self):
         x = self.tem.GUN.Shift.X
         y = self.tem.GUN.Shift.Y
         return x, y
 
     def setGunShift(self, x, y):
-        """x y can only be float numbers between -1 and 1."""
+        """X y can only be float numbers between -1 and 1."""
         gs = self.tem.GUN.Shift
         if abs(x) > 1 or abs(y) > 1:
             raise FEIValueError(f'GunShift x/y must be a floating number between -1 an 1. Input: x={x}, y={y}')
 
         if x is not None:
             gs.X = x
         if y is not None:
@@ -327,21 +253,21 @@
         if x is not None:
             bs.X = x
         if y is not None:
             bs.Y = y
         self.tom.Illumination.BeamAlignShift = bs
 
     def getBeamTilt(self):
-        """rotation center in FEI."""
+        """Rotation center in FEI."""
         x = self.tom.Illumination.BeamAlignmentTilt.X
         y = self.tom.Illumination.BeamAlignmentTilt.Y
         return x, y
 
     def setBeamTilt(self, x, y):
-        """rotation center in FEI."""
+        """Rotation center in FEI."""
         bt = self.tom.Illumination.BeamAlignmentTilt
 
         if x is not None:
             if abs(x) > 1:
                 raise FEIValueError(f'BeamTilt x must be a floating number between -1 an 1. Input: x={x}')
             bt.X = x
         if y is not None:
@@ -369,15 +295,15 @@
     def getImageShift2(self):
         return 0, 0
 
     def setImageShift2(self, x, y):
         return 0
 
     def getImageBeamShift(self):
-        """image-beam shift."""
+        """Image-beam shift."""
         return self.tom.Projection.ImageBeamShift.X, self.tom.Projection.ImageBeamShift.Y
 
     def setImageBeamShift(self, x, y):
         is1 = self.tom.Projection.ImageBeamShift
         if abs(x) > 1 or abs(y) > 1:
             print('Invalid gunshift setting: can only be float numbers between -1 and 1.')
             return
@@ -418,15 +344,15 @@
 
     """What is the relationship between defocus and focus?? Both are changing the defoc value"""
 
     def getDiffFocus(self):
         return self.tom.Projection.Defocus
 
     def setDiffFocus(self, value):
-        """defocus value in unit m."""
+        """Defocus value in unit m."""
         self.tom.Projection.Defocus = value
 
     def getFocus(self):
         return self.tom.Projection.Focus
 
     def setFocus(self, value):
         self.tom.Projection.Focus = value
@@ -439,26 +365,30 @@
         else:
             raise FEIValueError("aperture must be specified as 'C1' or 'C2'.")
 
     def getDarkFieldTilt(self):
         return self.tom.Illumination.DarkfieldTilt.X, self.tom.Illumination.DarkfieldTilt.Y
 
     def setDarkFieldTilt(self, x, y):
-        """does not set."""
+        """Does not set."""
         return 0
 
     def getScreenCurrent(self):
-        """return screen current in nA."""
+        """Return screen current in nA."""
         return self.tom.Screen.Current * 1e9
 
     def isfocusscreenin(self):
         return self.tom.Screen.IsFocusScreenIn
 
     def getDiffShift(self):
-        """user diff shift, encoded in a different way than system status on TEM USER INTERFACE: 180/pi*number = number on TEM USER INTERFACE. Not exactly though, close enough"""
+        """User diff shift, encoded in a different way than system status on
+        TEM USER INTERFACE: 180/pi*number = number on TEM USER INTERFACE.
+
+        Not exactly though, close enough
+        """
         return 180 / pi * self.tem.Projection.DiffractionShift.X, 180 / pi * self.tem.Projection.DiffractionShift.Y
 
     def setDiffShift(self, x, y):
         ds1 = self.tem.Projection.DiffractionShift
         if abs(x) > 1 or abs(y) > 1:
             print('Invalid gunshift setting: can only be float numbers between -1 and 1.')
             return
@@ -466,21 +396,21 @@
         if x is not None:
             ds1.X = x / 180 * pi
         if y is not None:
             ds1.Y = y / 180 * pi
 
         self.tem.Projection.DiffractionShift = ds1
 
-    def releaseConnection(self):
+    def release_connection(self):
         comtypes.CoUninitialize()
         logger.info('Connection to microscope released')
         print('Connection to microscope released')
 
     def isBeamBlanked(self):
-        """to be tested."""
+        """To be tested."""
         return self.tem.Illumination.BeamBlanked
 
     def setBeamBlank(self, value):
         """True/False or 1/0."""
         self.tem.Illumination.BeamBlanked = value
 
     def setBeamUnblank(self):
@@ -490,15 +420,15 @@
         return self.tom.Illumination.CondenserStigmator.X, self.tom.Illumination.CondenserStigmator.Y
 
     def setCondensorLensStigmator(self, x, y):
         self.tom.Illumination.CondenserStigmator.X = x
         self.tom.Illumination.CondenserStigmator.Y = y
 
     def getIntermediateLensStigmator(self):
-        """diffraction stigmator."""
+        """Diffraction stigmator."""
         return self.tom.Illumination.DiffractionStigmator.X, self.tom.Illumination.DiffractionStigmator.Y
 
     def setIntermediateLensStigmator(self, x, y):
         self.tom.Illumination.DiffractionStigmator.X = x
         self.tom.Illumination.DiffractionStigmator.Y = y
 
     def getObjectiveLensStigmator(self):
@@ -529,12 +459,12 @@
     def setMagnificationIndex(self, index):
         if self.tom.Projection.Mode != 1:
             self.proj.MagnificationIndex = index
         else:
             self.proj.CameraLengthIndex = index
 
     def getBrightness(self):
-        """return diameter in microns."""
+        """Return diameter in microns."""
         return self.tom.Illumination.IlluminatedAreaDiameter * 1e6
 
     def setBrightness(self, value):
         self.tom.Illumination.IlluminatedAreaDiameter = value * 1e-6
```

### Comparing `instamatic-1.9.0/instamatic/TEMController/fei_simu_microscope.py` & `instamatic-2.0.0/src/instamatic/TEMController/fei_simu_microscope.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
             t += 1
             if t > 3:
                 print(f'Waiting for microscope, t = {t}s')
             if t > 30:
                 raise TEMCommunicationError('Cannot establish microscope connection (timeout).')
 
         logger.info('Microscope connection established')
-        atexit.register(self.releaseConnection)
+        atexit.register(self.release_connection)
 
         self.name = name
         self.FUNCTION_MODES = FUNCTION_MODES
 
         self.FunctionMode_value = 0
 
         self.DiffractionFocus_value = random.randint(MIN, MAX)
@@ -282,15 +282,15 @@
     def getDiffShift(self):
         return self.DiffractionShift_x, self.DiffractionShift_y
 
     def setDiffShift(self, x, y):
         self.DiffractionShift_x = x
         self.DiffractionShift_y = y
 
-    def releaseConnection(self):
+    def release_connection(self):
         comtypes.CoUninitialize()
         logger.info('Connection to microscope released')
         print('Connection to microscope released')
 
     def isBeamBlanked(self, value):
         return self.beamblank
 
@@ -302,15 +302,15 @@
         return self.tom.Illumination.CondenserStigmator.X, self.tom.Illumination.CondenserStigmator.Y
 
     def setCondensorLensStigmator(self, x, y):
         self.tom.Illumination.CondenserStigmator.X = x
         self.tom.Illumination.CondenserStigmator.Y = y
 
     def getIntermediateLensStigmator(self):
-        """diffraction stigmator."""
+        """Diffraction stigmator."""
         return self.tom.Illumination.DiffractionStigmator.X, self.tom.Illumination.DiffractionStigmator.Y
 
     def setIntermediateLensStigmator(self, x, y):
         self.tom.Illumination.DiffractionStigmator.X = x
         self.tom.Illumination.DiffractionStigmator.Y = y
 
     def getObjectiveLensStigmator(self):
@@ -328,15 +328,15 @@
         self.tom.Illumination.SpotsizeIndex = value
 
     def getScreenPosition(self):
         # TO BE CHECKED: does FEI tem have a screenposition object??
         return self.screenposition_value
 
     def setScreenPosition(self, value):
-        """value = 'up' or 'down'"""
+        """Value = 'up' or 'down'."""
         self.screenposition_value = value
 
     def getCondensorLens1(self):
         return self.condensorlens1_value
 
     def getCondensorLens2(self):
         return self.condensorlens2_value
```

### Comparing `instamatic-1.9.0/instamatic/TEMController/jeol_microscope.py` & `instamatic-2.0.0/src/instamatic/TEMController/jeol_microscope.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
             t += 1
             if t > 3:
                 print(f'Waiting for microscope, t = {t}s')
             if t > 30:
                 raise TEMCommunicationError('Cannot establish microscope connection (timeout).')
 
         logger.info('Microscope connection established')
-        atexit.register(self.releaseConnection)
+        atexit.register(self.release_connection)
 
         self._x_direction = 0
         self._y_direction = 0
 
         self.name = name
 
         self.FUNCTION_MODES = FUNCTION_MODES
@@ -272,15 +272,15 @@
         x, y, result = self.def3.GetIS2()
         return x, y
 
     def setImageShift2(self, x: int, y: int):
         self.def3.SetIS2(x, y)
 
     def getStagePosition(self) -> Tuple[int, int, int, int, int]:
-        """x, y, z in nanometer a and b in degrees."""
+        """X, y, z in nanometer a and b in degrees."""
         x, y, z, a, b, result = self.stage3.GetPos()
         return x, y, z, a, b
 
     def isStageMoving(self):
         x, y, z, a, b, result = self.stage3.GetStatus()
         return x or y or z or a or b
 
@@ -378,20 +378,20 @@
         self.stage3.SetOrg()
 
     def stopStageMV(self):
         self.stage3.Stop()
         print('Goniometer stopped moving.')
 
     def getFunctionMode(self) -> str:
-        """mag1, mag2, lowmag, samag, diff."""
+        """Mag1, mag2, lowmag, samag, diff."""
         mode, name, result = self.eos3.GetFunctionMode()
         return self.FUNCTION_MODES[mode]
 
     def setFunctionMode(self, value: int):
-        """mag1, mag2, lowmag, samag, diff."""
+        """Mag1, mag2, lowmag, samag, diff."""
         if isinstance(value, str):
             try:
                 value = self.FUNCTION_MODES.index(value)
             except ValueError:
                 raise JEOLValueError(f'Unrecognized function mode: {value}')
         self.eos3.SelectFunctionMode(value)
 
@@ -423,15 +423,15 @@
     def getDiffShift(self) -> Tuple[int, int]:
         x, y, result = self.def3.GetPLA()
         return x, y
 
     def setDiffShift(self, x: int, y: int):
         self.def3.SetPLA(x, y)
 
-    def releaseConnection(self):
+    def release_connection(self):
         comtypes.CoUninitialize()
         logger.info('Connection to microscope released')
 
     def isBeamBlanked(self) -> bool:
         value, result = self.def3.GetBeamBlank()
         return bool(value)
 
@@ -489,15 +489,15 @@
             return 'up'
         elif value == DOWN:
             return 'down'
         else:
             return value
 
     def setScreenPosition(self, value: str):
-        """value = 'up' or 'down'"""
+        """Value = 'up' or 'down'."""
         UP, DOWN = 2, 0
         if value == 'up':
             self.screen2.SelectAngle(UP)
         elif value == 'down':
             self.screen2.SelectAngle(DOWN)
         else:
             raise JEOLValueError('No such screen position:', value, "(must be 'up'/'down')")
```

### Comparing `instamatic-1.9.0/instamatic/TEMController/lenses.py` & `instamatic-2.0.0/src/instamatic/TEMController/lenses.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,18 +41,19 @@
     def __init__(self, tem):
         super().__init__(tem=tem)
         self._getter = self._tem.getDiffFocus
         self._setter = self._tem.setDiffFocus
         self.is_defocused = False
 
     def set(self, value: int, confirm_mode: bool = True):
-        """
-        confirm_mode: verify that TEM is set to the correct mode ('diff').
+        """confirm_mode: verify that TEM is set to the correct mode ('diff').
+
         IL1 maps to different values in image and diffraction mode.
-        Turning it off results in a 2x speed-up in the call, but it will silently fail if the TEM is in the wrong mode.
+        Turning it off results in a 2x speed-up in the call, but it will
+        silently fail if the TEM is in the wrong mode.
         """
         self._setter(value, confirm_mode=confirm_mode)
 
     def defocus(self, offset):
         """Apply a defocus to the IL1 lens, use `.refocus` to restore the
         previous setting."""
         if self.is_defocused:
```

### Comparing `instamatic-1.9.0/instamatic/TEMController/microscope.py` & `instamatic-2.0.0/src/instamatic/TEMController/microscope.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,13 +45,13 @@
         config.load_microscope_config(microscope_name=name)
         interface = config.microscope.interface
     else:
         interface = config.microscope.interface
 
     if use_server:
         from .microscope_client import MicroscopeClient
-        tem = MicroscopeClient(name=name)
+        tem = MicroscopeClient(interface=interface)
     else:
-        cls = get_tem(interface)
+        cls = get_tem(interface=interface)
         tem = cls(name=name)
 
     return tem
```

### Comparing `instamatic-1.9.0/instamatic/TEMController/microscope_client.py` & `instamatic-2.0.0/src/instamatic/TEMController/microscope_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,18 +37,19 @@
     """Simulates a Microscope object and synchronizes calls over a socket
     server.
 
     For documentation, see the actual python interface to the microscope
     API.
     """
 
-    def __init__(self, name):
+    def __init__(self, *, interface: str):
         super().__init__()
 
-        self.name = name
+        self.interface = interface
+        self.name = interface
         self._bufsize = BUFSIZE
 
         try:
             self.connect()
         except ConnectionRefusedError:
             start_server_in_subprocess()
 
@@ -106,15 +107,15 @@
             raise exception_list.get(error_code, TEMCommunicationError)(*args)
 
         else:
             raise ConnectionError(f'Unknown status code: {status}')
 
     def _init_dict(self):
         from instamatic.TEMController.microscope import get_tem
-        tem = get_tem(self.name)
+        tem = get_tem(interface=self.interface)
 
         self._dct = {key: value for key, value in tem.__dict__.items() if not key.startswith('_')}
 
     def __dir__(self):
         return self._dct.keys()
 
     def check_goniotool(self):
```

### Comparing `instamatic-1.9.0/instamatic/TEMController/simu_microscope.py` & `instamatic-2.0.0/src/instamatic/TEMController/simu_microscope.py`

 * *Files 2% similar despite different names*

```diff
@@ -432,20 +432,20 @@
         return self._stage_dict['a']['speed_setting']
 
     def setRotationSpeed(self, value: int):
         self._stage_dict['a']['speed_setting'] = value
         self._stage_dict['a']['speed'] = 10.0 * (value / 12)
 
     def getFunctionMode(self) -> str:
-        """mag1, mag2, lowmag, samag, diff."""
+        """Mag1, mag2, lowmag, samag, diff."""
         mode = self.FunctionMode_value
         return FUNCTION_MODES[mode]
 
     def setFunctionMode(self, value: int):
-        """mag1, mag2, lowmag, samag, diff."""
+        """Mag1, mag2, lowmag, samag, diff."""
         if isinstance(value, str):
             try:
                 value = FUNCTION_MODES.index(value)
             except ValueError:
                 raise TEMValueError(f'Unrecognized function mode: {value}')
         self.FunctionMode_value = value
 
@@ -471,15 +471,15 @@
     def getDiffShift(self) -> Tuple[int, int]:
         return self.DiffractionShift_x, self.DiffractionShift_y
 
     def setDiffShift(self, x: int, y: int):
         self.DiffractionShift_x = x
         self.DiffractionShift_y = y
 
-    def releaseConnection(self):
+    def release_connection(self):
         print('Connection to microscope released')
 
     def isBeamBlanked(self) -> bool:
         return self.beamblank
 
     def setBeamBlank(self, mode: bool):
         """True/False or 1/0."""
@@ -510,15 +510,15 @@
         """0-based indexing for GetSpotSize, add 1 for consistency."""
         return self.spotsize
 
     def getScreenPosition(self) -> str:
         return self.screenposition_value
 
     def setScreenPosition(self, value: int):
-        """value = 'up' or 'down'"""
+        """Value = 'up' or 'down'."""
         if value not in ('up', 'down'):
             raise TEMValueError(f'No such screen position: `{value}`.')
         self.screenposition_value = value
 
     def setSpotSize(self, value: int):
         self.spotsize = value
```

### Comparing `instamatic-1.9.0/instamatic/TEMController/stage.py` & `instamatic-2.0.0/src/instamatic/TEMController/stage.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,18 +21,19 @@
 
     def __repr__(self):
         x, y, z, a, b = self.get()
         return f'{self.name}(x={x:.1f}, y={y:.1f}, z={z:.1f}, a={a:.1f}, b={b:.1f})'
 
     @property
     def name(self) -> str:
+        """Get name of the class."""
         return self.__class__.__name__
 
     def set(self, x: int = None, y: int = None, z: int = None, a: int = None, b: int = None, wait: bool = True) -> None:
-        """wait: bool, block until stage movement is complete (JEOL only)"""
+        """Wait: bool, block until stage movement is complete (JEOL only)"""
         self._setter(x, y, z, a, b, wait=wait)
 
     def set_with_speed(self, x: int = None, y: int = None, z: int = None, a: int = None, b: int = None, wait: bool = True, speed: float = 1.0) -> None:
         """Note that this function only works on FEI machines.
 
         wait: ignored, but necessary for compatibility with JEOL API
         speed: float, set stage rotation with specified speed (FEI only)
@@ -78,42 +79,45 @@
     def get(self) -> Tuple[int, int, int, int, int]:
         """Get stage positions; x, y, z, and status of the rotation axes; a,
         b."""
         return StagePositionTuple(*self._getter())
 
     @property
     def x(self) -> int:
+        """X position."""
         x, y, z, a, b = self.get()
         return x
 
     @x.setter
     def x(self, value: int):
         self.set(x=value, wait=self._wait)
 
     @property
     def y(self) -> int:
+        """Y position."""
         x, y, z, a, b = self.get()
         return y
 
     @y.setter
     def y(self, value: int):
         self.set(y=value, wait=self._wait)
 
     @property
     def xy(self) -> Tuple[int, int]:
+        """XY position as a tuple."""
         x, y, z, a, b = self.get()
         return x, y
 
     @xy.setter
     def xy(self, values: Tuple[int, int]):
         x, y = values
         self.set(x=x, y=y, wait=self._wait)
 
     def move_in_projection(self, delta_x: int, delta_y: int) -> None:
-        r"""y and z are always perpendicular to the sample stage. To achieve the
+        r"""Y and z are always perpendicular to the sample stage. To achieve the
         movement in the projection, x and yshould be broken down into the
         components z' and y'.
 
         y = y' * cos(a)
         z = y' * sin(a)
 
         z'|  / z
@@ -136,32 +140,35 @@
         a = np.radians(a)
         y = y + delta_z * np.sin(a)
         z = z + delta_z * np.cos(a)
         self.set(y=y, z=z)
 
     @property
     def z(self) -> int:
+        """Stage height Z."""
         x, y, z, a, b = self.get()
         return z
 
     @z.setter
     def z(self, value: int):
         self.set(z=value, wait=self._wait)
 
     @property
     def a(self) -> int:
+        """Rotation angle."""
         x, y, z, a, b = self.get()
         return a
 
     @a.setter
     def a(self, value: int):
         self.set(a=value, wait=self._wait)
 
     @property
     def b(self) -> int:
+        """Secondary rotation angle."""
         x, y, z, a, b = self.get()
         return b
 
     @b.setter
     def b(self, value: int):
         self.set(b=value, wait=self._wait)
```

### Comparing `instamatic-1.9.0/instamatic/TEMController/states.py` & `instamatic-2.0.0/src/instamatic/TEMController/states.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import time
 
 
 class State:
-    """Class for describing microscope state objects."""
+    """Generic class for describing microscope state objects."""
 
     def __init__(self, tem):
         super().__init__()
         self._tem = tem
         self._getter = None
         self._setter = None
 
@@ -17,14 +17,15 @@
         """Allow `str` comparison."""
         if isinstance(other, str):
             return self.state == other
         return False
 
     @property
     def name(self) -> str:
+        """Return name of the state control."""
         return self.__class__.__name__
 
 
 class Beam(State):
     """Control for the beam blanker."""
 
     def __init__(self, tem):
@@ -54,32 +55,35 @@
         """Turn the beamblank off, optionally wait for `delay` in ms to allow
         the beam to settle."""
         self._setter(False)
         if delay:
             time.sleep(delay)
 
     def set(self, state: str, delay: float = 0.0):
+        """Set state of the beam, with optional delay in ms."""
         index = self._states.index(state)
         f = (self.unblank, self.blank)[index]
         f(delay=delay)
 
     def get(self) -> str:
+        """Get current state of the beam."""
         return self._states[self.is_blanked]
 
 
 class Mode(State):
     """Control for the magnification mode."""
 
     def __init__(self, tem):
         super().__init__(tem=tem)
         self._setter = self._tem.setFunctionMode
         self._getter = self._tem.getFunctionMode
 
     @property
     def state(self) -> str:
+        """Return magnification mode."""
         return self.get()
 
     def set(self, mode: str) -> None:
         """Set the function mode."""
         self._setter(mode)
 
     def get(self) -> str:
```

### Comparing `instamatic-1.9.0/instamatic/__init__.py` & `instamatic-2.0.0/src/instamatic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 #   | | '_ \/ __| __/ _` | '_ ` _ \ / _` | __| |/ __|   #
 #   | | | | \__ \ || (_| | | | | | | (_| | |_| | (__    #
 #   |_|_| |_|___/\__\__,_|_| |_| |_|\__,_|\__|_|\___|   #
 #                                                       #
 # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 """
 
-__version__ = '1.9.0'
+__version__ = '2.0.0'
 __title__ = 'instamatic'
 __long_title__ = f'{__title__} v{__version__}'
 __author__ = 'Stef Smeets'
 __author_email__ = 's.smeets@esciencecenter.nl'
 __description__ = 'Python program for automated serial electron diffraction data collection'
 __license__ = 'GPLv3'
 __url__ = 'https://github.com/instamatic-dev/instamatic'
```

### Comparing `instamatic-1.9.0/instamatic/acquire_at_items.py` & `instamatic-2.0.0/src/instamatic/acquire_at_items.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/banner.py` & `instamatic-2.0.0/src/instamatic/banner.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/browser.py` & `instamatic-2.0.0/src/instamatic/browser.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/calibrate/calibrate_beamshift.py` & `instamatic-2.0.0/src/instamatic/calibrate/calibrate_beamshift.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
             plt.savefig(os.path.join(outdir, to_file))
             plt.close()
         else:
             plt.show()
 
     def center(self, ctrl):
         """Return beamshift values to center the beam in the frame."""
-        pixel_center = [val / 2.0 for val in ctrl.cam.getImageDimensions()]
+        pixel_center = [val / 2.0 for val in ctrl.cam.get_image_dimensions()]
 
         beamshift = self.pixelcoord_to_beamshift(pixel_center)
         if ctrl:
             ctrl.beamshift.set(*beamshift)
         else:
             return beamshift
```

### Comparing `instamatic-1.9.0/instamatic/calibrate/calibrate_brightness.py` & `instamatic-2.0.0/src/instamatic/calibrate/calibrate_brightness.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/calibrate/calibrate_directbeam.py` & `instamatic-2.0.0/src/instamatic/calibrate/calibrate_directbeam.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/calibrate/calibrate_imageshift12.py` & `instamatic-2.0.0/src/instamatic/calibrate/calibrate_imageshift12.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/calibrate/calibrate_stage_lowmag.py` & `instamatic-2.0.0/src/instamatic/calibrate/calibrate_stage_lowmag.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/calibrate/calibrate_stage_mag1.py` & `instamatic-2.0.0/src/instamatic/calibrate/calibrate_stage_mag1.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/calibrate/calibrate_stagematrix.py` & `instamatic-2.0.0/src/instamatic/calibrate/calibrate_stagematrix.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,15 +154,15 @@
 
     stage_x, stage_y = ctrl.stage.xy
 
     stage_shifts = []  # um
 
     mag = ctrl.magnification.value
     mode = ctrl.mode.get()
-    binning = ctrl.cam.getBinning()
+    binning = ctrl.cam.get_binning()
 
     pairs = []
 
     for i, (n_steps, step) in enumerate(args):
         j = 0
 
         current_stage_pos = ctrl.stage
@@ -289,15 +289,15 @@
         ctrl.magnification.value = mag
     else:
         mode = ctrl.mode.get()
         mag = ctrl.magnification.value
 
     print(f'\nCalibrating stagematrix mode=`{mode}` mag={mag}\n')
 
-    camera_shape = ctrl.cam.getCameraDimensions()
+    camera_shape = ctrl.cam.get_camera_dimensions()
     pixelsize = config.calibration[mode]['pixelsize'][mag]
 
     if pixelsize == 1.0 or pixelsize == 0.0:
         raise ValueError(f'Invalid pixelsize for `{mode}` @ {mag}x -> {pixelsize}')
 
     displacement = np.array(camera_shape) * pixelsize
     x_step, y_step = displacement * (1 - overlap)
```

### Comparing `instamatic-1.9.0/instamatic/calibrate/center_z.py` & `instamatic-2.0.0/src/instamatic/calibrate/center_z.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/calibrate/fit.py` & `instamatic-2.0.0/src/instamatic/calibrate/fit.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/camera/CCDCOM.h` & `instamatic-2.0.0/src/instamatic/camera/CCDCOM.h`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/camera/CCDCOM2_x64_gatan.dll` & `instamatic-2.0.0/src/instamatic/camera/CCDCOM2_x64_gatan.dll`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/camera/CCDCOM2_x64_simulation.dll` & `instamatic-2.0.0/src/instamatic/camera/CCDCOM2_x64_simulation.dll`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/camera/CCDCOM2_x86_gatan.dll` & `instamatic-2.0.0/src/instamatic/camera/CCDCOM2_x86_gatan.dll`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/camera/CCDCOM2_x86_simulation.dll` & `instamatic-2.0.0/src/instamatic/camera/CCDCOM2_x86_simulation.dll`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/camera/EMCameraObj.dll` & `instamatic-2.0.0/src/instamatic/camera/EMCameraObj.dll`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/camera/camera.py` & `instamatic-2.0.0/src/instamatic/camera/camera.py`

 * *Files 0% similar despite different names*

```diff
@@ -188,13 +188,13 @@
         else:
             write_tiff('out', arr, header=h)
 
 
 if __name__ == '__main__':
     # main_entry()
     cam = Camera(use_server=True)
-    arr = cam.getImage(exposure=0.1)
+    arr = cam.get_image(exposure=0.1)
     print(arr)
     print(arr.shape)
 
     from IPython import embed
     embed(banner1='')
```

### Comparing `instamatic-1.9.0/instamatic/camera/camera_client.py` & `instamatic-2.0.0/src/instamatic/camera/camera_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         self.shms = {}
 
         self._init_dict()
         self._init_attr_dict()
 
         atexit.register(self.s.close)
 
-        xres, yres = self.getImageDimensions()
+        xres, yres = self.get_image_dimensions()
         bitdepth = 4
         self._imagebufsize = bitdepth * xres * yres + self._bufsize
 
     @property
     def is_local_connection(self):
         """Check if the socket connection is a local connection."""
         return self.s.getpeername()[0] == self.s.getsockname()[0]
@@ -115,15 +115,19 @@
 
         return wrapper
 
     def _eval_dct(self, dct):
         """Takes approximately 0.2-0.3 ms per call if HOST=='localhost'."""
         self.s.send(dumper(dct))
 
-        acquiring_image = dct['attr_name'] == 'getImage'
+        acquiring_image = dct['attr_name'] == 'get_image'
+        acquiring_movie = dct['attr_name'] == 'get_movie'
+
+        if acquiring_movie:
+            raise NotImplementedError('Acquiring movies over a socket is not supported.')
 
         if acquiring_image and not self.use_shared_memory:
             response = self.s.recv(self._imagebufsize)
         else:
             response = self.s.recv(self._bufsize)
 
         if response:
```

### Comparing `instamatic-1.9.0/instamatic/camera/camera_emmenu.py` & `instamatic-2.0.0/src/instamatic/camera/camera_emmenu.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,64 +100,64 @@
 
         # set up instamatic data directory
         self.top_drc_index = self._immgr.TopDirectory
         self.top_drc_name = self._immgr.DirectoryName(self.top_drc_index)
 
         # check if exists
         if not self._immgr.DirectoryExist(self.top_drc_index, drc_name):
-            if self.getEMMenuVersion().startswith('4.'):
+            if self.get_emmenu_version().startswith('4.'):
                 self._immgr.CreateNewSubDirectory(self.top_drc_index, drc_name, 2, 2)
             else:
                 # creating new subdirectories is bugged in EMMENU 5.0.9.0/5.0.10.0
                 # No work-around -> raise exception for now until it is fixed
                 raise ValueError(f'Directory `{drc_name}` does not exist in the EMMENU Image manager.')
 
         self.drc_name = drc_name
         self.drc_index = self._immgr.DirectoryHandleFromName(drc_name)
 
         self._vp.DirectoryHandle = self.drc_index  # set current directory
 
         self.load_defaults()
 
-        msg = f'Camera `{self.getCameraName()}` ({self.name}) initialized'
+        msg = f'Camera `{self.get_camera_name()}` ({self.name}) initialized'
         # print(msg)
         logger.info(msg)
 
-        atexit.register(self.releaseConnection)
+        atexit.register(self.release_connection)
 
     def load_defaults(self) -> None:
         if self.name != config.settings.camera:
             config.load_camera_config(camera_name=self.name)
 
         self.__dict__.update(config.camera.mapping)
 
         self.streamable = False
 
-    def listConfigs(self) -> list:
+    def list_configs(self) -> list:
         """List the configs from the Configuration Manager."""
         print(f'Configurations for camera {self.name}')
         current = self._vp.Configuration
 
         lst = []
 
         for i, cfg in enumerate(self._obj.CameraConfigurations):
             is_selected = (current == cfg.Name)
             end = ' (selected)' if is_selected else ''
             print(f'{i+1:2d} - {cfg.Name}{end}')
             lst.append(cfg.Name)
 
         return lst
 
-    def getCurrentConfigName(self) -> str:
+    def get_current_config_name(self) -> str:
         """Return the name of the currently selected configuration in
         EMMENU."""
-        cfg = self.getCurrentConfig(as_dict=False)
+        cfg = self.get_current_config(as_dict=False)
         return cfg.Name
 
-    def getCurrentConfig(self, as_dict: bool = True) -> dict:
+    def get_current_config(self, as_dict: bool = True) -> dict:
         """Get selected config object currently associated with the
         viewport."""
         vp_cfg_name = self._vp.Configuration
         count = self._obj.CameraConfigurations.Count
         for j in range(1, count + 1):
             cfg = self._obj.CameraConfigurations.Item(j)
             if cfg.Name == vp_cfg_name:
@@ -210,23 +210,23 @@
             d['UseScriptAfterSeries'] = bool(cfg.UseScriptAfterSeries)
             d['ShutterMode'] = cfg.ShutterMode  # int
             d['ShutterModeStr'] = ('None', 'SH', 'BB', 'SH/BB', 'Dark/SH', 'Dark/BB', 'Dark/SH/BB')[cfg.ShutterMode]  # str
             return d
         else:
             return cfg
 
-    def selectConfig(self) -> None:
+    def select_config(self) -> None:
         """Select config by name."""
-        cfgs = self.listConfigs()
+        cfgs = self.list_configs()
         if config not in cfgs:
             raise ValueError(f'No such config: {config} -> must be one of {cfgs}')
 
         raise NotImplementedError
 
-    def getCurrentCameraInfo(self) -> dict:
+    def get_current_camera_info(self) -> dict:
         """Gets the current camera object."""
         cam = self._cam
 
         d = {}
         d['RealSizeX'] = cam.RealSizeX  # int
         d['RealSizeY'] = cam.RealSizeY  # int
         d['MaximumSizeX'] = cam.MaximumSizeX  # int
@@ -238,20 +238,20 @@
         d['PixelSizeX'] = cam.PixelSizeX  # int
         d['PixelSizeY'] = cam.PixelSizeY  # int
         d['Dynamic'] = cam.Dynamic  # int
         d['PostMag'] = cam.PostMag  # float
         d['CamCGroup'] = cam.CamCGroup  # int
         return d
 
-    def getCameraType(self) -> str:
+    def get_camera_type(self) -> str:
         """Get the name of the camera currently in use."""
-        cfg = self.getCurrentConfig(as_dict=False)
+        cfg = self.get_current_config(as_dict=False)
         return cfg.CameraType
 
-    def getEMMenuVersion(self) -> str:
+    def get_emmenu_version(self) -> str:
         """Get the version number of EMMENU."""
         return self._obj.EMMENUVersion
 
     def lock(self) -> None:
         """Lockdown interactions with emmenu, must call `self.unlock` to
         unlock.
 
@@ -261,15 +261,15 @@
         """
         self._obj.EnableMainframe(1)
 
     def unlock(self) -> None:
         """Unlock emmenu after it has been locked down with `self.lock`"""
         self._obj.EnableMainframe(0)
 
-    def listDirectories(self) -> dict:
+    def list_directories(self) -> dict:
         """List subdirectories of the top directory."""
         top_j = self._immgr.TopDirectory
         top_name = self._immgr.FullDirectoryName(top_j)
         print(f'{top_name} ({top_j})')
 
         drc_j = self._immgr.SubDirectory(top_j)
 
@@ -281,138 +281,138 @@
 
             d[drc_j] = drc_name
 
             drc_j = self._immgr.NextDirectory(drc_j)  # get next
 
         return d
 
-    def getEMVectorByIndex(self, img_index: int, drc_index: int = None) -> dict:
+    def get_emvector_by_index(self, img_index: int, drc_index: int = None) -> dict:
         """Returns the EMVector by index as a python dictionary."""
-        p = self.getImageByIndex(img_index, drc_index)
+        p = self.get_image_by_index(img_index, drc_index)
         v = p.EMVector
         d = EMVector2dict(v)
         return d
 
-    def deleteAllImages(self) -> None:
+    def delete_all_images(self) -> None:
         """Clears all images currently stored in EMMENU buffers."""
         for i, p in enumerate(self._emi):
             try:
                 self._emi.DeleteImage(p)
             except BaseException:
                 # sometimes EMMenu also loses track of image pointers...
                 print(f'Failed to delete buffer {i} ({p})')
 
-    def deleteImageByIndex(self, img_index: int, drc_index: int = None) -> int:
+    def delete_image_by_index(self, img_index: int, drc_index: int = None) -> int:
         """Delete the image from EMMENU by its index."""
-        p = self.getImageByIndex(img_index, drc_index)
+        p = self.get_image_by_index(img_index, drc_index)
         self._emi.DeleteImage(p)  # alternative: self._emi.Remove(p.ImgHandle)
 
-    def getImageByIndex(self, img_index: int, drc_index: int = None) -> int:
+    def get_image_by_index(self, img_index: int, drc_index: int = None) -> int:
         """Grab data from the image manager by index. Return image pointer
         (COM).
 
         Not accessible through server.
         """
         if not drc_index:
             drc_index = self.drc_index
 
         p = self._immgr.Image(drc_index, img_index)
 
         return p
 
-    def getImageDataByIndex(self, img_index: int, drc_index: int = None) -> 'np.array':
+    def get_image_data_by_index(self, img_index: int, drc_index: int = None) -> 'np.array':
         """Grab data from the image manager by index.
 
         Return numpy 2D array
         """
-        p = self.getImageByIndex(img_index, drc_index)
+        p = self.get_image_by_index(img_index, drc_index)
 
         tpe = p.DataType
         method = type_dict[tpe]
 
         f = getattr(p, method)
         arr = f()  # -> tuple of tuples
 
         return np.array(arr)
 
-    def getCameraDimensions(self) -> (int, int):
+    def get_camera_dimensions(self) -> (int, int):
         """Get the maximum dimensions reported by the camera."""
-        # cfg = self.getCurrentConfig()
+        # cfg = self.get_current_config()
         # return cfg.DimensionX, cfg.DimensionY
         return self._cam.RealSizeX, self._cam.RealSizeY
         # return self._cam.MaximumSizeX, self._cam.MaximumSizeY
 
-    def getImageDimensions(self) -> (int, int):
+    def get_image_dimensions(self) -> (int, int):
         """Get the dimensions of the image."""
-        binning = self.getBinning()
+        binning = self.get_binning()
         return int(self._cam.RealSizeX / binning), int(self._cam.RealSizeY / binning)
 
-    def getPhysicalPixelsize(self) -> (int, int):
+    def get_physical_pixelsize(self) -> (int, int):
         """Returns the physical pixel size of the camera nanometers."""
         return self._cam.PixelSizeX, self._cam.PixelSizeY
 
-    def getBinning(self) -> int:
+    def get_binning(self) -> int:
         """Returns the binning corresponding to the currently selected camera
         config."""
-        cfg = self.getCurrentConfig(as_dict=False)
+        cfg = self.get_current_config(as_dict=False)
         bin_x = cfg.BinningX
         bin_y = cfg.BinningY
         assert bin_x == bin_y, 'Binnings differ in X and Y direction! (X: {bin_x} | Y: {bin_y})'
         return bin_x
 
-    def getCameraName(self) -> str:
+    def get_camera_name(self) -> str:
         """Get the name reported by the camera."""
         return self._cam.name
 
-    def writeTiffFromPointer(self, image_pointer, filename: str) -> None:
+    def write_tiff_from_pointer(self, image_pointer, filename: str) -> None:
         """Write tiff file using the EMMENU machinery `image_pointer` is the
         memory address returned by `getImageIndex()`"""
         self._emf.WriteTiff(image_pointer, filename)
 
-    def writeTiff(self, image_index, filename: str) -> None:
+    def write_tiff(self, image_index, filename: str) -> None:
         """Write tiff file using the EMMENU machinery `image_index` is the
         index in the current directory of the image to be written."""
         drc_index = self.drc_index
-        p = self.getImageByIndex(image_index, drc_index)
+        p = self.get_image_by_index(image_index, drc_index)
 
-        self.writeTiffFromPointer(p, filename)
+        self.write_tiff_from_pointer(p, filename)
 
-    def writeTiffs(self, start_index: int, stop_index: int, path: str, clear_buffer: bool = False) -> None:
+    def write_tiffs(self, start_index: int, stop_index: int, path: str, clear_buffer: bool = False) -> None:
         """Write a series of data in tiff format and writes them to the given
         `path` using EMMENU machinery."""
         path = Path(path)
         drc_index = self.drc_index
 
         if stop_index <= start_index:
             raise IndexError(f'`stop_index`: {stop_index} >= `start_index`: {start_index}')
 
         for i, image_index in enumerate(range(start_index, stop_index + 1)):
-            p = self.getImageByIndex(image_index, drc_index)
+            p = self.get_image_by_index(image_index, drc_index)
 
             fn = str(path / f'{i:04d}.tiff')
             print(f'Image #{image_index} -> {fn}')
 
             # TODO: wrap writeTiff in try/except
             # writeTiff causes vague error if image does not exist
 
-            self.writeTiffFromPointer(p, fn)
+            self.write_tiff_from_pointer(p, fn)
 
             if clear_buffer:
                 # self._immgr.DeleteImageBuffer(drc_index, image_index)  # does not work on 3200
                 self._emi.DeleteImage(p)  # also clears from buffer
 
         print(f'Wrote {i+1} images to {path}')
 
-    def getImage(self, **kwargs) -> 'np.array':
+    def get_image(self, **kwargs) -> 'np.array':
         """Acquire image through EMMENU and return data as np array."""
         self._vp.AcquireAndDisplayImage()
         i = self.get_image_index()
-        return self.getImageDataByIndex(i)
+        return self.get_image_data_by_index(i)
 
-    def acquireImage(self, **kwargs) -> int:
+    def acquire_image(self, **kwargs) -> int:
         """Acquire image through EMMENU and store in the Image Manager Returns
         the image index."""
         self._vp.AcquireAndDisplayImage()
         return self.get_image_index()
 
     def set_image_index(self, index: int) -> None:
         """Change the currently selected buffer by the image index Note that
@@ -482,29 +482,29 @@
             self._vp.AutoIncrement = 0
 
     def get_timestamps(self, start_index: int, end_index: int) -> list:
         """Get timestamps in seconds for given image index range."""
         drc_index = self.drc_index
         timestamps = []
         for i, image_index in enumerate(range(start_index, end_index + 1)):
-            p = self.getImageByIndex(image_index, drc_index)
+            p = self.get_image_by_index(image_index, drc_index)
             t = p.EMVector.lImgCreationTime
             timestamps.append(t)
         return timestamps
 
-    def releaseConnection(self) -> None:
+    def release_connection(self) -> None:
         """Release the connection to the camera."""
         self.stop_liveview()
 
         self._vp.DirectoryHandle = self.top_drc_index
         self._vp.SetCaption('Image')
         self.set_image_index(0)
         # self._immgr.DeleteDirectory(self.drc_index)  # bugged in EMMENU 5.0.9.0/5.0.10.0, FIXME later
 
-        msg = f'Connection to camera `{self.getCameraName()}` ({self.name}) released'
+        msg = f'Connection to camera `{self.get_camera_name()}` ({self.name}) released'
         # print(msg)
         logger.info(msg)
 
         comtypes.CoUninitialize()
 
 
 if __name__ == '__main__':
```

### Comparing `instamatic-1.9.0/instamatic/camera/camera_gatan.py` & `instamatic-2.0.0/src/instamatic/camera/camera_gatan.py`

 * *Files 6% similar despite different names*

```diff
@@ -124,36 +124,36 @@
         self._initCCDCOM.restype = c_int
 
         self._isCameraInfoAvailable = getattr(lib, symbols['isCameraInfoAvailable'])
         self._isCameraInfoAvailable.restype = c_bool
 
         self._releaseCCDCOM = getattr(lib, symbols['releaseCCDCOM'])
 
-        self.establishConnection()
+        self.establish_connection()
 
         self.load_defaults()
 
-        msg = f'Camera {self.getName()} initialized'
+        msg = f'Camera {self.get_name()} initialized'
         logger.info(msg)
 
-        # dim_x, dim_y = self.getImageDimensions()
+        # dim_x, dim_y = self.get_image_dimensions()
         # print(f"Dimensions {dim_x}x{dim_y}")
-        # print(f"Info {self.isCameraInfoAvailable()} | Count {self.getCameraCount()}")
+        # print(f"Info {self.is_camera_info_available()} | Count {self.getCameraCount()}")
 
-        atexit.register(self.releaseConnection)
+        atexit.register(self.release_connection)
 
     def load_defaults(self):
         if self.name != config.settings.camera:
             config.load_camera_config(camera_name=self.name)
 
         self.__dict__.update(config.camera.mapping)
 
         self.streamable = False
 
-    def getImage(self, exposure=None, binsize=None, **kwargs) -> np.ndarray:
+    def get_image(self, exposure=None, binsize=None, **kwargs) -> np.ndarray:
         """Image acquisition routine.
 
         exposure: exposure time in seconds
         binsize: which binning to use
         showindm: show image in digital micrograph
         xmin, xmax, ymin, ymax: retrieve image with smaller size from a subset of pixels
         """
@@ -191,40 +191,40 @@
         if self.name == 'simulateDLL':
             # add some noise to static simulated images
             arr *= np.random.random((xres, yres)) + 0.5
             time.sleep(exposure)
 
         return arr
 
-    def isCameraInfoAvailable(self) -> bool:
+    def is_camera_info_available(self) -> bool:
         """Return the status of the camera."""
         return self._isCameraInfoAvailable()
 
-    def getCameraDimensions(self) -> (int, int):
+    def get_camera_dimensions(self) -> (int, int):
         """Return the dimensions reported by the camera."""
         pnWidth = c_int(0)
         pnHeight = c_int(0)
         self._cameraDimensions(byref(pnWidth), byref(pnHeight))
         return pnWidth.value, pnHeight.value
 
-    def getName(self) -> str:
+    def get_name(self) -> str:
         """Return the name reported by the camera."""
         buf = create_unicode_buffer(20)
         self._cameraName(buf, 20)
         return buf.value
 
-    def establishConnection(self) -> None:
+    def establish_connection(self) -> None:
         """Establish connection to the camera."""
         res = self._initCCDCOM(20120101)
         if res != 1:
             raise RuntimeError(f'Could not establish camera connection to {self.name}')
 
-    def releaseConnection(self) -> None:
+    def release_connection(self) -> None:
         """Release the connection to the camera."""
-        name = self.getName()
+        name = self.get_name()
         self._releaseCCDCOM()
         msg = f'Connection to camera {name} released'
         logger.info(msg)
 
 
 if __name__ == '__main__':
     cam = CameraDLL()
```

### Comparing `instamatic-1.9.0/instamatic/camera/camera_gatan2.py` & `instamatic-2.0.0/src/instamatic/camera/camera_gatan2.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,103 +23,103 @@
 
         self.g = GatanSocket()
 
         self._recording = False
 
         self.load_defaults()
 
-        msg = f'Camera `{self.getCameraName()}` ({self.name}) initialized'
+        msg = f'Camera `{self.get_camera_name()}` ({self.name}) initialized'
         # print(msg)
         logger.info(msg)
 
-        atexit.register(self.releaseConnection)
+        atexit.register(self.release_connection)
 
     def load_defaults(self) -> None:
         if self.name != config.settings.camera:
             config.load_camera_config(camera_name=self.name)
 
         self.__dict__.update(config.camera.mapping)
 
         self.streamable = False
 
-    def getCameraType(self) -> str:
+    def get_camera_type(self) -> str:
         """Get the name of the camera currently in use."""
         raise NotImplementedError
 
-    def getDMVersion(self) -> str:
+    def get_dm_version(self) -> str:
         """Get the version number of DM."""
         return self.g.GetDMVersion()
 
-    def getCameraDimensions(self) -> (int, int):
+    def get_camera_dimensions(self) -> (int, int):
         """Get the maximum dimensions reported by the camera."""
         raise NotImplementedError
 
-    def getImageDimensions(self) -> (int, int):
+    def get_image_dimensions(self) -> (int, int):
         """Get the dimensions of the image."""
-        binning = self.getBinning()
-        dim_x, dim_y = self.getCameraDimensions()
+        binning = self.get_binning()
+        dim_x, dim_y = self.get_camera_dimensions()
         return int(dim_x / binning), int(dim_y / binning)
 
-    def getPhysicalPixelsize(self) -> (int, int):
+    def get_physical_pixelsize(self) -> (int, int):
         """Returns the physical pixel size of the camera nanometers."""
         raise NotImplementedError
 
-    def getBinning(self) -> int:
+    def get_binning(self) -> int:
         """Returns the binning corresponding to the currently selected camera
         config."""
         raise NotImplementedError
 
-    def getCameraName(self) -> str:
+    def get_camera_name(self) -> str:
         """Get the name reported by the camera."""
         return self.name
 
-    def writeTiff(self, filename: str) -> None:
+    def write_tiff(self, filename: str) -> None:
         """Write tiff file using the DM machinery."""
         raise NotImplementedError
 
-    def writeTiffs(self) -> None:
+    def write_tiffs(self) -> None:
         """Write a series of data in tiff format and writes them to the given
         `path`"""
         raise NotImplementedError
 
         path = Path(path)
         i = 0
 
         print(f'Wrote {i+1} images to {path}')
 
-    def getImage(self,
-                 exposure=0.400,
-                 binning=1,
-                 processing='gain normalized',
-                 ) -> 'np.array':
+    def get_image(self,
+                  exposure=0.400,
+                  binning=1,
+                  processing='gain normalized',
+                  ) -> 'np.array':
         """Acquire image through DM and return data as np array."""
 
         width, height = self.dimensions
         top = 0
         left = 0
         bottom = height
         right = width
 
-        arr = self.g.getImage(processing=processing,
-                              height=height,
-                              width=width,
-                              binning=binning,
-                              top=top,
-                              left=left,
-                              bottom=bottom,
-                              right=right,
-                              exposure=exposure,
-                              shutterDelay=0,
-                              )
+        arr = self.g.get_image(processing=processing,
+                               height=height,
+                               width=width,
+                               binning=binning,
+                               top=top,
+                               left=left,
+                               bottom=bottom,
+                               right=right,
+                               exposure=exposure,
+                               shutterDelay=0,
+                               )
 
         return arr
 
-    def acquireImage(self, **kwargs) -> 'np.array':
+    def acquire_image(self, **kwargs) -> 'np.array':
         """Acquire image through DM."""
-        return self.getImage(**kwargs)
+        return self.get_image(**kwargs)
 
     def get_ready_for_record(self) -> None:
         self.reset_record_vars()
 
         while True:
             ready_for_acquire = self.get_tag('ready_for_acquire')
             if ready_for_acquire:
@@ -153,17 +153,17 @@
         """Set exposure time in ms."""
         raise NotImplementedError
 
     def get_exposure(self) -> int:
         """Return exposure time in ms."""
         raise NotImplementedError
 
-    def releaseConnection(self) -> None:
+    def release_connection(self) -> None:
         """Release the connection to the camera."""
-        msg = f'Connection to camera `{self.getCameraName()}` ({self.name}) released'
+        msg = f'Connection to camera `{self.get_camera_name()}` ({self.name}) released'
         # print(msg)
         logger.info(msg)
 
     def set_tag(self, key: str, value: float) -> None:
         """Set the tag `key` in the DM persistent parameters."""
         if isinstance(value, str):
             value = value.replace('\\', '\\\\')
```

### Comparing `instamatic-1.9.0/instamatic/camera/camera_serval.py` & `instamatic-2.0.0/src/instamatic/camera/camera_serval.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,30 +22,30 @@
         """Initialize camera module."""
         super().__init__()
 
         self.name = name
 
         self.load_defaults()
 
-        self.establishConnection()
+        self.establish_connection()
 
-        msg = f'Camera {self.getName()} initialized'
+        msg = f'Camera {self.get_name()} initialized'
         logger.info(msg)
 
-        atexit.register(self.releaseConnection)
+        atexit.register(self.release_connection)
 
     def load_defaults(self):
         if self.name != config.settings.camera:
             config.load_camera_config(camera_name=self.name)
 
         self.streamable = True
 
         self.__dict__.update(config.camera.mapping)
 
-    def getImage(self, exposure=None, binsize=None, **kwargs) -> np.ndarray:
+    def get_image(self, exposure=None, binsize=None, **kwargs) -> np.ndarray:
         """Image acquisition routine. If the exposure and binsize are not
         given, the default values are read from the config file.
 
         exposure:
             Exposure time in seconds.
         binsize:
             Which binning to use.
@@ -68,15 +68,15 @@
         self.conn.trigger_start()
 
         # Request a frame. Will be streamed *after* the exposure finishes
         img = self.conn.get_image_stream(nTriggers=1, disable_tqdm=True)[0]
         arr = np.array(img)
         return arr
 
-    def getMovie(self, n_frames, exposure=None, binsize=None, **kwargs):
+    def get_movie(self, n_frames, exposure=None, binsize=None, **kwargs):
         """Movie acquisition routine. If the exposure and binsize are not
         given, the default values are read from the config file.
 
         n_frames:
             Number of frames to collect
         exposure:
             Exposure time in seconds.
@@ -94,33 +94,33 @@
             nTriggers=n_frames,
             ExposureTime=exposure,
             TriggerPeriod=exposure,
         )
 
         return arr
 
-    def getImageDimensions(self) -> (int, int):
+    def get_image_dimensions(self) -> (int, int):
         """Get the binned dimensions reported by the camera."""
-        binning = self.getBinning()
-        dim_x, dim_y = self.getCameraDimensions()
+        binning = self.get_binning()
+        dim_x, dim_y = self.get_camera_dimensions()
 
         dim_x = int(dim_x / binning)
         dim_y = int(dim_y / binning)
 
         return dim_x, dim_y
 
-    def getCameraDimensions(self) -> (int, int):
+    def get_camera_dimensions(self) -> (int, int):
         """Get the dimensions reported by the camera."""
         return self.dimensions
 
-    def getName(self) -> str:
+    def get_name(self) -> str:
         """Get the name reported by the camera."""
         return self.name
 
-    def establishConnection(self) -> None:
+    def establish_connection(self) -> None:
         """Establish connection to the camera."""
         self.conn = ServalCamera()
         self.conn.connect(self.url)
         self.conn.set_chip_config_files(
             bpc_file_path=self.bpc_file_path,
             dacs_file_path=self.dacs_file_path)
         self.conn.set_detector_config(**self.detector_config)
@@ -140,18 +140,18 @@
                         # What (image) format to provide the files in.
                         'Format': file_format,
                         # What data to build a frame from
                         'Mode': 'count',
             }],
         }
 
-    def releaseConnection(self) -> None:
+    def release_connection(self) -> None:
         """Release the connection to the camera."""
         self.conn.measurement_stop()
-        name = self.getName()
+        name = self.get_name()
         msg = f"Connection to camera '{name}' released"
         logger.info(msg)
 
 
 if __name__ == '__main__':
     cam = CameraServal()
     from IPython import embed
```

### Comparing `instamatic-1.9.0/instamatic/camera/camera_simu.py` & `instamatic-2.0.0/src/instamatic/camera/camera_simu.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,22 +15,22 @@
 
     def __init__(self, name='simulate'):
         """Initialize camera module."""
         super().__init__()
 
         self.name = name
 
-        self.establishConnection()
+        self.establish_connection()
 
         self.load_defaults()
 
-        msg = f'Camera {self.getName()} initialized'
+        msg = f'Camera {self.get_name()} initialized'
         logger.info(msg)
 
-        atexit.register(self.releaseConnection)
+        atexit.register(self.release_connection)
 
         # EMMENU variables
         self._image_index = 0
         self._exposure = self.default_exposure
         self._autoincrement = True
         self._start_record_time = -1
 
@@ -38,87 +38,111 @@
         if self.name != config.settings.camera:
             config.load_camera_config(camera_name=self.name)
 
         self.streamable = True
 
         self.__dict__.update(config.camera.mapping)
 
-    def getImage(self, exposure=None, binsize=None, **kwargs) -> np.ndarray:
+    def get_image(self, exposure=None, binsize=None, **kwargs) -> np.ndarray:
         """Image acquisition routine. If the exposure and binsize are not
         given, the default values are read from the config file.
 
-        exposure:
+        Parameters
+        ----------
+        exposure : float
             Exposure time in seconds.
-        binsize:
+        binsize : int
             Which binning to use.
-        """
 
+        Returns
+        -------
+        arr : np.ndarray
+        """
         if exposure is None:
             exposure = self.default_exposure
         if not binsize:
             binsize = self.default_binsize
 
-        dim_x, dim_y = self.getCameraDimensions()
+        dim_x, dim_y = self.get_camera_dimensions()
 
         dim_x = int(dim_x / binsize)
         dim_y = int(dim_y / binsize)
 
         time.sleep(exposure)
 
         arr = np.random.randint(256, size=(dim_x, dim_y))
 
         return arr
 
-    def acquireImage(self) -> int:
+    def get_movie(self, n_frames, *, exposure: float = None, binsize: int = None, **kwargs):
+        """"Movie acquisition routine. If the exposure and binsize are not
+        given, the default values are read from the config file.
+
+        Parameters
+        ----------
+        n_frames : int
+            Number of frames to collect
+        exposure : float
+            Exposure time in seconds.
+        binsize : int
+            Which binning to use.
+
+        Returns
+        -------
+        stack : List[np.ndarray]
+        """
+        return [self.get_image(exposure=exposure, binsize=binsize) for _ in range(n_frames)]
+
+    def acquire_image(self) -> int:
         """For TVIPS compatibility."""
         return 1
 
-    def isCameraInfoAvailable(self) -> bool:
+    def is_camera_info_available(self) -> bool:
         """Check if the camera is available."""
         return True
 
-    def getImageDimensions(self) -> (int, int):
+    def get_image_dimensions(self) -> (int, int):
         """Get the binned dimensions reported by the camera."""
-        binning = self.getBinning()
-        dim_x, dim_y = self.getCameraDimensions()
+        binning = self.get_binning()
+        dim_x, dim_y = self.get_camera_dimensions()
 
         dim_x = int(dim_x / binning)
         dim_y = int(dim_y / binning)
 
         return dim_x, dim_y
 
-    def getCameraDimensions(self) -> (int, int):
+    def get_camera_dimensions(self) -> (int, int):
         """Get the dimensions reported by the camera."""
         return self.dimensions
 
-    def getName(self) -> str:
+    def get_name(self) -> str:
         """Get the name reported by the camera."""
         return self.name
 
-    def establishConnection(self) -> None:
+    def establish_connection(self) -> None:
         """Establish connection to the camera."""
         res = 1
         if res != 1:
             raise RuntimeError(f'Could not establish camera connection to {self.name}')
 
-    def releaseConnection(self) -> None:
+    def release_connection(self) -> None:
         """Release the connection to the camera."""
-        name = self.getName()
+        name = self.get_name()
         msg = f"Connection to camera '{name}' released"
         logger.info(msg)
 
     # Mimic EMMENU API
 
-    def getEMMenuVersion(self) -> str:
+    def get_emmenu_version(self) -> str:
         return 'simu'
 
-    def getCameraType(self) -> str:
+    def get_camera_type(self) -> str:
         return 'SimuType'
 
-    def getCurrentConfigName(self) -> str:
+    def get_current_config_name(self) -> str:
         return 'SimuCfg'
 
     def set_autoincrement(self, value):
         self._autoincrement = value
 
     def get_autoincrement(self):
         return self._autoincrement
@@ -157,12 +181,12 @@
 
     def get_exposure(self) -> int:
         return self._exposure
 
     def get_timestamps(self, start_index, end_index):
         return list(range(20))
 
-    def getBinning(self):
+    def get_binning(self):
         return self.default_binsize
 
-    def writeTiffs(self, start_index: int, stop_index: int, path: str, clear_buffer=True) -> None:
+    def write_tiffs(self, start_index: int, stop_index: int, path: str, clear_buffer=True) -> None:
         pass
```

### Comparing `instamatic-1.9.0/instamatic/camera/camera_timepix.py` & `instamatic-2.0.0/src/instamatic/camera/camera_timepix.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 CONFIG_PYTIMEPIX = 'tpx'
 
 
 class LockingError(RuntimeError):
     pass
 
 
-def arrangeData(raw, out=None):
+def arrange_data(raw, out=None):
     """10000 loops, best of 3: 81.3 s per loop."""
     s = 256 * 256
     q1 = raw[0:s].reshape(256, 256)
     q2 = raw[s:2 * s].reshape(256, 256)
     q3 = raw[2 * s:3 * s][::-1].reshape(256, 256)
     q4 = raw[3 * s:4 * s][::-1].reshape(256, 256)
 
@@ -37,15 +37,15 @@
     out[0:256, 260:516] = q2
     out[260:516, 0:256] = q4
     out[260:516, 260:516] = q3
 
     return out
 
 
-def correctCross(raw, factor=2.15):
+def correct_cross(raw, factor=2.15):
     """100000 loops, best of 3: 18 us per loop."""
     raw[255:258] = raw[255] / factor
     raw[:, 255:258] = raw[:, 255:256] / factor
 
     raw[258:261] = raw[260] / factor
     raw[:, 258:261] = raw[:, 260:261] / factor
 
@@ -69,15 +69,15 @@
         self.lib.EMCameraObj_Disconnect.restype = c_bool
         self.lib.EMCameraObj_timerExpired.restype = c_bool
 
         self.obj = self.lib.EMCameraObj_new()
         atexit.register(self.disconnect)
         self.is_connected = None
 
-        self.name = self.getName()
+        self.name = self.get_name()
         self.load_defaults()
 
     def acquire_lock(self):
         try:
             os.rename(self.lockfile, self.lockfile)
             # WinError 32 if file is open by the same/another process
         except PermissionError:
@@ -114,18 +114,18 @@
         if ret:
             self.is_connected = False
             print('Camera disconnected')
         else:
             print('Camera disconnect failed...')
         return ret
 
-    def getFrameSize(self):
+    def get_frame_size(self):
         return self.lib.EMCameraObj_getFrameSize(self.obj)
 
-    def readRealDacs(self, filename):
+    def read_real_dacs(self, filename):
         """std::string filename."""
         if not os.path.exists(filename):
             raise OSError(f'Cannot find `RealDacs` file: {filename}')
 
         filename = str(filename).encode()
         buffer = create_string_buffer(filename)
         # print buffer.value, len(buffer), buffer
@@ -133,15 +133,15 @@
         try:
             self.lib.EMCameraObj_readRealDacs(self.obj, buffer)
         except BaseException:
             traceback.print_exc()
             self.disconnect()
             sys.exit()
 
-    def readHwDacs(self, filename):
+    def read_hw_dacs(self, filename):
         """std::string filename."""
         if not os.path.exists(filename):
             raise OSError(f'Cannot find `HwDacs` file: {filename}')
 
         filename = str(filename).encode()
         buffer = create_string_buffer(filename)
         # print buffer.value, len(buffer), buffer
@@ -149,15 +149,15 @@
         try:
             self.lib.EMCameraObj_readHwDacs(self.obj, buffer)
         except BaseException:
             traceback.print_exc()
             self.disconnect()
             sys.exit()
 
-    def readPixelsCfg(self, filename):
+    def read_pixels_cfg(self, filename):
         """std::string filename."""
         'int mode = TPX_MODE_DONT_SET  ->  set in header file'
         if not os.path.exists(filename):
             raise OSError(f'Cannot find `PixelsCfg` file: {filename}')
 
         filename = str(filename).encode()
         buffer = create_string_buffer(filename)
@@ -166,58 +166,58 @@
         try:
             self.lib.EMCameraObj_readPixelsCfg(self.obj, buffer)
         except BaseException:
             traceback.print_exc()
             self.disconnect()
             sys.exit()
 
-    def processRealDac(self, chipnr=None, index=None, key=None, value=None):
+    def process_real_dac(self, chipnr=None, index=None, key=None, value=None):
         """int *chipnr."""
         'int *index'
         'std::string *key'
         'std::string *value'
 
         chipnr = c_int(0)
         index = c_int(0)
         key = create_unicode_buffer(20)
         value = create_unicode_buffer(20)
 
         self.lib.EMCameraObj_processRealDac(self.obj, byref(chipnr), byref(index), key, value)
 
-    def processHwDac(self, key, value):
+    def process_hw_dac(self, key, value):
         """std::string *key."""
         'std::string *value'
 
         key = create_unicode_buffer(20)
         value = create_unicode_buffer(20)
         self.lib.EMCameraObj_processHwDac(self.obj, byref(key), byref(value))
 
-    def startAcquisition(self):
-        """Equivalent to openShutteR?"""
+    def start_acquisition(self):
+        """Equivalent to openShutter?"""
         self.lib.EMCameraObj_startAcquisition(self.obj)
 
-    def stopAcquisition(self):
-        """Equivalent to closeShutter?"""
+    def stop_acquisition(self):
+        """Equivalent to close_shutter?"""
         self.lib.EMCameraObj_stopAcquisition(self.obj)
 
-    def openShutter(self):
+    def open_shutter(self):
         """Opens the Relaxd shutter under software control.
 
         Note that opening and closing the shutter under software control
         does not give a good control over the timing and should only be
         used for debugging or very long exposures where timing is less
         important.
         """
         self.lib.EMCameraObj_openShutter(self.obj)
 
-    def closeShutter(self):
+    def close_shutter(self):
         """Closes shutter under software control."""
         self.lib.EMCameraObj_closeShutter(self.obj)
 
-    def readMatrix(self, arr=None, sz=512 * 512):
+    def read_matrix(self, arr=None, sz=512 * 512):
         """Reads a frame from all connected devices, decodes the data and
         stores the pixel counts in array data.
 
         i16 *data # data storage array u32 sz    # size of array
         """
         if arr is None:
             arr = np.empty(sz, dtype=np.int16)
@@ -227,77 +227,77 @@
 
         # readout speed
         # 100 loops, best of 3: 7.52 ms per loop
         self.lib.EMCameraObj_readMatrix(self.obj, byref(ref), sz)
 
         return arr
 
-    def enableTimer(self, enable, us):
+    def enable_timer(self, enable, us):
         """Disables (enable is false) or enables the timer and sets the timer
         time-out to us microseconds. Note that the timer resolution is 10 us.
         After the Relaxd shutter opens (either explicitly by software or by an
         external trigger), it closes again after the set time.
 
         bool enable
         int us = 10 # microseconds
         """
         enable = c_bool(enable)
         us = c_int(us)
 
         self.lib.EMCameraObj_enableTimer(self.obj, enable, us)
 
-    def resetMatrix(self):
+    def reset_matrix(self):
         self.lib.EMCameraObj_resetMatrix(self.obj)
 
-    def timerExpired(self):
+    def timer_expired(self):
         return self.lib.EMCameraObj_timerExpired(self.obj)
 
-    def setAcqPars(self, pars):
+    def set_acq_pars(self, pars):
         """AcqParams *pars."""
         raise NotImplementedError
         pars = AcqParams
         self.lib.EMCameraObj_setAcqPars(self.obj, byref(pars))
 
-    def isBusy(self, busy):
+    def is_busy(self, busy):
         """bool *busy."""
         busy = c_bool(busy)
         self.lib.EMCameraObj_isBusy(self.obj, byref(busy))
 
-    def acquireData(self, exposure=0.001):
+    def acquire_data(self, exposure=0.001):
         microseconds = int(exposure * 1e6)  # seconds to microseconds
-        self.enableTimer(True, microseconds)
+        self.enable_timer(True, microseconds)
 
-        self.openShutter()
+        self.open_shutter()
 
         # sleep here to avoid burning cycles
         # only sleep if exposure is longer than Windows timer resolution, i.e. 1 ms
         if exposure > 0.001:
             time.sleep(exposure - 0.001)
 
-        while not self.timerExpired():
+        while not self.timer_expired():
             pass
 
-        # self.closeShutter()
+        # self.close_shutter()
 
-        arr = self.readMatrix()
+        arr = self.read_matrix()
 
-        out = arrangeData(arr)
-        correctCross(out, factor=self.correction_ratio)
+        out = arrange_data(arr)
+        correct_cross(out, factor=self.correction_ratio)
 
         out = np.rot90(out, k=3)
 
         return out
 
-    def getImage(self, exposure):
-        return self.acquireData(exposure=exposure)
+    def get_image(self, exposure):
+        return self.acquire_data(exposure=exposure)
 
-    def getName(self):
+    def get_name(self):
         return 'timepix'
 
-    def getCameraDimensions(self) -> (int, int):
+    def get_camera_dimensions(self) -> (int, int):
         return self.dimensions
 
     def load_defaults(self):
         if self.name != config.settings.camera:
             config.load_camera_config(camera_name=self.name)
 
         self.__dict__.update(config.camera.mapping)
@@ -324,19 +324,19 @@
                 pixelsCfg = base / inp[1]
 
     cam = CameraTPX(name=name)
     cam.connect(hwId)
 
     cam.init()
 
-    cam.readHwDacs(hwDacs)
-    cam.readPixelsCfg(pixelsCfg)
-    cam.readRealDacs(realDacs)
+    cam.read_hw_dacs(hwDacs)
+    cam.read_pixels_cfg(pixelsCfg)
+    cam.read_real_dacs(realDacs)
 
-    print(f'Camera {cam.getName()} initialized (resolution: {cam.getCameraDimensions()})')
+    print(f'Camera {cam.get_name()} initialized (resolution: {cam.get_camera_dimensions()})')
 
     return cam
 
 
 if __name__ == '__main__':
     from IPython import embed
 
@@ -355,18 +355,18 @@
 
     cam = initialize(tpx_config_file)
 
     if True:
         t = 0.01
         n = 100
 
-        arr = cam.acquireData(t)
+        arr = cam.acquire_data(t)
         print(f'[ py hardware timer] -> shape: {arr.shape}')
         t0 = time.perf_counter()
         for x in range(n):
-            cam.acquireData(t)
+            cam.acquire_data(t)
         dt = time.perf_counter() - t0
         print(f'Total time: {dt:.1f} s, acquisition time: {1000*(dt/n):.2f} ms, overhead: {1000*(dt/n - t):.2f} ms')
 
     embed(banner1='')
 
     isDisconnected = cam.disconnect()
```

### Comparing `instamatic-1.9.0/instamatic/camera/fakevideostream.py` & `instamatic-2.0.0/src/instamatic/camera/fakevideostream.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,16 +42,16 @@
         except AttributeError as e:
             reraise_on_fail = e
             try:
                 return getattr(self.cam, attrname)
             except AttributeError:
                 raise reraise_on_fail
 
-    def getImage(self, exposure=None, binsize=None):
-        frame = self.cam.getImage(exposure=exposure, binsize=binsize)
+    def get_image(self, exposure=None, binsize=None):
+        frame = self.cam.get_image(exposure=exposure, binsize=binsize)
 
         self.frame, scale = autoscale(frame, maxdim=self.display_dim)
 
         return frame
 
     def update_frametime(self, frametime):
         self.frametime = frametime
@@ -83,15 +83,15 @@
         go_on = True
         i = 0
 
         self.block()
         while go_on:
             i += 1
 
-            img = self.getImage(exposure=exposure)
+            img = self.get_image(exposure=exposure)
 
             if callback:
                 go_on = callback(img)
             else:
                 buffer.append(img)
                 go_on = i < n
```

### Comparing `instamatic-1.9.0/instamatic/camera/gatansocket3.md` & `instamatic-2.0.0/src/instamatic/camera/gatansocket3.md`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/camera/gatansocket3.py` & `instamatic-2.0.0/src/instamatic/camera/gatansocket3.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,15 +122,15 @@
         """Serialize the data."""
         data_size = self.array.data.itemsize
         if self.array.data.itemsize > ARGS_BUFFER_SIZE:
             raise RuntimeError(f'Message packet size {data_size} is larger than maximum {ARGS_BUFFER_SIZE}')
         return self.array.data
 
     def unpack(self, buf):
-        """unpack buffer into our data structure."""
+        """Unpack buffer into our data structure."""
         self.array = np.frombuffer(buf, dtype=self.dtype)[0]
 
 
 def log(message):
     global debug_log
     if debug_log is None:
         return
```

### Comparing `instamatic-1.9.0/instamatic/camera/merlin_io.py` & `instamatic-2.0.0/src/instamatic/camera/merlin_io.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,16 +89,22 @@
     @classmethod
     def from_buffer(cls, buffer: bytes):
         """Return MIB properties from buffer."""
         head = buffer[:384].decode().split(',')
         return cls(head)
 
 
-def load_mib(buffer: bytes):
-    """Load Quantum Detectors MIB file from a memory buffer."""
+def load_mib(buffer: bytes, skip: int = 0):
+    """Load Quantum Detectors MIB file from a memory buffer.
+
+    skip : int, optional
+        Skip first n bytes.
+    """
+    buffer = buffer[skip:]
+
     assert isinstance(buffer, (bytes, bytearray))
 
     props = MIBProperties.from_buffer(buffer)
 
     merlin_frame_dtype = np.dtype([
         ('header', np.string_, props.headsize),
         ('data', props.pixeltype, props.merlin_size),
```

### Comparing `instamatic-1.9.0/instamatic/camera/mpxhwrelaxd.dll` & `instamatic-2.0.0/src/instamatic/camera/mpxhwrelaxd.dll`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/camera/tpx/171207_with_flatfield.bpc` & `instamatic-2.0.0/src/instamatic/camera/tpx/171207_with_flatfield.bpc`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/camera/tpx/171207_with_flatfield.bpc.dacs` & `instamatic-2.0.0/src/instamatic/camera/tpx/171207_with_flatfield.bpc.dacs`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/camera/videostream.py` & `instamatic-2.0.0/src/instamatic/camera/videostream.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,19 +45,19 @@
 
     def run(self):
         while not self.stopEvent.is_set():
 
             if self.acquireInitiateEvent.is_set():
                 self.acquireInitiateEvent.clear()
 
-                frame = self.cam.getImage(exposure=self.exposure, binsize=self.binsize)
+                frame = self.cam.get_image(exposure=self.exposure, binsize=self.binsize)
                 self.callback(frame, acquire=True)
 
             elif not self.continuousCollectionEvent.is_set():
-                frame = self.cam.getImage(exposure=self.frametime, binsize=self.binsize)
+                frame = self.cam.get_image(exposure=self.frametime, binsize=self.binsize)
                 self.callback(frame)
 
     def start_loop(self):
         self.thread = threading.Thread(target=self.run, args=(), daemon=True)
         self.thread.start()
 
     def stop(self):
@@ -118,15 +118,15 @@
             self.grabber.lock.release()
 
     def setup_grabber(self):
         grabber = ImageGrabber(self.cam, callback=self.send_frame, frametime=self.frametime)
         atexit.register(grabber.stop)
         return grabber
 
-    def getImage(self, exposure=None, binsize=None):
+    def get_image(self, exposure=None, binsize=None):
         current_frametime = self.grabber.frametime
 
         # set to 0 to prevent it lagging data acquisition
         self.grabber.frametime = 0
         if exposure:
             self.grabber.exposure = exposure
         if binsize:
@@ -175,15 +175,15 @@
         go_on = True
         i = 0
 
         self.block()
         while go_on:
             i += 1
 
-            img = self.getImage(exposure=exposure)
+            img = self.get_image(exposure=exposure)
 
             if callback:
                 go_on = callback(img)
             else:
                 buffer.append(img)
                 go_on = i < n
```

### Comparing `instamatic-1.9.0/instamatic/config/__init__.py` & `instamatic-2.0.0/src/instamatic/config/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -268,18 +268,18 @@
 
 locations = {
     'base': base_drc,
     'config': config_drc,
     'logs': logs_drc,
     'scripts': scripts_drc,
     'camera': alignments_drc,
-    'microscope': calibration.location.parent,
-    'calibration': microscope.location.parent,
+    'calibration': calibration.location.parent,
+    'microscope': microscope.location.parent,
     'alignments': camera.location.parent,
     'data': settings.data_directory,
     'work': settings.work_directory,
-    'microscope_config': calibration.location,
-    'calibration_config': microscope.location,
+    'calibration_config': calibration.location,
+    'microscope_config': microscope.location,
     'alignments_config': camera.location,
     'settings': config_drc / _settings_yaml,
     'defaults': config_drc / _defaults_yaml,
 }
```

### Comparing `instamatic-1.9.0/instamatic/config/autoconfig.py` & `instamatic-2.0.0/src/instamatic/config/autoconfig.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,25 +10,25 @@
 def get_tvips_calibs(ctrl, rng: list, mode: str, wavelength: float) -> dict:
     """Loop over magnification ranges and return calibrations from EMMENU."""
     if mode == 'diff':
         print('Warning: Pixelsize can be a factor 10 off in diff mode (bug in EMMENU)')
 
     calib_range = {}
 
-    binning = ctrl.cam.getBinning()
+    binning = ctrl.cam.get_binning()
 
     ctrl.mode.set(mode)
 
     for i, mag in enumerate(rng):
         ctrl.magnification.index = i
-        d = ctrl.cam.getCurrentCameraInfo()
+        d = ctrl.cam.get_current_camera_info()
 
         img = ctrl.get_image(exposure=10)  # set to minimum allowed value
         index = ctrl.cam.get_image_index()
-        v = ctrl.cam.getEMVectorByIndex(index)
+        v = ctrl.cam.get_emvector_by_index(index)
 
         PixelSizeX = v['fImgDistX']
         PixelSizeY = v['fImgDistY']
 
         assert PixelSizeX == PixelSizeY, 'Pixelsizes differ in X and Y direction?! (X: {PixelSizeX} | Y: {PixelSizeY})'
 
         if mode == 'diff':
@@ -83,41 +83,50 @@
         description=description,
         formatter_class=argparse.RawDescriptionHelpFormatter)
 
     options = parser.parse_args()
 
     # Connect to microscope
 
-    tem_name = choice_prompt(choices='jeol fei simulate'.split(),
+    tem_name = choice_prompt(choices=['jeol', 'fei', 'simulate'],
                              default='simulate',
                              question='Which microscope can I connect to?')
 
-    # Connect to camera
-
-    cam_name = choice_prompt(choices=[None, 'gatan', 'tvips', 'simulate'],
-                             default='simulate',
-                             question='Which camera can I connect to?')
-
     # Fetch camera config
 
     drc = Path(__file__).parent
     choices = list(drc.glob('camera/*.yaml'))
     choices.append(None)
 
     cam_config = choice_prompt(choices=choices,
                                default=None,
                                question='Which camera type do you want to use (select closest one and modify if needed)?')
 
-    # Instantiate microscope / camera connection
+    if cam_config:
+        with open(cam_config) as f:
+            cam_config_dict = yaml.safe_load(f)
+            cam_name = cam_config_dict['interface']
+
+            cam_connect = input(
+                f'\nShould I connect to `{cam_name}` immediately?'
+                '\nThis is usually OK for gatan/simulate/TVIPS. [y/N] >> ',
+            ) == 'y'
+    else:
+        cam_connect = False
+        cam_name = None
 
     from instamatic.camera.camera import get_cam
     from instamatic.TEMController.microscope import get_tem
     from instamatic.TEMController.TEMController import TEMController
 
-    cam = get_cam(cam_name)() if cam_name else None
+    if cam_connect:
+        cam = get_cam(cam_name)() if cam_name else None
+    else:
+        cam = None
+
     tem = get_tem(tem_name)()
 
     ctrl = TEMController(tem=tem, cam=cam)
 
     try:
         ranges = ctrl.magnification.get_ranges()
     except BaseException:
@@ -178,14 +187,16 @@
     print()
     print(f'In `{settings_yaml}`:')
     print(f'    microscope: {tem_name}_tem')
     print(f'    calibration: {tem_name}_calib')
     if cam_config:
         print(f'    camera: {cam_name}_cam')
     print()
-    print(f'Todo: Check and update the pixelsizes in `{calib_config_fn}`')
-    print('    In real space, pixelsize in nm')
-    print('    In reciprocal space, pixelsize in px/Angstrom')
+    print('Todo:')
+    print(f' 1. Check and update the pixelsizes in `{calib_config_fn}`')
+    print('    - In real space, pixelsize in nm')
+    print('    - In reciprocal space, pixelsize in px/Angstrom')
+    print(f' 2. Check and update magnification ranges in `{microscope_config_fn}`')
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `instamatic-1.9.0/instamatic/config/calibration/orius.yaml` & `instamatic-2.0.0/src/instamatic/config/calibration/orius.yaml`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/config/calibration/simulate.yaml` & `instamatic-2.0.0/tests/config/calibration/test.yaml`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/config/calibration/timepix.yaml` & `instamatic-2.0.0/src/instamatic/config/calibration/timepix.yaml`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/config/calibration/tvips-f416.yaml` & `instamatic-2.0.0/src/instamatic/config/calibration/tvips-f416.yaml`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/config/camera/serval.yaml` & `instamatic-2.0.0/src/instamatic/config/camera/serval.yaml`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/config/config_updater.py` & `instamatic-2.0.0/src/instamatic/config/config_updater.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
 
 if __name__ == '__main__':
 
     class config:
         def __init__(self, fn):
             self.fn = fn
-            self.mapping = yaml.full_load(open(fn, 'r'))
+            self.mapping = yaml.full_load(open(fn))
             self.name = self.fn.parent.name
 
         def update(self):
             convert_config(self.fn, kind=self.name)
 
         @property
         def is_oldstyle(self):
```

### Comparing `instamatic-1.9.0/instamatic/config/microscope/fei_simu.yaml` & `instamatic-2.0.0/src/instamatic/config/microscope/jeol.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-interface: fei_simu
+interface: jeol
 ranges:
   diff: [150, 200, 250, 300, 400, 500, 600, 800, 1000, 1200, 1500, 2000, 2500, 3000,
     3500, 4000, 4500]
   lowmag: [50, 80, 100, 150, 200, 250, 300, 400, 500, 600, 800, 1000, 1200, 1500,
     2000, 2500, 3000, 5000, 6000, 8000, 10000, 12000, 15000]
   mag1: [2500, 3000, 4000, 5000, 6000, 8000, 10000, 12000, 15000, 20000, 25000, 30000,
     40000, 50000, 60000, 80000, 100000, 120000, 150000, 200000, 250000, 300000, 400000,
     500000, 600000, 800000, 1000000, 1500000, 2000000]
-wavelength: 0.019687
+wavelength: 0.025079
```

### Comparing `instamatic-1.9.0/instamatic/config/microscope/fei_themisZ.yaml` & `instamatic-2.0.0/src/instamatic/config/microscope/simulate.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-interface: fei
+interface: simulate
 ranges:
   diff: [150, 200, 250, 300, 400, 500, 600, 800, 1000, 1200, 1500, 2000, 2500, 3000,
     3500, 4000, 4500]
   lowmag: [50, 80, 100, 150, 200, 250, 300, 400, 500, 600, 800, 1000, 1200, 1500,
     2000, 2500, 3000, 5000, 6000, 8000, 10000, 12000, 15000]
   mag1: [2500, 3000, 4000, 5000, 6000, 8000, 10000, 12000, 15000, 20000, 25000, 30000,
     40000, 50000, 60000, 80000, 100000, 120000, 150000, 200000, 250000, 300000, 400000,
     500000, 600000, 800000, 1000000, 1500000, 2000000]
-wavelength: 0.019687
+wavelength: 0.025079
```

### Comparing `instamatic-1.9.0/instamatic/config/microscope/jeol-1400.yaml` & `instamatic-2.0.0/src/instamatic/config/microscope/jeol-1400.yaml`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/config/microscope/jeol.yaml` & `instamatic-2.0.0/tests/config/microscope/test.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-interface: jeol
+interface: simulate
 ranges:
   diff: [150, 200, 250, 300, 400, 500, 600, 800, 1000, 1200, 1500, 2000, 2500, 3000,
     3500, 4000, 4500]
   lowmag: [50, 80, 100, 150, 200, 250, 300, 400, 500, 600, 800, 1000, 1200, 1500,
     2000, 2500, 3000, 5000, 6000, 8000, 10000, 12000, 15000]
   mag1: [2500, 3000, 4000, 5000, 6000, 8000, 10000, 12000, 15000, 20000, 25000, 30000,
     40000, 50000, 60000, 80000, 100000, 120000, 150000, 200000, 250000, 300000, 400000,
```

### Comparing `instamatic-1.9.0/instamatic/config/scripts/readme.md` & `instamatic-2.0.0/src/instamatic/config/scripts/readme.md`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/config/settings.yaml` & `instamatic-2.0.0/src/instamatic/config/settings.yaml`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/config/utils.py` & `instamatic-2.0.0/src/instamatic/config/utils.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/exceptions.py` & `instamatic-2.0.0/src/instamatic/exceptions.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/experiments/autocred/experiment.py` & `instamatic-2.0.0/src/instamatic/experiments/autocred/experiment.py`

 * *Files 0% similar despite different names*

```diff
@@ -321,15 +321,15 @@
                         pass
 
                 img = np.delete(img, indy, 1)
 
             return np.var(img)
 
     def check_img_outsidebeam_byscale(self, img1_scale, img2_scale):
-        """img1 is the original image for reference, img2 is the new image."""
+        """`img1` is the original image for reference, `img2` is the new image."""
         if img2_scale / img1_scale < 0.5 or img2_scale / img1_scale > 2:
             return 1
         else:
             return 0
 
     def eliminate_backlash_in_tiltx(self):
         a_i = self.ctrl.stage.a
@@ -988,15 +988,15 @@
             return self.calib_beamshift.reference_pixel
         else:
             return self.calib_beamshift.reference_pixel
 
     def raster_scan(self):
         from instamatic.experiments.serialed.experiment import get_offsets_in_scan_area
         pixelsize_mag1 = config.calibration['mag1']['pixelsize'][self.magnification] / 1000  # nm -> um
-        xdim, ydim = self.ctrl.getCameraDimensions()
+        xdim, ydim = self.ctrl.cam.get_camera_dimensions()
         box_x, box_y = self.pixelsize_mag1 * xdim, self.pixelsize_mag1 * ydim
 
         # Make negative to reflect config change 2019-07-03 to make omega more in line with other software
         rot_axis = -config.camera.camera_rotation_vs_stage_xy
 
         offsets = get_offsets_in_scan_area(box_x, box_y, self.scan_area, angle=rot_axis)
         self.offsets = offsets * 1000
```

### Comparing `instamatic-1.9.0/instamatic/experiments/cred/experiment.py` & `instamatic-2.0.0/src/instamatic/experiments/cred/experiment.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/experiments/cred_gatan/experiment.py` & `instamatic-2.0.0/src/instamatic/experiments/cred_gatan/experiment.py`

 * *Files 0% similar despite different names*

```diff
@@ -328,18 +328,18 @@
         print('Start stage position:  X {:6.0f} | Y {:6.0f} | Z {:6.0f} | A {:6.1f} | B {:6.1f}'.format(*self.start_position))
         print('End stage position:    X {:6.0f} | Y {:6.0f} | Z {:6.0f} | A {:6.1f} | B {:6.1f}'.format(*self.end_position))
         print(f'Data collection camera length: {self.camera_length} cm')
         print(f'Data collection spot size: {self.spotsize}')
         print(f'Rotation speed: {self.rotation_speed:.3f} degrees/s')
 
         with open(self.path / 'cRED_log.txt', 'w') as f:
-            print(f'Program: {instamatic.__long_title__} + GMS {self.cam.getDMVersion()}', file=f)
+            print(f'Program: {instamatic.__long_title__} + GMS {self.cam.get_dm_version()}', file=f)
             print(f'Camera: {config.camera.name}', file=f)
             print(f'Microscope: {config.microscope.name}', file=f)
-            # print(f"Camera type: {self.cam.getCameraType()}", file=f)
+            # print(f"Camera type: {self.cam.get_camera_type()}", file=f)
             print(f'Mode: {self.mode}', file=f)
             print(f'Data Collection Time: {self.now}', file=f)
             print(f'Time Period Start: {self.t_start}', file=f)
             print(f'Time Period End: {self.t_end}', file=f)
             print(f'Number of frames: {self.nframes}', file=f)
             print(f'Starting angle: {self.start_angle:.2f} degrees', file=f)
             print(f'Ending angle: {self.end_angle:.2f} degrees', file=f)
```

### Comparing `instamatic-1.9.0/instamatic/experiments/cred_tvips/experiment.py` & `instamatic-2.0.0/src/instamatic/experiments/cred_tvips/experiment.py`

 * *Files 1% similar despite different names*

```diff
@@ -278,18 +278,16 @@
             a = self.ctrl.stage.a
 
         print('Rotation started...')
 
         return a
 
     def start_collection(self, target_angle: float, start_angle: float = None, manual_control: bool = False):
-        """
-        manual_control : bool
-            Control the rotation using the buttons or pedals
-        """
+        """manual_control : bool Control the rotation using the buttons or
+        pedals."""
         angle_tolerance = 0.5  # degrees
 
         self.now = datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')
 
         self.stage_positions = []
         interval = 0.7  # interval at which it check for rotation to end / does tracking
 
@@ -428,15 +426,15 @@
         self.log_end_status()
         self.log_stage_positions()
 
         print('Writing data files...')
         path_data = self.path / 'tiff'
         path_data.mkdir(exist_ok=True, parents=True)
 
-        self.emmenu.writeTiffs(start_index, end_index, path=path_data)
+        self.emmenu.write_tiffs(start_index, end_index, path=path_data)
 
         if self.track:
             # Center crystal position
             if self.mode == 'diff':
                 self.ctrl.difffocus.defocus(self.defocus_offset)
             self.ctrl.beam.unblank()
 
@@ -461,34 +459,34 @@
             pixelsize = config.calibration['diff']['pixelsize'][self.camera_length]  # px / Angstrom
         except KeyError:
             print(f'Warning: No such camera length: {self.camera_length} in diff calibration, defaulting to 1.0')
             pixelsize = 1.0
 
         physical_pixelsize = config.camera.physical_pixelsize  # mm
 
-        binning = self.emmenu.getBinning()
-        image_dimensions_x, image_dimensions_y = self.emmenu.getImageDimensions()
-        camera_dimensions_x, camera_dimensions_y = self.emmenu.getCameraDimensions()
+        binning = self.emmenu.get_binning()
+        image_dimensions_x, image_dimensions_y = self.emmenu.get_image_dimensions()
+        camera_dimensions_x, camera_dimensions_y = self.emmenu.get_camera_dimensions()
 
         pixelsize *= binning
         physical_pixelsize *= binning
 
         print(f'\nRotated {self.total_angle:.2f} degrees from {self.start_angle:.2f} to {self.end_angle:.2f}')
         print('Start stage position:  X {:6.0f} | Y {:6.0f} | Z {:6.0f} | A {:6.1f} | B {:6.1f}'.format(*self.start_position))
         print('End stage position:    X {:6.0f} | Y {:6.0f} | Z {:6.0f} | A {:6.1f} | B {:6.1f}'.format(*self.end_position))
         print(f'Data collection camera length: {self.camera_length} cm')
         print(f'Data collection spot size: {self.spotsize}')
         print(f'Rotation speed: {self.rotation_speed:.3f} degrees/s')
 
         with open(self.path / 'cRED_log.txt', 'w') as f:
-            print(f'Program: {instamatic.__long_title__} + EMMenu {self.emmenu.getEMMenuVersion()}', file=f)
+            print(f'Program: {instamatic.__long_title__} + EMMenu {self.emmenu.get_emmenu_version()}', file=f)
             print(f'Camera: {config.camera.name}', file=f)
             print(f'Microscope: {config.microscope.name}', file=f)
-            print(f'Camera type: {self.emmenu.getCameraType()}', file=f)
-            print(f'Camera config: {self.emmenu.getCurrentConfigName()}', file=f)
+            print(f'Camera type: {self.emmenu.get_camera_type()}', file=f)
+            print(f'Camera config: {self.emmenu.get_current_config_name()}', file=f)
             print(f'Mode: {self.mode}', file=f)
             print(f'Data Collection Time: {self.now}', file=f)
             print(f'Time Period Start: {self.t_start}', file=f)
             print(f'Time Period End: {self.t_end}', file=f)
             print(f'Number of frames: {self.nframes}', file=f)
             print(f'Starting angle: {self.start_angle:.2f} degrees', file=f)
             print(f'Ending angle: {self.end_angle:.2f} degrees', file=f)
```

### Comparing `instamatic-1.9.0/instamatic/experiments/red/experiment.py` & `instamatic-2.0.0/src/instamatic/experiments/red/experiment.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/experiments/serialed/experiment.py` & `instamatic-2.0.0/src/instamatic/experiments/serialed/experiment.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,15 +209,15 @@
 
             self.calib_beamshift = CalibBeamShift.live(self.ctrl, outdir=self.calibdir)
 
             self.magnification = self.ctrl.magnification.value
             self.log.info('Brightness=%s', self.ctrl.brightness)
 
         self.pixelsize_mag1 = config.calibration['mag1']['pixelsize'][self.magnification] / 1000  # nm -> um
-        xdim, ydim = self.ctrl.cam.getCameraDimensions()
+        xdim, ydim = self.ctrl.cam.get_camera_dimensions()
         self.image_dimensions = self.pixelsize_mag1 * xdim, self.pixelsize_mag1 * ydim
         self.log.info('Image dimensions %s', self.image_dimensions)
 
         self.diff_binsize = kwargs.get('diff_binsize', self.ctrl.cam.default_binsize)  # this also messes with calibrate_beamshift class
         self.diff_exposure = kwargs.get('diff_exposure', self.ctrl.cam.default_exposure)
         self.diff_spotsize = kwargs.get('diff_spotsize', 4)
         # self.diff_cameralength = kwargs.get("diff_cameralength",       800)
```

### Comparing `instamatic-1.9.0/instamatic/formats/__init__.py` & `instamatic-2.0.0/src/instamatic/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/formats/adscimage.py` & `instamatic-2.0.0/src/instamatic/formats/adscimage.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
     with open(fname, 'wb') as outf:
         outf.write(out)
         outf.write(data.tobytes())
 
 
 def readheader(infile):
-    """read an adsc header."""
+    """Read an adsc header."""
     header = {}
     line = infile.readline()
     bytesread = len(line)
     while b'}' not in line:
         string = line.decode().strip()
         if '=' in string:
             (key, val) = string.split('=')
@@ -64,15 +64,15 @@
             header[key] = val
         line = infile.readline()
         bytesread = bytesread + len(line)
     return header
 
 
 def read_adsc(fname: str) -> (np.array, dict):
-    """read in the file."""
+    """Read in the file."""
     with open(fname, 'rb', buffering=0) as infile:
         try:
             header = readheader(infile)
         except BaseException:
             raise Exception('Error processing adsc header')
         # banned by bzip/gzip???
         try:
```

### Comparing `instamatic-1.9.0/instamatic/formats/csvIO.py` & `instamatic-2.0.0/src/instamatic/formats/csvIO.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/formats/mrc.py` & `instamatic-2.0.0/src/instamatic/formats/mrc.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/formats/util.py` & `instamatic-2.0.0/src/instamatic/formats/util.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/formats/xdscbf.py` & `instamatic-2.0.0/src/instamatic/formats/xdscbf.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         start = stop + 1
     if start < delta.size:
         binary_blob += delta[start:].astype(np.int8).tobytes()
     return binary_blob
 
 
 def write(fname, data, header={}):
-    """write the file in CBF format.
+    """Write the file in CBF format.
 
     :param str fname: name of the file
     """
     if data is not None:
         dim2, dim1 = data.shape
     else:
         raise RuntimeError('CBF image contains no data')
```

### Comparing `instamatic-1.9.0/instamatic/goniotool.py` & `instamatic-2.0.0/src/instamatic/goniotool.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/gridmontage.py` & `instamatic-2.0.0/src/instamatic/gridmontage.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,17 +53,17 @@
             Stage coordinates for the montage acquisition
         """
         self.nx = nx
         self.ny = ny
         self.overlap = overlap
 
         if not binning:
-            binning = self.ctrl.cam.getBinning()
+            binning = self.ctrl.cam.get_binning()
 
-        res_x, res_y = self.ctrl.cam.getImageDimensions()
+        res_x, res_y = self.ctrl.cam.get_image_dimensions()
 
         overlap_x = int(res_x * overlap)
         overlap_y = int(res_y * overlap)
 
         vect = np.array((res_x - overlap_x, res_y - overlap_y))
 
         grid = make_grid((nx, ny), direction=self.direction, zigzag=self.zigzag)
```

### Comparing `instamatic-1.9.0/instamatic/gui/about_frame.py` & `instamatic-2.0.0/src/instamatic/gui/about_frame.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/gui/autocred_frame.py` & `instamatic-2.0.0/src/instamatic/gui/autocred_frame.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/gui/base_module.py` & `instamatic-2.0.0/src/instamatic/gui/base_module.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/gui/console_frame.py` & `instamatic-2.0.0/src/instamatic/gui/console_frame.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/gui/cred_fei_frame.py` & `instamatic-2.0.0/src/instamatic/gui/cred_fei_frame.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/gui/cred_frame.py` & `instamatic-2.0.0/src/instamatic/gui/cred_frame.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/gui/cred_tvips_frame.py` & `instamatic-2.0.0/src/instamatic/gui/cred_tvips_frame.py`

 * *Files 0% similar despite different names*

```diff
@@ -292,15 +292,15 @@
     def search(self):
         self.ctrl.run_script('search_mode.py')
 
     def focus(self):
         self.ctrl.run_script('focus_mode.py')
 
     def get_image(self):
-        self.ctrl.cam.acquireImage()
+        self.ctrl.cam.acquire_image()
 
 
 def acquire_data_CRED_TVIPS(controller, **kwargs):
     controller.log.info('Start cRED (TVIPS) experiment')
     from instamatic.experiments import cRED_tvips
 
     task = kwargs['task']
```

### Comparing `instamatic-1.9.0/instamatic/gui/ctrl_frame.py` & `instamatic-2.0.0/src/instamatic/gui/ctrl_frame.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/gui/debug_frame.py` & `instamatic-2.0.0/src/instamatic/gui/debug_frame.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/gui/defocus_button.py` & `instamatic-2.0.0/src/instamatic/gui/defocus_button.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/gui/gui.py` & `instamatic-2.0.0/src/instamatic/gui/gui.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/gui/io_frame.py` & `instamatic-2.0.0/src/instamatic/gui/io_frame.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/gui/jobs.py` & `instamatic-2.0.0/src/instamatic/gui/jobs.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/gui/machine_learning_frame.py` & `instamatic-2.0.0/src/instamatic/gui/machine_learning_frame.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/gui/modules.py` & `instamatic-2.0.0/src/instamatic/gui/modules.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/gui/mpl_frame.py` & `instamatic-2.0.0/src/instamatic/gui/mpl_frame.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/gui/red_frame.py` & `instamatic-2.0.0/src/instamatic/gui/red_frame.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/gui/sed_frame.py` & `instamatic-2.0.0/src/instamatic/gui/sed_frame.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/gui/videostream_frame.py` & `instamatic-2.0.0/src/instamatic/gui/videostream_frame.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/image_utils.py` & `instamatic-2.0.0/src/instamatic/image_utils.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/imreg.py` & `instamatic-2.0.0/src/instamatic/imreg.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/io.py` & `instamatic-2.0.0/src/instamatic/io.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/main.py` & `instamatic-2.0.0/src/instamatic/main.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/montage.py` & `instamatic-2.0.0/src/instamatic/montage.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/neural_network/neural_network.py` & `instamatic-2.0.0/src/instamatic/neural_network/neural_network.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/neural_network/preprocess.py` & `instamatic-2.0.0/src/instamatic/neural_network/preprocess.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/neural_network/preprocess_SerialRED.py` & `instamatic-2.0.0/src/instamatic/neural_network/preprocess_SerialRED.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/processing/ImgConversion.py` & `instamatic-2.0.0/src/instamatic/processing/ImgConversion.py`

 * *Files 0% similar despite different names*

```diff
@@ -695,9 +695,9 @@
         cx, cy = self.mean_beam_center
         with open(path / 'shifts.sc', 'w') as f:
             print(f' {cy:.2f} {cx:.2f}', file=f)  # cx/cy must be switched around, y first
             for i in self.observed_range:
                 print(f'{i:4d}{0:8.2f}{0:8.2f}', file=f)
 
     def add_beamstop(self, rect):
-        """rect must be a 2x4 coordinate array."""
+        """Rect must be a 2x4 coordinate array."""
         self.untrusted_areas.append(('quadrilateral', rect))
```

### Comparing `instamatic-1.9.0/instamatic/processing/ImgConversionDM.py` & `instamatic-2.0.0/src/instamatic/processing/ImgConversionDM.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/processing/ImgConversionTPX.py` & `instamatic-2.0.0/src/instamatic/processing/ImgConversionTPX.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/processing/ImgConversionTVIPS.py` & `instamatic-2.0.0/src/instamatic/processing/ImgConversionTVIPS.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/processing/XDS_template.py` & `instamatic-2.0.0/src/instamatic/processing/XDS_template.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/processing/XDS_templateDM.py` & `instamatic-2.0.0/src/instamatic/processing/XDS_templateDM.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/processing/XDS_templateTPX.py` & `instamatic-2.0.0/src/instamatic/processing/XDS_templateTPX.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/processing/XDS_templateTVIPS.py` & `instamatic-2.0.0/src/instamatic/processing/XDS_templateTVIPS.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/processing/find_crystals.py` & `instamatic-2.0.0/src/instamatic/processing/find_crystals.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/processing/find_crystals_ilastik.py` & `instamatic-2.0.0/src/instamatic/processing/find_crystals_ilastik.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/processing/find_holes.py` & `instamatic-2.0.0/src/instamatic/processing/find_holes.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/processing/flatfield.py` & `instamatic-2.0.0/src/instamatic/processing/flatfield.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/processing/stretch_correction.py` & `instamatic-2.0.0/src/instamatic/processing/stretch_correction.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/server/TEMServer_FEI.py` & `instamatic-2.0.0/src/instamatic/server/TEMServer_FEI.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Utility script to enable rotation control from a dmscript See
-`https://github.com/instamatic-dev/instamatic/tree/master/dmscript` for
+`https://github.com/instamatic-dev/InsteaDMatic` for
 usage."""
 import datetime
 import logging
 import subprocess as sp
 import threading
 from socket import *
 
@@ -42,15 +42,15 @@
     print('Rotation completed.')
 
 
 def main():
     import argparse
 
     description = """
-Utility script to enable rotation control from a dmscript. See [https://github.com/instamatic-dev/instamatic/tree/master/dmscript] for usage.
+Utility script to enable rotation control from a dmscript. See [https://github.com/instamatic-dev/InsteaDMatic] for usage.
 """
 
     parser = argparse.ArgumentParser(
         description=description,
         formatter_class=argparse.RawDescriptionHelpFormatter)
 
     options = parser.parse_args()
```

### Comparing `instamatic-1.9.0/instamatic/server/cam_server.py` & `instamatic-2.0.0/src/instamatic/server/cam_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,15 @@
                     traceback.print_exc()
                     if self.log:
                         self.log.exception(e)
                     ret = (e.__class__.__name__, e.args)
                     status = 500
                 else:
                     if self.use_shared_memory:
-                        if attr_name == 'getImage':
+                        if attr_name == 'get_image':
                             self.copy_data_to_shared_buffer(ret)
                             ret = {
                                 'shape': ret.shape,
                                 'dtype': str(ret.dtype),
                                 'name': self.shmem.name,
                             }
```

### Comparing `instamatic-1.9.0/instamatic/server/dials_server.py` & `instamatic-2.0.0/src/instamatic/server/dials_server.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/server/goniotool_server.py` & `instamatic-2.0.0/src/instamatic/server/goniotool_server.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/server/serializer.py` & `instamatic-2.0.0/src/instamatic/server/serializer.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/server/tem_server.py` & `instamatic-2.0.0/src/instamatic/server/tem_server.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/server/vm_ubuntu_server.py` & `instamatic-2.0.0/src/instamatic/server/vm_ubuntu_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 VM_DELAY2 = config.settings.VM_DESKTOP_DELAY
 VM_SF = config.settings.VM_SHARED_FOLDER
 # ENABLE_SHELXT = config.settings.ENABLE_SHELXT
 BUFF = 1024
 
 
 def start_vm_process(vmname=VM_ID, vmachine_pwd=VM_PWD, time_delay=VM_DELAY1, mode='headless'):
-    """mode can be either gui or headless."""
+    """Mode can be either gui or headless."""
     try:
         vbox = virtualbox.VirtualBox()
     except ModuleNotFoundError:
         print('Please install virtualbox with guest ubuntu and virtualbox SDK first before using this server.')
         print('Download virtualbox python SDK from:')
         print('https://www.virtualbox.org/wiki/Downloads')
 
@@ -44,15 +44,15 @@
     session.console.keyboard.put_keys(vmachine_pwd)
     session.console.keyboard.put_keys(['ENTER'])
     print('password delivered!')
     return session
 
 
 def vm_ubuntu_start_terminal(session):
-    """type ctrl+alt+t to bring up terminal in the ubuntu machine."""
+    """Type ctrl+alt+t to bring up terminal in the ubuntu machine."""
     session.console.keyboard.put_keys(press_keys='t', hold_keys=['CTRL', 'ALT'])
 
 
 def vm_ubuntu_execute_script(vmname=VM_ID, vmachine_username=VM_USERNAME, vmachine_pwd=VM_PWD, time_delay=30, script_path='/usr/loca/bin/xds'):
     try:
         vbox = virtualbox.VirtualBox()
     except ModuleNotFoundError:
@@ -68,15 +68,15 @@
     gs = session.console.guest.create_session(vmachine_username, vmachine_pwd)
 
     process, stdout, stderr = gs.execute(script_path)
     print(stdout)
 
 
 def vm_ubuntu_start_xds_AtFolder(session, conn, shelxt, unitcell, spgr, composition):
-    """incoming conn should contain a path that is shared already between VBox
+    """Incoming conn should contain a path that is shared already between VBox
     and windows."""
 
     # path = "/media/sf_SharedWithVM/test_vm_server"
 
     while True:
 
         try:
```

### Comparing `instamatic-1.9.0/instamatic/server/xds_server.py` & `instamatic-2.0.0/src/instamatic/server/xds_server.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/tools.py` & `instamatic-2.0.0/src/instamatic/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -200,15 +200,15 @@
         over = np.where(XY > (im_mean * treshold))[0]
         rads[n] = (over[-1] - over[0]) / 2
         center[n] = over[0] + rads[n]
     return center, rads
 
 
 def get_acquisition_time(timestamps: tuple, exp_time: float, savefig: bool = True, drc: str = None) -> object:
-    """take a list of timestamps and return the acquisition time and overhead.
+    """Take a list of timestamps and return the acquisition time and overhead.
 
     Parameters
     ----------
     timestamps : tuple
         List of timestamps
     exp_time : float
         Exposure time in s
```

### Comparing `instamatic-1.9.0/instamatic/utils/beamstop.py` & `instamatic-2.0.0/src/instamatic/utils/beamstop.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/utils/high_precision_timers.py` & `instamatic-2.0.0/src/instamatic/utils/high_precision_timers.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/utils/progress.py` & `instamatic-2.0.0/src/instamatic/utils/progress.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/utils/spinbox.py` & `instamatic-2.0.0/src/instamatic/utils/spinbox.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic/utils/xds_parser.py` & `instamatic-2.0.0/src/instamatic/utils/xds_parser.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/instamatic.egg-info/PKG-INFO` & `instamatic-2.0.0/src/instamatic.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: instamatic
-Version: 1.9.0
+Version: 2.0.0
 Summary: Python program for automated electron diffraction data collection
-Home-page: http://github.com/instamatic-dev/instamatic
-Author: Stef Smeets
-Author-email: s.smeets@esciencecenter.nl
-License: UNKNOWN
-Project-URL: Bug Tracker, http://github.com/instamatic-dev/instamatic/issues
-Project-URL: Documentation, https://instamatic.readthedocs.io/
+Author-email: Stef Smeets <s.smeets@esciencecenter.nl>
+License: BSD License
+Project-URL: homepage, https://github.com/instamatic-dev/instamatic
+Project-URL: issues, http://github.com/instamatic-dev/instamatic/issues
+Project-URL: documentation, https://instamatic.readthedocs.io
+Project-URL: changelog, https://github.com/instamatic-dev/instamatic/releases
 Keywords: electron-crystallography,electron-microscopy,electron-diffraction,serial-crystallography,3D-electron-diffraction,micro-ed,data-collection,automation
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Software Development :: Libraries
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: develop
 Provides-Extra: serval
+Provides-Extra: docs
+Provides-Extra: publishing
 License-File: LICENCE
-
-UNKNOWN
-
```

### Comparing `instamatic-1.9.0/instamatic.egg-info/SOURCES.txt` & `instamatic-2.0.0/src/instamatic.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,212 +1,214 @@
 .pre-commit-config.yaml
 LICENCE
 MANIFEST.in
 THANKS.md
 pyproject.toml
 requirements.txt
-setup.cfg
-setup.py
-setup_win.bat
-docs/conf.py
+docs/CODE_OF_CONDUCT.md
+docs/CONTRIBUTING.md
+docs/banner.png
 docs/config.md
 docs/formats.md
 docs/gui.md
+docs/index.md
 docs/make_programs_md.py
+docs/merlin.md
+docs/network.md
 docs/programs.md
 docs/setup.md
 docs/tem_api.md
 docs/tvips.md
-instamatic/__init__.py
-instamatic/acquire_at_items.py
-instamatic/admin.py
-instamatic/banner.py
-instamatic/browser.py
-instamatic/exceptions.py
-instamatic/goniotool.py
-instamatic/gridmontage.py
-instamatic/image_utils.py
-instamatic/imreg.py
-instamatic/io.py
-instamatic/main.py
-instamatic/montage.py
-instamatic/tools.py
-instamatic.egg-info/PKG-INFO
-instamatic.egg-info/SOURCES.txt
-instamatic.egg-info/dependency_links.txt
-instamatic.egg-info/entry_points.txt
-instamatic.egg-info/not-zip-safe
-instamatic.egg-info/requires.txt
-instamatic.egg-info/top_level.txt
-instamatic/TEMController/TEMController.py
-instamatic/TEMController/__init__.py
-instamatic/TEMController/deflectors.py
-instamatic/TEMController/fei_microscope.py
-instamatic/TEMController/fei_simu_microscope.py
-instamatic/TEMController/jeol_microscope.py
-instamatic/TEMController/lenses.py
-instamatic/TEMController/microscope.py
-instamatic/TEMController/microscope_client.py
-instamatic/TEMController/simu_microscope.py
-instamatic/TEMController/stage.py
-instamatic/TEMController/states.py
-instamatic/calibrate/__init__.py
-instamatic/calibrate/calibrate_beamshift.py
-instamatic/calibrate/calibrate_brightness.py
-instamatic/calibrate/calibrate_directbeam.py
-instamatic/calibrate/calibrate_imageshift12.py
-instamatic/calibrate/calibrate_stage_lowmag.py
-instamatic/calibrate/calibrate_stage_mag1.py
-instamatic/calibrate/calibrate_stagematrix.py
-instamatic/calibrate/center_z.py
-instamatic/calibrate/filenames.py
-instamatic/calibrate/fit.py
-instamatic/camera/CCDCOM.h
-instamatic/camera/CCDCOM2_x64_gatan.dll
-instamatic/camera/CCDCOM2_x64_simulation.dll
-instamatic/camera/CCDCOM2_x86_gatan.dll
-instamatic/camera/CCDCOM2_x86_simulation.dll
-instamatic/camera/EMCameraObj.dll
-instamatic/camera/__init__.py
-instamatic/camera/camera.py
-instamatic/camera/camera_client.py
-instamatic/camera/camera_emmenu.py
-instamatic/camera/camera_gatan.py
-instamatic/camera/camera_gatan2.py
-instamatic/camera/camera_merlin.py
-instamatic/camera/camera_serval.py
-instamatic/camera/camera_simu.py
-instamatic/camera/camera_timepix.py
-instamatic/camera/fakevideostream.py
-instamatic/camera/gatansocket3.md
-instamatic/camera/gatansocket3.py
-instamatic/camera/merlin_io.py
-instamatic/camera/mpxhwrelaxd.dll
-instamatic/camera/timepix.lockfile
-instamatic/camera/videostream.py
-instamatic/camera/tpx/171207_with_flatfield.bpc
-instamatic/camera/tpx/171207_with_flatfield.bpc.dacs
-instamatic/camera/tpx/HW.dacs
-instamatic/camera/tpx/config.txt
-instamatic/config/__init__.py
-instamatic/config/autoconfig.py
-instamatic/config/config_updater.py
-instamatic/config/defaults.yaml
-instamatic/config/settings.yaml
-instamatic/config/utils.py
-instamatic/config/alignments/neutral.yaml
-instamatic/config/calibration/orius.yaml
-instamatic/config/calibration/simulate.yaml
-instamatic/config/calibration/timepix.yaml
-instamatic/config/calibration/tvips-f416.yaml
-instamatic/config/camera/merlin.yaml
-instamatic/config/camera/orius.yaml
-instamatic/config/camera/serval.yaml
-instamatic/config/camera/simulate.yaml
-instamatic/config/camera/simulateDLL.yaml
-instamatic/config/camera/timepix.yaml
-instamatic/config/camera/tvips-f416.yaml
-instamatic/config/camera/tvips-xf416.yaml
-instamatic/config/microscope/fei_simu.yaml
-instamatic/config/microscope/fei_themisZ.yaml
-instamatic/config/microscope/jeol-1400.yaml
-instamatic/config/microscope/jeol.yaml
-instamatic/config/microscope/simulate.yaml
-instamatic/config/scripts/readme.md
-instamatic/experiments/__init__.py
-instamatic/experiments/autocred/__init__.py
-instamatic/experiments/autocred/experiment.py
-instamatic/experiments/cred/__init__.py
-instamatic/experiments/cred/experiment.py
-instamatic/experiments/cred_gatan/__init__.py
-instamatic/experiments/cred_gatan/experiment.py
-instamatic/experiments/cred_tvips/__init__.py
-instamatic/experiments/cred_tvips/experiment.py
-instamatic/experiments/red/__init__.py
-instamatic/experiments/red/experiment.py
-instamatic/experiments/serialed/__init__.py
-instamatic/experiments/serialed/experiment.py
-instamatic/formats/__init__.py
-instamatic/formats/adscimage.py
-instamatic/formats/csvIO.py
-instamatic/formats/mrc.py
-instamatic/formats/util.py
-instamatic/formats/xdscbf.py
-instamatic/gui/__init__.py
-instamatic/gui/about_frame.py
-instamatic/gui/autocred_frame.py
-instamatic/gui/base_module.py
-instamatic/gui/console_frame.py
-instamatic/gui/cred_fei_frame.py
-instamatic/gui/cred_frame.py
-instamatic/gui/cred_tvips_frame.py
-instamatic/gui/ctrl_frame.py
-instamatic/gui/debug_frame.py
-instamatic/gui/defocus_button.py
-instamatic/gui/gui.py
-instamatic/gui/io_frame.py
-instamatic/gui/jobs.py
-instamatic/gui/machine_learning_frame.py
-instamatic/gui/modules.py
-instamatic/gui/mpl_frame.py
-instamatic/gui/red_frame.py
-instamatic/gui/sed_frame.py
-instamatic/gui/videostream_frame.py
-instamatic/neural_network/__init__.py
-instamatic/neural_network/neural_network.py
-instamatic/neural_network/preprocess.py
-instamatic/neural_network/preprocess_SerialRED.py
-instamatic/processing/ImgConversion.py
-instamatic/processing/ImgConversionDM.py
-instamatic/processing/ImgConversionTPX.py
-instamatic/processing/ImgConversionTVIPS.py
-instamatic/processing/XDS_template.py
-instamatic/processing/XDS_templateDM.py
-instamatic/processing/XDS_templateTPX.py
-instamatic/processing/XDS_templateTVIPS.py
-instamatic/processing/__init__.py
-instamatic/processing/find_crystals.py
-instamatic/processing/find_crystals_ilastik.py
-instamatic/processing/find_holes.py
-instamatic/processing/flatfield.py
-instamatic/processing/stretch_correction.py
-instamatic/server/TEMServer_FEI.py
-instamatic/server/__init__.py
-instamatic/server/cam_client.py
-instamatic/server/cam_server.py
-instamatic/server/dials_server.py
-instamatic/server/goniotool_server.py
-instamatic/server/serializer.py
-instamatic/server/tem_client.py
-instamatic/server/tem_server.py
-instamatic/server/vm_ubuntu_server.py
-instamatic/server/xds_server.py
-instamatic/utils/__init__.py
-instamatic/utils/beamstop.py
-instamatic/utils/high_precision_timers.py
-instamatic/utils/progress.py
-instamatic/utils/singleton.py
-instamatic/utils/spinbox.py
-instamatic/utils/xds_parser.py
-notebooks/data_collection.ipynb
-notebooks/grid_montage_collection.ipynb
-notebooks/montage_processing.ipynb
-notebooks/nav.nav
-notebooks/readme.md
 scripts/__init__.py
 scripts/browser.py
 scripts/center_images_smv.py
 scripts/diagnose_beam_drift.py
 scripts/learn.py
 scripts/make_interval_movie.py
 scripts/make_serialed_movie.py
 scripts/process_dm.py
 scripts/process_tpx.py
 scripts/process_tvips.py
 scripts/viewer.py
+src/instamatic/__init__.py
+src/instamatic/acquire_at_items.py
+src/instamatic/admin.py
+src/instamatic/banner.py
+src/instamatic/browser.py
+src/instamatic/exceptions.py
+src/instamatic/goniotool.py
+src/instamatic/gridmontage.py
+src/instamatic/image_utils.py
+src/instamatic/imreg.py
+src/instamatic/io.py
+src/instamatic/main.py
+src/instamatic/montage.py
+src/instamatic/tools.py
+src/instamatic.egg-info/PKG-INFO
+src/instamatic.egg-info/SOURCES.txt
+src/instamatic.egg-info/dependency_links.txt
+src/instamatic.egg-info/entry_points.txt
+src/instamatic.egg-info/requires.txt
+src/instamatic.egg-info/top_level.txt
+src/instamatic/TEMController/TEMController.py
+src/instamatic/TEMController/__init__.py
+src/instamatic/TEMController/deflectors.py
+src/instamatic/TEMController/fei_microscope.py
+src/instamatic/TEMController/fei_simu_microscope.py
+src/instamatic/TEMController/jeol_microscope.py
+src/instamatic/TEMController/lenses.py
+src/instamatic/TEMController/microscope.py
+src/instamatic/TEMController/microscope_client.py
+src/instamatic/TEMController/simu_microscope.py
+src/instamatic/TEMController/stage.py
+src/instamatic/TEMController/states.py
+src/instamatic/calibrate/__init__.py
+src/instamatic/calibrate/calibrate_beamshift.py
+src/instamatic/calibrate/calibrate_brightness.py
+src/instamatic/calibrate/calibrate_directbeam.py
+src/instamatic/calibrate/calibrate_imageshift12.py
+src/instamatic/calibrate/calibrate_stage_lowmag.py
+src/instamatic/calibrate/calibrate_stage_mag1.py
+src/instamatic/calibrate/calibrate_stagematrix.py
+src/instamatic/calibrate/center_z.py
+src/instamatic/calibrate/filenames.py
+src/instamatic/calibrate/fit.py
+src/instamatic/camera/CCDCOM.h
+src/instamatic/camera/CCDCOM2_x64_gatan.dll
+src/instamatic/camera/CCDCOM2_x64_simulation.dll
+src/instamatic/camera/CCDCOM2_x86_gatan.dll
+src/instamatic/camera/CCDCOM2_x86_simulation.dll
+src/instamatic/camera/EMCameraObj.dll
+src/instamatic/camera/__init__.py
+src/instamatic/camera/camera.py
+src/instamatic/camera/camera_client.py
+src/instamatic/camera/camera_emmenu.py
+src/instamatic/camera/camera_gatan.py
+src/instamatic/camera/camera_gatan2.py
+src/instamatic/camera/camera_merlin.py
+src/instamatic/camera/camera_serval.py
+src/instamatic/camera/camera_simu.py
+src/instamatic/camera/camera_timepix.py
+src/instamatic/camera/fakevideostream.py
+src/instamatic/camera/gatansocket3.md
+src/instamatic/camera/gatansocket3.py
+src/instamatic/camera/merlin_io.py
+src/instamatic/camera/mpxhwrelaxd.dll
+src/instamatic/camera/timepix.lockfile
+src/instamatic/camera/videostream.py
+src/instamatic/camera/tpx/171207_with_flatfield.bpc
+src/instamatic/camera/tpx/171207_with_flatfield.bpc.dacs
+src/instamatic/camera/tpx/HW.dacs
+src/instamatic/camera/tpx/config.txt
+src/instamatic/config/__init__.py
+src/instamatic/config/autoconfig.py
+src/instamatic/config/config_updater.py
+src/instamatic/config/defaults.yaml
+src/instamatic/config/settings.yaml
+src/instamatic/config/utils.py
+src/instamatic/config/alignments/neutral.yaml
+src/instamatic/config/calibration/orius.yaml
+src/instamatic/config/calibration/simulate.yaml
+src/instamatic/config/calibration/timepix.yaml
+src/instamatic/config/calibration/tvips-f416.yaml
+src/instamatic/config/camera/merlin.yaml
+src/instamatic/config/camera/orius.yaml
+src/instamatic/config/camera/serval.yaml
+src/instamatic/config/camera/simulate.yaml
+src/instamatic/config/camera/simulateDLL.yaml
+src/instamatic/config/camera/timepix.yaml
+src/instamatic/config/camera/tvips-f416.yaml
+src/instamatic/config/camera/tvips-xf416.yaml
+src/instamatic/config/microscope/fei_simu.yaml
+src/instamatic/config/microscope/fei_themisZ.yaml
+src/instamatic/config/microscope/jeol-1400.yaml
+src/instamatic/config/microscope/jeol.yaml
+src/instamatic/config/microscope/simulate.yaml
+src/instamatic/config/scripts/close_down.py
+src/instamatic/config/scripts/focus_mode.py
+src/instamatic/config/scripts/hello_world.py
+src/instamatic/config/scripts/readme.md
+src/instamatic/config/scripts/search_mode.py
+src/instamatic/experiments/__init__.py
+src/instamatic/experiments/autocred/__init__.py
+src/instamatic/experiments/autocred/experiment.py
+src/instamatic/experiments/cred/__init__.py
+src/instamatic/experiments/cred/experiment.py
+src/instamatic/experiments/cred_gatan/__init__.py
+src/instamatic/experiments/cred_gatan/experiment.py
+src/instamatic/experiments/cred_tvips/__init__.py
+src/instamatic/experiments/cred_tvips/experiment.py
+src/instamatic/experiments/red/__init__.py
+src/instamatic/experiments/red/experiment.py
+src/instamatic/experiments/serialed/__init__.py
+src/instamatic/experiments/serialed/experiment.py
+src/instamatic/formats/__init__.py
+src/instamatic/formats/adscimage.py
+src/instamatic/formats/csvIO.py
+src/instamatic/formats/mrc.py
+src/instamatic/formats/util.py
+src/instamatic/formats/xdscbf.py
+src/instamatic/gui/__init__.py
+src/instamatic/gui/about_frame.py
+src/instamatic/gui/autocred_frame.py
+src/instamatic/gui/base_module.py
+src/instamatic/gui/console_frame.py
+src/instamatic/gui/cred_fei_frame.py
+src/instamatic/gui/cred_frame.py
+src/instamatic/gui/cred_tvips_frame.py
+src/instamatic/gui/ctrl_frame.py
+src/instamatic/gui/debug_frame.py
+src/instamatic/gui/defocus_button.py
+src/instamatic/gui/gui.py
+src/instamatic/gui/io_frame.py
+src/instamatic/gui/jobs.py
+src/instamatic/gui/machine_learning_frame.py
+src/instamatic/gui/modules.py
+src/instamatic/gui/mpl_frame.py
+src/instamatic/gui/red_frame.py
+src/instamatic/gui/sed_frame.py
+src/instamatic/gui/videostream_frame.py
+src/instamatic/neural_network/__init__.py
+src/instamatic/neural_network/neural_network.py
+src/instamatic/neural_network/preprocess.py
+src/instamatic/neural_network/preprocess_SerialRED.py
+src/instamatic/neural_network/weights-py2.p
+src/instamatic/neural_network/weights-py3.p
+src/instamatic/processing/ImgConversion.py
+src/instamatic/processing/ImgConversionDM.py
+src/instamatic/processing/ImgConversionTPX.py
+src/instamatic/processing/ImgConversionTVIPS.py
+src/instamatic/processing/XDS_template.py
+src/instamatic/processing/XDS_templateDM.py
+src/instamatic/processing/XDS_templateTPX.py
+src/instamatic/processing/XDS_templateTVIPS.py
+src/instamatic/processing/__init__.py
+src/instamatic/processing/find_crystals.py
+src/instamatic/processing/find_crystals_ilastik.py
+src/instamatic/processing/find_holes.py
+src/instamatic/processing/flatfield.py
+src/instamatic/processing/stretch_correction.py
+src/instamatic/server/TEMServer_FEI.py
+src/instamatic/server/__init__.py
+src/instamatic/server/cam_client.py
+src/instamatic/server/cam_server.py
+src/instamatic/server/dials_server.py
+src/instamatic/server/goniotool_server.py
+src/instamatic/server/serializer.py
+src/instamatic/server/tem_client.py
+src/instamatic/server/tem_server.py
+src/instamatic/server/vm_ubuntu_server.py
+src/instamatic/server/xds_server.py
+src/instamatic/utils/__init__.py
+src/instamatic/utils/beamstop.py
+src/instamatic/utils/high_precision_timers.py
+src/instamatic/utils/progress.py
+src/instamatic/utils/singleton.py
+src/instamatic/utils/spinbox.py
+src/instamatic/utils/xds_parser.py
 tests/conftest.py
 tests/test_camera.py
 tests/test_ctrl.py
 tests/test_experiments.py
 tests/test_formats.py
 tests/test_grid_mapping.py
 tests/test_merlin_io.py
```

### Comparing `instamatic-1.9.0/instamatic.egg-info/entry_points.txt` & `instamatic-2.0.0/src/instamatic.egg-info/entry_points.txt`

 * *Files 0% similar despite different names*

```diff
@@ -20,8 +20,7 @@
 instamatic.learn = scripts.learn:main_entry
 instamatic.serialed = instamatic.experiments.serialed.experiment:main
 instamatic.stretch_correction = instamatic.processing.stretch_correction:main_entry
 instamatic.temserver = instamatic.server.tem_server:main
 instamatic.temserver_fei = instamatic.server.TEMServer_FEI:main
 instamatic.viewer = scripts.viewer:main
 instamatic.xdsserver = instamatic.server.xds_server:main
-
```

### Comparing `instamatic-1.9.0/scripts/browser.py` & `instamatic-2.0.0/scripts/browser.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/scripts/center_images_smv.py` & `instamatic-2.0.0/scripts/center_images_smv.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 n = len(fns)
 print(n)
 
 
 def find_beam_center_blur(z: np.ndarray, sigma: int = 30) -> np.ndarray:
     """Estimate direct beam position by blurring the image with a large
     Gaussian kernel and finding the maximum.
+
     Parameters
     ----------
     sigma : float
         Sigma value for Gaussian blurring kernel.
     Returns
     -------
     center : np.array
```

### Comparing `instamatic-1.9.0/scripts/diagnose_beam_drift.py` & `instamatic-2.0.0/scripts/diagnose_beam_drift.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/scripts/learn.py` & `instamatic-2.0.0/scripts/learn.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/scripts/make_interval_movie.py` & `instamatic-2.0.0/scripts/make_interval_movie.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/scripts/make_serialed_movie.py` & `instamatic-2.0.0/scripts/make_serialed_movie.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/scripts/process_dm.py` & `instamatic-2.0.0/scripts/process_dm.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import numpy as np
 from PIL import Image
 
 from instamatic.processing.ImgConversionDM import ImgConversionDM as ImgConversion
 
 # Script to process cRED data collecting using the DigitalMicrograph script `insteaDMatic`
-# https://github.com/instamatic-dev/instamatic/tree/master/dmscript
+# https://github.com/instamatic-dev/InsteaDMatic
 #
 # To use:
 #     Run `python process_dm.py cred_log.txt`
 #
 # Where the first argument is the path to the cred_log.txt file. Assumes the data are stored
 # in a subdirectory `tiff/*.tif` from where cred_log.txt is stored.
 #
```

### Comparing `instamatic-1.9.0/scripts/process_tpx.py` & `instamatic-2.0.0/scripts/process_tpx.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/scripts/process_tvips.py` & `instamatic-2.0.0/scripts/process_tvips.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/scripts/viewer.py` & `instamatic-2.0.0/scripts/viewer.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/tests/config/calibration/test.yaml` & `instamatic-2.0.0/src/instamatic/config/calibration/simulate.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -7,17 +7,61 @@
     300: 0.00412
     400: 0.00296
     500: 0.00238
     600: 0.00198
     800: 0.00148
 lowmag:
   pixelsize:
-    -1: -1
+    50: 569.400
+    80: 355.875
+    100: 284.700
+    150: 189.800
+    200: 142.350
+    250: 113.880
+    300: 94.900
+    400: 71.175
+    500: 56.940
+    600: 47.450
+    800: 35.586
+    1000: 28.470
+    1200: 23.725
+    1500: 18.980
+    2000: 14.235
+    2500: 11.388
+    3000: 9.490
+    5000: 5.694
+    6000: 4.745
+    8000: 3.559
+    10000: 2.847
+    12000: 2.373
+    15000: 1.898
   stagematrix:
-    -1: []
+    50: [1, 0, 0, 1]
+    80: [1, 0, 0, 1]
+    100: [1, 0, 0, 1]
+    150: [1, 0, 0, 1]
+    200: [1, 0, 0, 1]
+    250: [1, 0, 0, 1]
+    300: [1, 0, 0, 1]
+    400: [1, 0, 0, 1]
+    500: [1, 0, 0, 1]
+    600: [1, 0, 0, 1]
+    800: [1, 0, 0, 1]
+    1000: [1, 0, 0, 1]
+    1200: [1, 0, 0, 1]
+    1500: [1, 0, 0, 1]
+    2000: [1, 0, 0, 1]
+    2500: [1, 0, 0, 1]
+    3000: [1, 0, 0, 1]
+    5000: [1, 0, 0, 1]
+    6000: [1, 0, 0, 1]
+    8000: [1, 0, 0, 1]
+    10000: [1, 0, 0, 1]
+    12000: [1, 0, 0, 1]
+    15000: [1, 0, 0, 1]
 mag1:
   pixelsize:
     2500: 11.54651
     3000: 9.49031
     4000: 6.99806
     5000: 5.54069
     6000: 4.5872
```

### Comparing `instamatic-1.9.0/tests/test_ctrl.py` & `instamatic-2.0.0/tests/test_ctrl.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/tests/test_experiments.py` & `instamatic-2.0.0/tests/test_experiments.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/tests/test_formats.py` & `instamatic-2.0.0/tests/test_formats.py`

 * *Files identical despite different names*

### Comparing `instamatic-1.9.0/tests/test_merlin_io.py` & `instamatic-2.0.0/tests/test_merlin_io.py`

 * *Files identical despite different names*

