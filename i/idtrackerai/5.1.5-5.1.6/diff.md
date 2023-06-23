# Comparing `tmp/idtrackerai-5.1.5.tar.gz` & `tmp/idtrackerai-5.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idtrackerai-5.1.5.tar", last modified: Thu Jun 15 10:24:12 2023, max compression
+gzip compressed data, was "idtrackerai-5.1.6.tar", last modified: Fri Jun 23 14:41:48 2023, max compression
```

## Comparing `idtrackerai-5.1.5.tar` & `idtrackerai-5.1.6.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-15 10:24:12.037140 idtrackerai-5.1.5/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    35987 2023-02-10 16:03:19.000000 idtrackerai-5.1.5/LICENSE
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2828 2023-06-15 10:24:12.037140 idtrackerai-5.1.5/PKG-INFO
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1601 2023-05-29 19:16:39.000000 idtrackerai-5.1.5/README.md
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3095 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/pyproject.toml
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       38 2023-06-15 10:24:12.037140 idtrackerai-5.1.5/setup.cfg
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-15 10:24:12.013139 idtrackerai-5.1.5/src/
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-15 10:24:12.013139 idtrackerai-5.1.5/src/idmatcherai/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:15:16.000000 idtrackerai-5.1.5/src/idmatcherai/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     9102 2023-05-29 19:16:39.000000 idtrackerai-5.1.5/src/idmatcherai/main.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3614 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idmatcherai/matcher.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-15 10:24:12.013139 idtrackerai-5.1.5/src/idtrackerai/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      587 2023-05-16 10:39:16.000000 idtrackerai-5.1.5/src/idtrackerai/__init__.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-15 10:24:12.017139 idtrackerai-5.1.5/src/idtrackerai/animals_detection/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       90 2023-05-16 10:39:16.000000 idtrackerai-5.1.5/src/idtrackerai/animals_detection/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6157 2023-05-29 18:19:35.000000 idtrackerai-5.1.5/src/idtrackerai/animals_detection/animals_detection.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    14496 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai/animals_detection/segmentation.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    31620 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai/blob.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3215 2023-05-29 18:15:16.000000 idtrackerai-5.1.5/src/idtrackerai/constants.toml
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-15 10:24:12.017139 idtrackerai-5.1.5/src/idtrackerai/crossings_detection/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1658 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai/crossings_detection/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5128 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai/crossings_detection/crossing_detector.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     7941 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai/crossings_detection/crossings_dataset.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5788 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai/crossings_detection/crossings_network.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4938 2023-05-29 19:16:39.000000 idtrackerai-5.1.5/src/idtrackerai/crossings_detection/model_area.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-15 10:24:12.021139 idtrackerai-5.1.5/src/idtrackerai/data/
--rwxrwxr-x   0 jordi     (1000) jordi     (1000)  5933626 2023-05-16 10:39:16.000000 idtrackerai-5.1.5/src/idtrackerai/data/test_A.avi
--rwxrwxr-x   0 jordi     (1000) jordi     (1000)  5976882 2023-05-16 10:39:16.000000 idtrackerai-5.1.5/src/idtrackerai/data/test_B.avi
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    26290 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai/fragment.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-15 10:24:12.029139 idtrackerai-5.1.5/src/idtrackerai/fragmentation/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       78 2023-05-16 10:39:16.000000 idtrackerai-5.1.5/src/idtrackerai/fragmentation/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4529 2023-06-12 11:03:30.000000 idtrackerai-5.1.5/src/idtrackerai/fragmentation/fragmentation.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     7903 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai/globalfragment.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-15 10:24:12.029139 idtrackerai-5.1.5/src/idtrackerai/groundtruth_utils/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-05-16 10:39:16.000000 idtrackerai-5.1.5/src/idtrackerai/groundtruth_utils/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    22015 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai/groundtruth_utils/compute_groundtruth_statistics.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    20302 2023-05-29 18:15:16.000000 idtrackerai-5.1.5/src/idtrackerai/groundtruth_utils/compute_groundtruth_statistics_general.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3924 2023-05-16 10:39:16.000000 idtrackerai-5.1.5/src/idtrackerai/groundtruth_utils/compute_individual_groundtruth_statistics.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5589 2023-05-29 18:15:16.000000 idtrackerai-5.1.5/src/idtrackerai/groundtruth_utils/generate_groundtruth.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3989 2023-05-29 18:15:16.000000 idtrackerai-5.1.5/src/idtrackerai/groundtruth_utils/generate_individual_groundtruth.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    15622 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai/list_of_blobs.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    27122 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai/list_of_fragments.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    10046 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai/list_of_global_fragments.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-15 10:24:12.029139 idtrackerai-5.1.5/src/idtrackerai/network/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      489 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai/network/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2541 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai/network/evaluate.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3097 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai/network/learners.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6563 2023-05-29 18:15:16.000000 idtrackerai-5.1.5/src/idtrackerai/network/models.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2049 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai/network/network_params.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2190 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai/network/train.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3109 2023-06-15 10:19:56.000000 idtrackerai-5.1.5/src/idtrackerai/network/utils.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-15 10:24:12.029139 idtrackerai-5.1.5/src/idtrackerai/postprocess/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      292 2023-05-16 10:39:16.000000 idtrackerai-5.1.5/src/idtrackerai/postprocess/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    27711 2023-05-29 19:16:39.000000 idtrackerai-5.1.5/src/idtrackerai/postprocess/assign_them_all.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2731 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai/postprocess/compute_velocity_model.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    21299 2023-05-29 19:16:39.000000 idtrackerai-5.1.5/src/idtrackerai/postprocess/correct_impossible_velocity_jumps.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3602 2023-05-29 19:16:39.000000 idtrackerai-5.1.5/src/idtrackerai/postprocess/erosion.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     8671 2023-05-29 19:16:39.000000 idtrackerai-5.1.5/src/idtrackerai/postprocess/get_trajectories.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2592 2023-05-16 10:39:16.000000 idtrackerai-5.1.5/src/idtrackerai/postprocess/identify_non_assigned_with_interpolation.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5168 2023-05-29 19:16:39.000000 idtrackerai-5.1.5/src/idtrackerai/postprocess/trajectories_creation.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4576 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai/postprocess/trajectories_to_csv.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-15 10:24:12.033139 idtrackerai-5.1.5/src/idtrackerai/tracker/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-05-16 10:39:16.000000 idtrackerai-5.1.5/src/idtrackerai/tracker/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    34690 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai/tracker/accumulation_manager.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     8555 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai/tracker/accumulator.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5735 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai/tracker/assigner.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6611 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai/tracker/identity_dataset.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     7871 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai/tracker/identity_network.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5548 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai/tracker/identity_transfer.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6595 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai/tracker/pre_trainer.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    26449 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai/tracker/tracker.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-15 10:24:12.033139 idtrackerai-5.1.5/src/idtrackerai/utils/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1216 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai/utils/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2170 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai/utils/check_PyPI_version.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1143 2023-05-16 10:39:16.000000 idtrackerai-5.1.5/src/idtrackerai/utils/confparams.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2890 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai/utils/init_logger.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    13544 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai/utils/py_utils.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    32674 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai/video.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-15 10:24:12.017139 idtrackerai-5.1.5/src/idtrackerai.egg-info/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2828 2023-06-15 10:24:11.000000 idtrackerai-5.1.5/src/idtrackerai.egg-info/PKG-INFO
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5052 2023-06-15 10:24:12.000000 idtrackerai-5.1.5/src/idtrackerai.egg-info/SOURCES.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-06-15 10:24:12.000000 idtrackerai-5.1.5/src/idtrackerai.egg-info/dependency_links.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      341 2023-06-15 10:24:12.000000 idtrackerai-5.1.5/src/idtrackerai.egg-info/entry_points.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      364 2023-06-15 10:24:12.000000 idtrackerai-5.1.5/src/idtrackerai.egg-info/requires.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      108 2023-06-15 10:24:12.000000 idtrackerai-5.1.5/src/idtrackerai.egg-info/top_level.txt
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-15 10:24:12.033139 idtrackerai-5.1.5/src/idtrackerai_GUI_tools/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6443 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai_GUI_tools/GUI_main_base.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1016 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai_GUI_tools/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2448 2023-05-16 10:39:16.000000 idtrackerai-5.1.5/src/idtrackerai_GUI_tools/cmap_gist_rainbow.dat
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    66516 2023-05-16 10:39:16.000000 idtrackerai-5.1.5/src/idtrackerai_GUI_tools/logo_256.png
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     9146 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai_GUI_tools/themes.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      619 2023-05-16 10:39:16.000000 idtrackerai-5.1.5/src/idtrackerai_GUI_tools/tooltips.toml
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-15 10:24:12.033139 idtrackerai-5.1.5/src/idtrackerai_GUI_tools/widgets_utils/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5528 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai_GUI_tools/widgets_utils/canvas.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6046 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai_GUI_tools/widgets_utils/custom_list.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     8201 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai_GUI_tools/widgets_utils/other_utils.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2870 2023-05-29 18:19:35.000000 idtrackerai-5.1.5/src/idtrackerai_GUI_tools/widgets_utils/video_paths_holder.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    13651 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai_GUI_tools/widgets_utils/video_player.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-15 10:24:12.033139 idtrackerai-5.1.5/src/idtrackerai_start_app/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:15:16.000000 idtrackerai-5.1.5/src/idtrackerai_start_app/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5657 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai_start_app/__main__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1515 2023-05-29 18:15:16.000000 idtrackerai-5.1.5/src/idtrackerai_start_app/all_valid_parameters.dat
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6826 2023-05-29 18:15:16.000000 idtrackerai-5.1.5/src/idtrackerai_start_app/arg_parser.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5904 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai_start_app/run_idtrackerai.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    16108 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai_start_app/segmentation_GUI.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-15 10:24:12.033139 idtrackerai-5.1.5/src/idtrackerai_start_app/segmentation_widgets/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     8407 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai_start_app/segmentation_widgets/ROI_widget.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      482 2023-05-16 10:39:16.000000 idtrackerai-5.1.5/src/idtrackerai_start_app/segmentation_widgets/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5782 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai_start_app/segmentation_widgets/bkg_widget.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5804 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai_start_app/segmentation_widgets/blob_info_widget.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3527 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai_start_app/segmentation_widgets/frame_analyzer.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2358 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai_start_app/segmentation_widgets/intensity_ths.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6777 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai_start_app/segmentation_widgets/open_video_widget.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4997 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai_start_app/segmentation_widgets/track_intervals_widget.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2713 2023-05-29 18:15:16.000000 idtrackerai-5.1.5/src/idtrackerai_start_app/tooltips.toml
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-15 10:24:12.037140 idtrackerai-5.1.5/src/idtrackerai_validator/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:15:16.000000 idtrackerai-5.1.5/src/idtrackerai_validator/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      671 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai_validator/__main__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      715 2023-05-16 10:39:16.000000 idtrackerai-5.1.5/src/idtrackerai_validator/tooltips.toml
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    35131 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai_validator/validation_GUI.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-15 10:24:12.037140 idtrackerai-5.1.5/src/idtrackerai_validator/validator_widgets/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      547 2023-05-29 19:16:39.000000 idtrackerai-5.1.5/src/idtrackerai_validator/validator_widgets/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1986 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai_validator/validator_widgets/additional_info.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     8093 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai_validator/validator_widgets/errors_explorer.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6047 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai_validator/validator_widgets/id_groups.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1495 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai_validator/validator_widgets/id_labels.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    12980 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai_validator/validator_widgets/interpolator.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4484 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai_validator/validator_widgets/mark_properties.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6771 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai_validator/validator_widgets/paint_blobs.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4926 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai_validator/validator_widgets/setup_points.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-15 10:24:12.037140 idtrackerai-5.1.5/src/idtrackerai_video/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:15:16.000000 idtrackerai-5.1.5/src/idtrackerai_video/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5157 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai_video/general_video.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4085 2023-05-29 19:16:39.000000 idtrackerai-5.1.5/src/idtrackerai_video/individual_videos.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2961 2023-05-29 18:19:35.000000 idtrackerai-5.1.5/src/idtrackerai_video/main.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-23 14:41:48.182894 idtrackerai-5.1.6/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    35987 2023-02-10 16:03:19.000000 idtrackerai-5.1.6/LICENSE
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2828 2023-06-23 14:41:48.178894 idtrackerai-5.1.6/PKG-INFO
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1601 2023-05-29 19:16:39.000000 idtrackerai-5.1.6/README.md
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3120 2023-06-23 11:15:02.000000 idtrackerai-5.1.6/pyproject.toml
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       38 2023-06-23 14:41:48.182894 idtrackerai-5.1.6/setup.cfg
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-23 14:41:48.150894 idtrackerai-5.1.6/src/
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-23 14:41:48.150894 idtrackerai-5.1.6/src/idmatcherai/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:15:16.000000 idtrackerai-5.1.6/src/idmatcherai/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     9110 2023-06-23 11:05:25.000000 idtrackerai-5.1.6/src/idmatcherai/main.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3614 2023-06-23 11:39:21.000000 idtrackerai-5.1.6/src/idmatcherai/matcher.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-23 14:41:48.150894 idtrackerai-5.1.6/src/idtrackerai/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      587 2023-05-16 10:39:16.000000 idtrackerai-5.1.6/src/idtrackerai/__init__.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-23 14:41:48.154894 idtrackerai-5.1.6/src/idtrackerai/animals_detection/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       90 2023-05-16 10:39:16.000000 idtrackerai-5.1.6/src/idtrackerai/animals_detection/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6157 2023-05-29 18:19:35.000000 idtrackerai-5.1.6/src/idtrackerai/animals_detection/animals_detection.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    14070 2023-06-23 14:35:23.000000 idtrackerai-5.1.6/src/idtrackerai/animals_detection/segmentation.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    31662 2023-06-20 14:51:36.000000 idtrackerai-5.1.6/src/idtrackerai/blob.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3145 2023-06-23 14:35:23.000000 idtrackerai-5.1.6/src/idtrackerai/constants.toml
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-23 14:41:48.154894 idtrackerai-5.1.6/src/idtrackerai/crossings_detection/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1658 2023-06-15 10:18:22.000000 idtrackerai-5.1.6/src/idtrackerai/crossings_detection/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5128 2023-06-15 10:18:22.000000 idtrackerai-5.1.6/src/idtrackerai/crossings_detection/crossing_detector.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     7941 2023-06-15 10:18:22.000000 idtrackerai-5.1.6/src/idtrackerai/crossings_detection/crossings_dataset.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5788 2023-06-15 10:18:22.000000 idtrackerai-5.1.6/src/idtrackerai/crossings_detection/crossings_network.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4938 2023-05-29 19:16:39.000000 idtrackerai-5.1.6/src/idtrackerai/crossings_detection/model_area.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-23 14:41:48.162894 idtrackerai-5.1.6/src/idtrackerai/data/
+-rwxrwxr-x   0 jordi     (1000) jordi     (1000)  5933626 2023-05-16 10:39:16.000000 idtrackerai-5.1.6/src/idtrackerai/data/test_A.avi
+-rwxrwxr-x   0 jordi     (1000) jordi     (1000)  5976882 2023-05-16 10:39:16.000000 idtrackerai-5.1.6/src/idtrackerai/data/test_B.avi
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    26290 2023-06-15 10:18:22.000000 idtrackerai-5.1.6/src/idtrackerai/fragment.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-23 14:41:48.174894 idtrackerai-5.1.6/src/idtrackerai/fragmentation/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       78 2023-05-16 10:39:16.000000 idtrackerai-5.1.6/src/idtrackerai/fragmentation/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4529 2023-06-12 11:03:30.000000 idtrackerai-5.1.6/src/idtrackerai/fragmentation/fragmentation.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     7903 2023-06-15 10:18:22.000000 idtrackerai-5.1.6/src/idtrackerai/globalfragment.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-23 14:41:48.174894 idtrackerai-5.1.6/src/idtrackerai/groundtruth_utils/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-05-16 10:39:16.000000 idtrackerai-5.1.6/src/idtrackerai/groundtruth_utils/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    22015 2023-06-15 10:18:22.000000 idtrackerai-5.1.6/src/idtrackerai/groundtruth_utils/compute_groundtruth_statistics.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    20302 2023-05-29 18:15:16.000000 idtrackerai-5.1.6/src/idtrackerai/groundtruth_utils/compute_groundtruth_statistics_general.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3924 2023-05-16 10:39:16.000000 idtrackerai-5.1.6/src/idtrackerai/groundtruth_utils/compute_individual_groundtruth_statistics.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5589 2023-05-29 18:15:16.000000 idtrackerai-5.1.6/src/idtrackerai/groundtruth_utils/generate_groundtruth.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3989 2023-05-29 18:15:16.000000 idtrackerai-5.1.6/src/idtrackerai/groundtruth_utils/generate_individual_groundtruth.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    15622 2023-06-20 13:14:38.000000 idtrackerai-5.1.6/src/idtrackerai/list_of_blobs.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    27120 2023-06-23 11:09:04.000000 idtrackerai-5.1.6/src/idtrackerai/list_of_fragments.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    10046 2023-06-15 10:18:22.000000 idtrackerai-5.1.6/src/idtrackerai/list_of_global_fragments.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-23 14:41:48.174894 idtrackerai-5.1.6/src/idtrackerai/network/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      489 2023-06-15 10:18:22.000000 idtrackerai-5.1.6/src/idtrackerai/network/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2541 2023-06-15 10:18:22.000000 idtrackerai-5.1.6/src/idtrackerai/network/evaluate.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3097 2023-06-15 10:18:22.000000 idtrackerai-5.1.6/src/idtrackerai/network/learners.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6563 2023-05-29 18:15:16.000000 idtrackerai-5.1.6/src/idtrackerai/network/models.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2049 2023-06-15 10:18:22.000000 idtrackerai-5.1.6/src/idtrackerai/network/network_params.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2190 2023-06-15 10:18:22.000000 idtrackerai-5.1.6/src/idtrackerai/network/train.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3108 2023-06-19 08:08:41.000000 idtrackerai-5.1.6/src/idtrackerai/network/utils.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-23 14:41:48.174894 idtrackerai-5.1.6/src/idtrackerai/postprocess/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      292 2023-05-16 10:39:16.000000 idtrackerai-5.1.6/src/idtrackerai/postprocess/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    27711 2023-06-20 12:51:26.000000 idtrackerai-5.1.6/src/idtrackerai/postprocess/assign_them_all.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2731 2023-06-15 10:18:22.000000 idtrackerai-5.1.6/src/idtrackerai/postprocess/compute_velocity_model.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    21299 2023-05-29 19:16:39.000000 idtrackerai-5.1.6/src/idtrackerai/postprocess/correct_impossible_velocity_jumps.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3602 2023-06-20 10:49:06.000000 idtrackerai-5.1.6/src/idtrackerai/postprocess/erosion.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     8671 2023-05-29 19:16:39.000000 idtrackerai-5.1.6/src/idtrackerai/postprocess/get_trajectories.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2592 2023-05-16 10:39:16.000000 idtrackerai-5.1.6/src/idtrackerai/postprocess/identify_non_assigned_with_interpolation.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5168 2023-05-29 19:16:39.000000 idtrackerai-5.1.6/src/idtrackerai/postprocess/trajectories_creation.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4563 2023-06-23 11:13:23.000000 idtrackerai-5.1.6/src/idtrackerai/postprocess/trajectories_to_csv.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-23 14:41:48.174894 idtrackerai-5.1.6/src/idtrackerai/tracker/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-05-16 10:39:16.000000 idtrackerai-5.1.6/src/idtrackerai/tracker/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    34690 2023-06-15 10:18:22.000000 idtrackerai-5.1.6/src/idtrackerai/tracker/accumulation_manager.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     8555 2023-06-15 10:18:22.000000 idtrackerai-5.1.6/src/idtrackerai/tracker/accumulator.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5735 2023-06-15 10:18:22.000000 idtrackerai-5.1.6/src/idtrackerai/tracker/assigner.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6611 2023-06-15 10:18:22.000000 idtrackerai-5.1.6/src/idtrackerai/tracker/identity_dataset.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     7871 2023-06-15 10:18:22.000000 idtrackerai-5.1.6/src/idtrackerai/tracker/identity_network.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5548 2023-06-15 10:18:22.000000 idtrackerai-5.1.6/src/idtrackerai/tracker/identity_transfer.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6595 2023-06-15 10:18:22.000000 idtrackerai-5.1.6/src/idtrackerai/tracker/pre_trainer.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    26449 2023-06-15 10:18:22.000000 idtrackerai-5.1.6/src/idtrackerai/tracker/tracker.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-23 14:41:48.174894 idtrackerai-5.1.6/src/idtrackerai/utils/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1216 2023-06-15 10:18:22.000000 idtrackerai-5.1.6/src/idtrackerai/utils/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2170 2023-06-15 10:18:22.000000 idtrackerai-5.1.6/src/idtrackerai/utils/check_PyPI_version.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1241 2023-06-23 10:32:11.000000 idtrackerai-5.1.6/src/idtrackerai/utils/confparams.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2940 2023-06-22 12:27:52.000000 idtrackerai-5.1.6/src/idtrackerai/utils/init_logger.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    13548 2023-06-23 11:21:42.000000 idtrackerai-5.1.6/src/idtrackerai/utils/py_utils.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    32579 2023-06-23 14:35:23.000000 idtrackerai-5.1.6/src/idtrackerai/video.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-23 14:41:48.154894 idtrackerai-5.1.6/src/idtrackerai.egg-info/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2828 2023-06-23 14:41:48.000000 idtrackerai-5.1.6/src/idtrackerai.egg-info/PKG-INFO
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5052 2023-06-23 14:41:48.000000 idtrackerai-5.1.6/src/idtrackerai.egg-info/SOURCES.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-06-23 14:41:48.000000 idtrackerai-5.1.6/src/idtrackerai.egg-info/dependency_links.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      341 2023-06-23 14:41:48.000000 idtrackerai-5.1.6/src/idtrackerai.egg-info/entry_points.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      364 2023-06-23 14:41:48.000000 idtrackerai-5.1.6/src/idtrackerai.egg-info/requires.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      108 2023-06-23 14:41:48.000000 idtrackerai-5.1.6/src/idtrackerai.egg-info/top_level.txt
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-23 14:41:48.178894 idtrackerai-5.1.6/src/idtrackerai_GUI_tools/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6725 2023-06-21 11:03:55.000000 idtrackerai-5.1.6/src/idtrackerai_GUI_tools/GUI_main_base.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1016 2023-06-15 10:18:22.000000 idtrackerai-5.1.6/src/idtrackerai_GUI_tools/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2448 2023-05-16 10:39:16.000000 idtrackerai-5.1.6/src/idtrackerai_GUI_tools/cmap_gist_rainbow.dat
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    66516 2023-05-16 10:39:16.000000 idtrackerai-5.1.6/src/idtrackerai_GUI_tools/logo_256.png
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     9146 2023-06-15 10:18:22.000000 idtrackerai-5.1.6/src/idtrackerai_GUI_tools/themes.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      619 2023-05-16 10:39:16.000000 idtrackerai-5.1.6/src/idtrackerai_GUI_tools/tooltips.toml
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-23 14:41:48.178894 idtrackerai-5.1.6/src/idtrackerai_GUI_tools/widgets_utils/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5656 2023-06-19 12:08:12.000000 idtrackerai-5.1.6/src/idtrackerai_GUI_tools/widgets_utils/canvas.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6062 2023-06-19 12:08:12.000000 idtrackerai-5.1.6/src/idtrackerai_GUI_tools/widgets_utils/custom_list.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     8201 2023-06-15 10:18:22.000000 idtrackerai-5.1.6/src/idtrackerai_GUI_tools/widgets_utils/other_utils.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2870 2023-05-29 18:19:35.000000 idtrackerai-5.1.6/src/idtrackerai_GUI_tools/widgets_utils/video_paths_holder.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    13667 2023-06-21 11:03:58.000000 idtrackerai-5.1.6/src/idtrackerai_GUI_tools/widgets_utils/video_player.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-23 14:41:48.178894 idtrackerai-5.1.6/src/idtrackerai_start_app/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:15:16.000000 idtrackerai-5.1.6/src/idtrackerai_start_app/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5578 2023-06-23 14:34:29.000000 idtrackerai-5.1.6/src/idtrackerai_start_app/__main__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1491 2023-06-23 14:35:23.000000 idtrackerai-5.1.6/src/idtrackerai_start_app/all_valid_parameters.dat
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6812 2023-06-19 09:25:42.000000 idtrackerai-5.1.6/src/idtrackerai_start_app/arg_parser.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5865 2023-06-23 14:35:23.000000 idtrackerai-5.1.6/src/idtrackerai_start_app/run_idtrackerai.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    16383 2023-06-23 10:19:31.000000 idtrackerai-5.1.6/src/idtrackerai_start_app/segmentation_GUI.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-23 14:41:48.178894 idtrackerai-5.1.6/src/idtrackerai_start_app/segmentation_widgets/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     8423 2023-06-19 12:08:12.000000 idtrackerai-5.1.6/src/idtrackerai_start_app/segmentation_widgets/ROI_widget.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      482 2023-05-16 10:39:16.000000 idtrackerai-5.1.6/src/idtrackerai_start_app/segmentation_widgets/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6039 2023-06-23 10:16:28.000000 idtrackerai-5.1.6/src/idtrackerai_start_app/segmentation_widgets/bkg_widget.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5804 2023-06-15 10:18:22.000000 idtrackerai-5.1.6/src/idtrackerai_start_app/segmentation_widgets/blob_info_widget.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3527 2023-06-15 10:18:22.000000 idtrackerai-5.1.6/src/idtrackerai_start_app/segmentation_widgets/frame_analyzer.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2374 2023-06-19 12:08:12.000000 idtrackerai-5.1.6/src/idtrackerai_start_app/segmentation_widgets/intensity_ths.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6895 2023-06-23 10:48:42.000000 idtrackerai-5.1.6/src/idtrackerai_start_app/segmentation_widgets/open_video_widget.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4997 2023-06-15 10:18:22.000000 idtrackerai-5.1.6/src/idtrackerai_start_app/segmentation_widgets/track_intervals_widget.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2713 2023-05-29 18:15:16.000000 idtrackerai-5.1.6/src/idtrackerai_start_app/tooltips.toml
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-23 14:41:48.178894 idtrackerai-5.1.6/src/idtrackerai_validator/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:15:16.000000 idtrackerai-5.1.6/src/idtrackerai_validator/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      624 2023-06-19 09:27:23.000000 idtrackerai-5.1.6/src/idtrackerai_validator/__main__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      715 2023-05-16 10:39:16.000000 idtrackerai-5.1.6/src/idtrackerai_validator/tooltips.toml
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    34888 2023-06-21 11:04:01.000000 idtrackerai-5.1.6/src/idtrackerai_validator/validation_GUI.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-23 14:41:48.178894 idtrackerai-5.1.6/src/idtrackerai_validator/validator_widgets/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      547 2023-05-29 19:16:39.000000 idtrackerai-5.1.6/src/idtrackerai_validator/validator_widgets/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1986 2023-06-15 10:18:22.000000 idtrackerai-5.1.6/src/idtrackerai_validator/validator_widgets/additional_info.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     9012 2023-06-19 12:13:43.000000 idtrackerai-5.1.6/src/idtrackerai_validator/validator_widgets/errors_explorer.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6063 2023-06-19 12:08:11.000000 idtrackerai-5.1.6/src/idtrackerai_validator/validator_widgets/id_groups.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1511 2023-06-19 12:08:12.000000 idtrackerai-5.1.6/src/idtrackerai_validator/validator_widgets/id_labels.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    12996 2023-06-19 12:08:11.000000 idtrackerai-5.1.6/src/idtrackerai_validator/validator_widgets/interpolator.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4500 2023-06-19 12:08:12.000000 idtrackerai-5.1.6/src/idtrackerai_validator/validator_widgets/mark_properties.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6761 2023-06-19 08:07:06.000000 idtrackerai-5.1.6/src/idtrackerai_validator/validator_widgets/paint_blobs.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4968 2023-06-19 12:10:31.000000 idtrackerai-5.1.6/src/idtrackerai_validator/validator_widgets/setup_points.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-23 14:41:48.178894 idtrackerai-5.1.6/src/idtrackerai_video/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:15:16.000000 idtrackerai-5.1.6/src/idtrackerai_video/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5157 2023-06-15 10:18:22.000000 idtrackerai-5.1.6/src/idtrackerai_video/general_video.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4085 2023-05-29 19:16:39.000000 idtrackerai-5.1.6/src/idtrackerai_video/individual_videos.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2925 2023-06-19 09:26:41.000000 idtrackerai-5.1.6/src/idtrackerai_video/main.py
```

### Comparing `idtrackerai-5.1.5/LICENSE` & `idtrackerai-5.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.5/PKG-INFO` & `idtrackerai-5.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idtrackerai
-Version: 5.1.5
+Version: 5.1.6
 Summary: Idtracker.ai tracks up to 100 unmarked animals from videos recorded in laboratory conditions using artificial intelligence. Free and open source.
 Author: Francisco Romero Ferrero, Mattia G. Bergomi, Francisco J.H. Heras, Ricardo Ribeiro
 Author-email: Jordi Torrents <jordi.torrentsm@gmail.com>
 Project-URL: Homepage, https://idtracker.ai/
 Project-URL: Repository, https://gitlab.com/polavieja_lab/idtrackerai
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `idtrackerai-5.1.5/README.md` & `idtrackerai-5.1.6/README.md`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.5/pyproject.toml` & `idtrackerai-5.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "idtrackerai"
-version = "5.1.5"
+version = "5.1.6"
 authors = [
     { name = "Jordi Torrents", email = "jordi.torrentsm@gmail.com" },
     { name = "Francisco Romero Ferrero" },
     { name = "Mattia G. Bergomi" },
     { name = "Francisco J.H. Heras" },
     { name = "Ricardo Ribeiro" },
 ]
@@ -107,8 +107,9 @@
 ignore_modules = 'qtpy'
 disable = [
     "missing-docstring",
     "fixme",
     "logging-fstring-interpolation",
     "wrong-import-order",
     "invalid-name",
+    "no-name-in-module",
 ]
```

### Comparing `idtrackerai-5.1.5/src/idmatcherai/main.py` & `idtrackerai-5.1.6/src/idmatcherai/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,17 +130,17 @@
         indirect_scores = [
             score_row(indirect_matches[:, assignment], assigned_id)
             for assigned_id, assignment in zip(assigned_ids, assignments)
         ]
 
         with (results_path / "assignments.csv").open("w", encoding="utf_8") as file:
             file.write("identity, assignment, direct score, indirect score\n")
-            for i in range(len(assigned_ids)):
+            for i, assigned_id in enumerate(assigned_ids):
                 file.write(
-                    f"{assigned_ids[i]+1:8d}, {assignments[i]+1:10d},"
+                    f"{assigned_id+1:8d}, {assignments[i]+1:10d},"
                     f" {direct_scores[i]:12.4f}, {indirect_scores[i]:14.4f}\n"
                 )
 
         mean_direct_score = float(np.mean(direct_scores))
         mean_indirect_score = float(np.mean(indirect_scores))
         mean_score = (mean_direct_score + mean_indirect_score) / 2
         save_matrix(
```

### Comparing `idtrackerai-5.1.5/src/idmatcherai/matcher.py` & `idtrackerai-5.1.6/src/idmatcherai/matcher.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.5/src/idtrackerai/__init__.py` & `idtrackerai-5.1.6/src/idtrackerai/__init__.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.5/src/idtrackerai/animals_detection/animals_detection.py` & `idtrackerai-5.1.6/src/idtrackerai/animals_detection/animals_detection.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.5/src/idtrackerai/animals_detection/segmentation.py` & `idtrackerai-5.1.6/src/idtrackerai/animals_detection/segmentation.py`

 * *Files 5% similar despite different names*

```diff
@@ -150,18 +150,15 @@
 def process_frame(
     frame,
     intensity_ths,
     area_ths,
     ROI_mask: np.ndarray | None,
     bkg_model,
     resolution_reduction,
-    sigma_blurring=None,
 ) -> tuple[list[int], list[np.ndarray], np.ndarray]:
-    # frame = gaussian_blur(frame, sigma=sigma_blurring)
-
     # Apply resolution reduction
     if resolution_reduction != 1:
         frame = cv2.resize(
             frame,
             None,  # type: ignore
             fx=resolution_reduction,
             fy=resolution_reduction,
@@ -225,16 +222,14 @@
     _segment_video_in_parallel
 
     """
     logging.info("Segmenting video")
     # avoid computing with all the cores in very large videos. It fills the RAM.
     num_jobs = conf.number_of_parallel_workers
 
-    segmentation_parameters["sigma_blurring"] = conf.SIGMA_GAUSSIAN_BLURRING
-
     logging.info(f"Segmenting {len(episodes)} episodes in {num_jobs} parallel jobs")
 
     inputs = [
         (episode, video_paths, segmentation_parameters, bbox_images_path.parent)
         for episode in episodes
     ]
 
@@ -345,16 +340,14 @@
     ----------
     video_paths : list[str]
     original_ROI: np.ndarray
     episodes: list[tuple(int, int, int, int, int)]
     stat: str
         statistic to compute over the sampled frames
         ('median', 'mean', 'max' or 'min')
-    sigma_gaussian_blur: float
-        sigma of the gaussian kernel to blur each frame
 
     Returns
     -------
     bkg : np.ndarray
         Background model
     """
     if n_frames_for_background is None:
@@ -371,20 +364,14 @@
         return None
 
     background = generate_background_from_frame_stack(frame_stack, stat)
 
     return background
 
 
-def gaussian_blur(frame: np.ndarray, sigma=None) -> np.ndarray:
-    if sigma is not None and sigma > 0:
-        frame = cv2.GaussianBlur(frame, (0, 0), sigma)
-    return frame
-
-
 def to_gray_scale(frame: np.ndarray) -> np.ndarray:
     if frame.ndim > 2:
         frame = cv2.cvtColor(frame, cv2.COLOR_BGR2GRAY)
     return frame
 
 
 def get_bbox_image(frame: np.ndarray, cnt: np.ndarray) -> np.ndarray:
```

### Comparing `idtrackerai-5.1.5/src/idtrackerai/blob.py` & `idtrackerai-5.1.6/src/idtrackerai/blob.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,16 +127,14 @@
     """Identity of the blob after correcting impossible velocity jumps"""
 
     identities_corrected_closing_gaps: list | None = None
     """Identity of the blob after crossings interpolation"""
 
     interpolated_centroids: list | None = None
 
-    centroid: tuple[float, float]
-
     added_by_user: bool = False
 
     forced_crossing: bool = False
     """Indicates if the crossing attribute has been forced by set_individual_with_identity_0_as_crossings()"""
 
     def __init__(
         self,
@@ -172,41 +170,47 @@
 
     @cached_property
     def area(self) -> int:
         return cv2.contourArea(self.contour)
 
     @cached_property
     def bbox_in_frame_coordinates(self) -> tuple[tuple[int, int], tuple[int, int]]:
-        """(x0, y0), (x + w, y + h)"""
-        x, y, w, h = cv2.boundingRect(self.contour)
-        return (x, y), (x + w - 1, y + h - 1)
+        return self.contour.min(0), self.contour.max(0)
 
     @property
     def estimated_body_length(self):
-        x, y, w, h = cv2.boundingRect(self.contour)
-        return int(np.ceil(sqrt(w**2 + h**2)))
+        width, height = np.ptp(self.contour, axis=0)
+        return int(np.ceil(sqrt(width**2 + height**2)))
 
-    def set_contour(self, contour: np.ndarray):
-        if contour.ndim == 3 and contour.shape[1] == 1:
-            # OpenCV returns contours as (n_points, 1, 2)
-            contour = contour[:, 0, :]
-        self.contour = contour
-        M = cv2.moments(contour)
+    @cached_property
+    def centroid(self) -> tuple[float, float]:
+        M = cv2.moments(self.contour)
+        try:
+            return M["m10"] / M["m00"], M["m01"] / M["m00"]
+        except ZeroDivisionError:
+            return tuple(np.mean(self.contour, axis=0))
 
-        if M["m00"] == 0 or M["m00"] == 0:
-            self.centroid = tuple(np.mean(contour, axis=0))
-            self.orientation = 0
-        else:
+    @cached_property
+    def orientation(self) -> float:
+        M = cv2.moments(self.contour)
+        try:
             x = M["m10"] / M["m00"]
             y = M["m01"] / M["m00"]
-            self.centroid = x, y
             a = M["m20"] / M["m00"] - x * x
             b = 2 * (M["m11"] / M["m00"] - x * y)
             c = M["m02"] / M["m00"] - y * y
-            self.orientation = 0.5 * atan2(b, (a - c))
+            return 0.5 * atan2(b, (a - c))
+        except ZeroDivisionError:
+            return 0
+
+    def set_contour(self, contour: np.ndarray):
+        if contour.ndim == 3 and contour.shape[1] == 1:
+            # OpenCV returns contours as (n_points, 1, 2)
+            contour = contour[:, 0, :]
+        self.contour = contour.astype(np.int32, copy=False)
 
     @property
     def is_a_crossing(self) -> bool:
         """Flag indicating whether the blob represents two or more animals
         together.
 
         This attribute is the negative of `is_an_individual` and is set at
@@ -331,18 +335,17 @@
         -------
         bool
             True if the lists of pixels of both blobs have non-empty
             intersection
         """
 
         # Check bounding boxes
-        S_xmin, S_ymin = self.bbox_in_frame_coordinates[0]
-        S_xmax, S_ymax = self.bbox_in_frame_coordinates[1]
-        O_xmin, O_ymin = other.bbox_in_frame_coordinates[0]
-        O_xmax, O_ymax = other.bbox_in_frame_coordinates[1]
+        (S_xmin, S_ymin), (S_xmax, S_ymax) = self.bbox_in_frame_coordinates
+        (O_xmin, O_ymin), (O_xmax, O_ymax) = other.bbox_in_frame_coordinates
+
         if not S_xmax >= O_xmin and O_xmax >= S_xmin:  # x overlap
             return False
         if not S_ymax >= O_ymin and O_ymax >= S_ymin:  # y overlap
             return False
 
         # Check convex hull
         if not cv2.intersectConvexConvex(self.convexHull, other.convexHull)[0]:
@@ -656,16 +659,16 @@
             np.uint8,
         )
         return cv2.fillPoly(
             img=base,
             pts=(self.contour,),
             color=1,
             offset=(
-                -self.bbox_in_frame_coordinates[0][0] + 1,  # bbox_image_pad
-                -self.bbox_in_frame_coordinates[0][1] + 1,  # bbox_image_pad
+                1 - self.bbox_in_frame_coordinates[0][0],  # bbox_image_pad
+                1 - self.bbox_in_frame_coordinates[0][1],  # bbox_image_pad
             ),
         )
 
     def update_centroid(
         self,
         old_centroid: tuple[float, float],
         new_centroid: tuple[float, float],
```

### Comparing `idtrackerai-5.1.5/src/idtrackerai/constants.toml` & `idtrackerai-5.1.6/src/idtrackerai/constants.toml`

 * *Files 9% similar despite different names*

```diff
@@ -27,17 +27,14 @@
 # 'trajectories': saves only the trajectories
 # 'validation': saves the information needed to validate the video
 # 'knowledge_transfer': saves the information needed to perfom identity_transfer
 # to another video
 # 'idmatcher.ai': saves the information needed to perform identity_matching
 # between videos
 
-# Crossing detector advanced parameters
-sigma_gaussian_blurring = ''
-
 # Set None to use the default mode of the system.
 # (see segmentation.py module for details)
 model_area_sd_tolerance = 4
 minimum_number_of_crossings_to_train_crossing_detector = 10
 
 max_images_per_class_crossing_detector = 3000
 learning_rate_dcd = 0.001
```

### Comparing `idtrackerai-5.1.5/src/idtrackerai/crossings_detection/__init__.py` & `idtrackerai-5.1.6/src/idtrackerai/crossings_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.5/src/idtrackerai/crossings_detection/crossing_detector.py` & `idtrackerai-5.1.6/src/idtrackerai/crossings_detection/crossing_detector.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.5/src/idtrackerai/crossings_detection/crossings_dataset.py` & `idtrackerai-5.1.6/src/idtrackerai/crossings_detection/crossings_dataset.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.5/src/idtrackerai/crossings_detection/crossings_network.py` & `idtrackerai-5.1.6/src/idtrackerai/crossings_detection/crossings_network.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.5/src/idtrackerai/crossings_detection/model_area.py` & `idtrackerai-5.1.6/src/idtrackerai/crossings_detection/model_area.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.5/src/idtrackerai/data/test_A.avi` & `idtrackerai-5.1.6/src/idtrackerai/data/test_A.avi`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.5/src/idtrackerai/data/test_B.avi` & `idtrackerai-5.1.6/src/idtrackerai/data/test_B.avi`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.5/src/idtrackerai/fragment.py` & `idtrackerai-5.1.6/src/idtrackerai/fragment.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.5/src/idtrackerai/fragmentation/fragmentation.py` & `idtrackerai-5.1.6/src/idtrackerai/fragmentation/fragmentation.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.5/src/idtrackerai/globalfragment.py` & `idtrackerai-5.1.6/src/idtrackerai/globalfragment.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.5/src/idtrackerai/groundtruth_utils/compute_groundtruth_statistics.py` & `idtrackerai-5.1.6/src/idtrackerai/groundtruth_utils/compute_groundtruth_statistics.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.5/src/idtrackerai/groundtruth_utils/compute_groundtruth_statistics_general.py` & `idtrackerai-5.1.6/src/idtrackerai/groundtruth_utils/compute_groundtruth_statistics_general.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.5/src/idtrackerai/groundtruth_utils/compute_individual_groundtruth_statistics.py` & `idtrackerai-5.1.6/src/idtrackerai/groundtruth_utils/compute_individual_groundtruth_statistics.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.5/src/idtrackerai/groundtruth_utils/generate_groundtruth.py` & `idtrackerai-5.1.6/src/idtrackerai/groundtruth_utils/generate_groundtruth.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.5/src/idtrackerai/groundtruth_utils/generate_individual_groundtruth.py` & `idtrackerai-5.1.6/src/idtrackerai/groundtruth_utils/generate_individual_groundtruth.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.5/src/idtrackerai/list_of_blobs.py` & `idtrackerai-5.1.6/src/idtrackerai/list_of_blobs.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.5/src/idtrackerai/list_of_fragments.py` & `idtrackerai-5.1.6/src/idtrackerai/list_of_fragments.py`

 * *Files 1% similar despite different names*

```diff
@@ -282,15 +282,15 @@
         if scope == "to_the_past":
             fragments_to_the_past = filter(
                 lambda frag: frag.end_frame <= specific_frame, self.fragments
             )
             return sorted(
                 fragments_to_the_past, key=lambda x: x.end_frame, reverse=True
             )
-        elif scope == "to_the_future":
+        if scope == "to_the_future":
             fragments_to_the_future = filter(
                 lambda frag: frag.start_frame >= specific_frame, self.fragments
             )
             return sorted(fragments_to_the_future, key=lambda x: x.start_frame)
         raise ValueError(scope)
 
     def save(self, path: Path | str):
```

### Comparing `idtrackerai-5.1.5/src/idtrackerai/list_of_global_fragments.py` & `idtrackerai-5.1.6/src/idtrackerai/list_of_global_fragments.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.5/src/idtrackerai/network/evaluate.py` & `idtrackerai-5.1.6/src/idtrackerai/network/evaluate.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.5/src/idtrackerai/network/learners.py` & `idtrackerai-5.1.6/src/idtrackerai/network/learners.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.5/src/idtrackerai/network/models.py` & `idtrackerai-5.1.6/src/idtrackerai/network/models.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.5/src/idtrackerai/network/network_params.py` & `idtrackerai-5.1.6/src/idtrackerai/network/network_params.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.5/src/idtrackerai/network/train.py` & `idtrackerai-5.1.6/src/idtrackerai/network/train.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.5/src/idtrackerai/network/utils.py` & `idtrackerai-5.1.6/src/idtrackerai/network/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         logging.info('Using Cuda backend with "%s"', torch.cuda.get_device_name(0))
         return torch.device(0)
     if mps.is_available():
         logging.info("Using MacOS Metal backend")
         return torch.device("mps")
     logging.warning(
         (
-            "[bold red]No graphics device was found available[/], running neural"
+            "[bold red]No graphic device was found available[/], running neural"
             " networks on CPU. This may slow down the training steps."
         ),
         extra={"markup": True},
     )
     return torch.device("cpu")
```

### Comparing `idtrackerai-5.1.5/src/idtrackerai/postprocess/assign_them_all.py` & `idtrackerai-5.1.6/src/idtrackerai/postprocess/assign_them_all.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.5/src/idtrackerai/postprocess/compute_velocity_model.py` & `idtrackerai-5.1.6/src/idtrackerai/postprocess/compute_velocity_model.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.5/src/idtrackerai/postprocess/correct_impossible_velocity_jumps.py` & `idtrackerai-5.1.6/src/idtrackerai/postprocess/correct_impossible_velocity_jumps.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.5/src/idtrackerai/postprocess/erosion.py` & `idtrackerai-5.1.6/src/idtrackerai/postprocess/erosion.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.5/src/idtrackerai/postprocess/get_trajectories.py` & `idtrackerai-5.1.6/src/idtrackerai/postprocess/get_trajectories.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.5/src/idtrackerai/postprocess/identify_non_assigned_with_interpolation.py` & `idtrackerai-5.1.6/src/idtrackerai/postprocess/identify_non_assigned_with_interpolation.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.5/src/idtrackerai/postprocess/trajectories_creation.py` & `idtrackerai-5.1.6/src/idtrackerai/postprocess/trajectories_creation.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.5/src/idtrackerai/postprocess/trajectories_to_csv.py` & `idtrackerai-5.1.6/src/idtrackerai/postprocess/trajectories_to_csv.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,14 @@
             else:
                 attributes_dict[key] = value
 
         json_path = output_dir / npy_path.with_suffix(".attributes.json").name
         json.dump(attributes_dict, json_path.open("w"), indent=4)
     except Exception as e:
         logging.error(e)
-        pass
 
 
 @wrap_exceptions
 def main():
     logging.basicConfig(level=logging.DEBUG, format="%(message)s", datefmt="%H:%M:%S")
 
     parser = ArgumentParser()
```

### Comparing `idtrackerai-5.1.5/src/idtrackerai/tracker/accumulation_manager.py` & `idtrackerai-5.1.6/src/idtrackerai/tracker/accumulation_manager.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.5/src/idtrackerai/tracker/accumulator.py` & `idtrackerai-5.1.6/src/idtrackerai/tracker/accumulator.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.5/src/idtrackerai/tracker/assigner.py` & `idtrackerai-5.1.6/src/idtrackerai/tracker/assigner.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.5/src/idtrackerai/tracker/identity_dataset.py` & `idtrackerai-5.1.6/src/idtrackerai/tracker/identity_dataset.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.5/src/idtrackerai/tracker/identity_network.py` & `idtrackerai-5.1.6/src/idtrackerai/tracker/identity_network.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.5/src/idtrackerai/tracker/identity_transfer.py` & `idtrackerai-5.1.6/src/idtrackerai/tracker/identity_transfer.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.5/src/idtrackerai/tracker/pre_trainer.py` & `idtrackerai-5.1.6/src/idtrackerai/tracker/pre_trainer.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.5/src/idtrackerai/tracker/tracker.py` & `idtrackerai-5.1.6/src/idtrackerai/tracker/tracker.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.5/src/idtrackerai/utils/__init__.py` & `idtrackerai-5.1.6/src/idtrackerai/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.5/src/idtrackerai/utils/check_PyPI_version.py` & `idtrackerai-5.1.6/src/idtrackerai/utils/check_PyPI_version.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.5/src/idtrackerai/utils/confparams.py` & `idtrackerai-5.1.6/src/idtrackerai/utils/confparams.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import logging
+from typing import Any
 
 
 class ConfParams:
     parameters: dict = {}
 
     @staticmethod
     def pprint_dict(d: dict) -> str:
         text = ""
         pad = min(max(map(len, d.keys())), 25)
         for key, value in d.items():
             text += f"\n[bold]{key:>{pad}}[/] = {repr(value)}"
         return text
 
-    def set_dict(self, data: dict, verbose=False):
+    def set_dict(self, data: dict[str, Any], verbose=False):
+        logging.info("Setting %d keys in ConfParams", len(data))
         data = {key.lower(): value for key, value in data.items()}
         if verbose:
             logging.info(self.pprint_dict(data), extra={"markup": True})
         self.parameters = data
 
     def __getattr__(self, name: str):
         lower_name = name.lower()
```

### Comparing `idtrackerai-5.1.5/src/idtrackerai/utils/init_logger.py` & `idtrackerai-5.1.6/src/idtrackerai/utils/init_logger.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 import logging
 import os
 import sys
 from datetime import datetime
 from importlib import metadata
 from pathlib import Path
 from platform import platform
+from typing import Callable
 
 from rich.console import Console
 from rich.logging import RichHandler
 
 from .check_PyPI_version import check_version_on_console_thread
 
 LOG_FILE_PATH = Path("idtrackerai.log").resolve()
 
 
 class CustomError(Exception):
     pass
 
 
-def initLogger(testing=False, check_version=True, level: int = logging.DEBUG):
+def initLogger(check_version=True, level: int = logging.DEBUG):
     logger_width_when_no_terminal = 130
     try:
         os.get_terminal_size()
     except OSError:
         # stdout is sent to file. We define logger width to a constant
         size = logger_width_when_no_terminal
     else:
@@ -34,40 +35,41 @@
 
     # The first handler is the terminal, the second one the .log file,
     # both rendered with Rich and full logging (level=0)
     logging.basicConfig(
         level=level,
         format="%(message)s",
         datefmt="%H:%M:%S",
-        force=not testing,
+        force=True,
         handlers=[
             RichHandler(console=Console(width=size)),
             RichHandler(
                 console=Console(
                     file=LOG_FILE_PATH.open("w", encoding="utf_8"),  # noqa SIM115
                     width=logger_width_when_no_terminal,
                 )
             ),
         ],
     )
 
+    logging.captureWarnings(True)
     logging.info("Welcome to idtracker.ai")
     logging.debug(
         f"Running idtracker.ai '{metadata.version('idtrackerai')}'"
         f" on Python '{sys.version.split(' ')[0]}'\nPlatform: '{platform(True)}'"
         "\nDate: "
         + str(datetime.now()).split(".")[0]
     )
     logging.info("Writing log in %s", LOG_FILE_PATH)
 
     if check_version:
         check_version_on_console_thread()
 
 
-def wrap_exceptions(main_function):
+def wrap_exceptions(main_function: Callable):
     def applicator(*args, **kwargs):
         try:
             return main_function(*args, **kwargs)
         except CustomError as error:
             logging.critical(error, exc_info=False)
             return False
         except Exception as error:
```

### Comparing `idtrackerai-5.1.5/src/idtrackerai/utils/py_utils.py` & `idtrackerai-5.1.6/src/idtrackerai/utils/py_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -415,13 +415,13 @@
     with the class attributes"""
     class_attr = obj.__class__.__dict__
 
     attributes_to_remove: list[str] = [
         attr
         for attr, value in obj.__dict__.items()
         if attr in class_attr
-        and type(class_attr[attr]) == type(value)
+        and isinstance(class_attr[attr], type(value))
         and class_attr[attr] == value
     ]
 
     for attr in attributes_to_remove:
         delattr(obj, attr)
```

### Comparing `idtrackerai-5.1.5/src/idtrackerai/video.py` & `idtrackerai-5.1.6/src/idtrackerai/video.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,30 +128,27 @@
         output_dir: Path | None,
         session,
         tracking_intervals: list | None,
         resolution_reduction: float,
         roi_list: list[str] | None,
         use_bkg: bool,
         track_wo_identities: bool,
-        sigma_gaussian_blurring: float | None,
         check_segmentation: bool,
         identity_transfer: bool,
         knowledge_transfer_folder: Path | None,
         bkg_model,
         **kwargs,
     ):
         """Initializes a video object
 
         Parameters
         ----------
         video_path : str
             Path to a video file
         """
-        if sigma_gaussian_blurring is None:
-            sigma_gaussian_blurring = conf.SIGMA_GAUSSIAN_BLURRING
         if kwargs:
             logging.info(
                 f"Ignoring the next arguments in Video.__init__():\n{kwargs.keys()}"
             )
 
         logging.debug("Initializing Video object")
         self.use_bkg = use_bkg
@@ -161,15 +158,14 @@
         self.intensity_ths = intensity_ths
         self.area_ths = area_ths
         self.knowledge_transfer_folder = knowledge_transfer_folder
         self.resolution_reduction = resolution_reduction
         self.number_of_animals = int(number_of_animals)
         """Number of animals in the video indicated by user"""
         self.set_video_paths(video_paths)
-        self.sigma_gaussian_blurring = sigma_gaussian_blurring
         self.data_policy: str = conf.DATA_POLICY
         self.frames_per_episode: int = conf.frames_per_episode
         self.version = metadata.version("idtrackerai")
         self.protocol3_action: str = conf.protocol3_action
         self.accumulation_statistics_data = [None] * (
             conf.MAXIMUM_NUMBER_OF_PARACHUTE_ACCUMULATIONS + 1
         )
@@ -617,14 +613,15 @@
                 continue
 
             logging.info(f"All video files found on {folder_candidate}")
             found = True
             break
         else:
             found = False
+            candidate_new_video_paths = []
             logging.error(f"Video file paths not found: {self.video_paths}")
 
         need_to_save = False
         if self.session_folder != new_video_object_path:
             logging.info(
                 f"Updated session folder from {self.session_folder} to"
                 f" {new_video_object_path}"
@@ -637,16 +634,18 @@
             self.video_paths = candidate_new_video_paths
             need_to_save = True
 
         if need_to_save:
             self.save()
 
     @staticmethod
-    def assert_video_paths(video_paths: Iterable[Path | str]):
-        accepted_extensions = conf.AVAILABLE_VIDEO_EXTENSION
+    def assert_video_paths(
+        video_paths: Iterable[Path | str], accepted_extensions: list[str] | None = None
+    ):
+        accepted_extensions = accepted_extensions or conf.AVAILABLE_VIDEO_EXTENSION
         assert video_paths, "Empty video_paths list"
 
         for path in video_paths:
             path = Path(path).expanduser().resolve()
             assert path.is_file(), f"Video file {path} not found"
             assert (
                 path.suffix in accepted_extensions
```

### Comparing `idtrackerai-5.1.5/src/idtrackerai.egg-info/PKG-INFO` & `idtrackerai-5.1.6/src/idtrackerai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idtrackerai
-Version: 5.1.5
+Version: 5.1.6
 Summary: Idtracker.ai tracks up to 100 unmarked animals from videos recorded in laboratory conditions using artificial intelligence. Free and open source.
 Author: Francisco Romero Ferrero, Mattia G. Bergomi, Francisco J.H. Heras, Ricardo Ribeiro
 Author-email: Jordi Torrents <jordi.torrentsm@gmail.com>
 Project-URL: Homepage, https://idtracker.ai/
 Project-URL: Repository, https://gitlab.com/polavieja_lab/idtrackerai
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `idtrackerai-5.1.5/src/idtrackerai.egg-info/SOURCES.txt` & `idtrackerai-5.1.6/src/idtrackerai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.5/src/idtrackerai_GUI_tools/GUI_main_base.py` & `idtrackerai-5.1.6/src/idtrackerai_GUI_tools/GUI_main_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import json
 import logging
+from importlib import metadata
 from pathlib import Path
 
-from qtpy.QtCore import Qt, QThread, QTimer, QUrl, Signal
+from qtpy import API_NAME
+from qtpy.QtCore import Qt, QThread, QTimer, QUrl, Signal  # type: ignore
 from qtpy.QtGui import QAction, QCloseEvent, QDesktopServices, QGuiApplication, QIcon
 from qtpy.QtWidgets import (
     QApplication,
     QDialog,
     QHBoxLayout,
     QLayout,
     QMainWindow,
@@ -21,15 +23,21 @@
 from idtrackerai.utils import check_version
 
 from .themes import dark, light
 
 
 class GUIBase(QMainWindow):
     def __init__(self):
-        logging.debug(f"Initializing {self.__class__.__name__}")
+        try:
+            QT_version = metadata.version(API_NAME)
+        except metadata.PackageNotFoundError:
+            QT_version = "unknown version"
+        logging.info(
+            "Initializing %s with %s %s", self.__class__.__name__, API_NAME, QT_version
+        )
         if "Fusion" in QStyleFactory.keys():  # noqa SIM118
             QApplication.setStyle("Fusion")
         super().__init__()
 
         QApplication.setApplicationDisplayName("idtracker.ai")
         QApplication.setApplicationName("idtracker.ai")
         self.setWindowIcon(QIcon(str(Path(__file__).parent / "logo_256.png")))
```

### Comparing `idtrackerai-5.1.5/src/idtrackerai_GUI_tools/__init__.py` & `idtrackerai-5.1.6/src/idtrackerai_GUI_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.5/src/idtrackerai_GUI_tools/cmap_gist_rainbow.dat` & `idtrackerai-5.1.6/src/idtrackerai_GUI_tools/cmap_gist_rainbow.dat`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.5/src/idtrackerai_GUI_tools/logo_256.png` & `idtrackerai-5.1.6/src/idtrackerai_GUI_tools/logo_256.png`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.5/src/idtrackerai_GUI_tools/themes.py` & `idtrackerai-5.1.6/src/idtrackerai_GUI_tools/themes.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.5/src/idtrackerai_GUI_tools/tooltips.toml` & `idtrackerai-5.1.6/src/idtrackerai_GUI_tools/tooltips.toml`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.5/src/idtrackerai_GUI_tools/widgets_utils/canvas.py` & `idtrackerai-5.1.6/src/idtrackerai_GUI_tools/widgets_utils/canvas.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 from dataclasses import dataclass
 from math import sqrt
 
-from qtpy.QtCore import QPoint, QPointF, Qt, Signal
+from qtpy.QtCore import QPoint, QPointF, Qt, Signal  # type: ignore
 from qtpy.QtGui import (
     QColor,
     QColorConstants,
     QMouseEvent,
     QPainter,
     QPaintEvent,
     QPolygon,
@@ -26,14 +26,18 @@
 
     def distance_to(self, point: tuple[float, float]):
         return sqrt(self.sq_distance_to(point))
 
     def sq_distance_to(self, point: tuple[float, float]):
         return (point[0] - self.xy_data[0]) ** 2 + (point[1] - self.xy_data[1]) ** 2
 
+    @property
+    def int_xy_data(self):
+        return int(self.xy_data[0] + 0.5), int(self.xy_data[1] + 0.5)
+
 
 class CanvasPainter(QPainter):
     def __init__(self, parent, zoom: float):
         self.applied_zoom = zoom
         super().__init__(parent)
 
     def drawPolygonFromVertices(self, vertices, scale: float):
```

### Comparing `idtrackerai-5.1.5/src/idtrackerai_GUI_tools/widgets_utils/custom_list.py` & `idtrackerai-5.1.6/src/idtrackerai_GUI_tools/widgets_utils/custom_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from qtpy.QtCore import QEvent, QSize, Qt, QTimer, Signal
+from qtpy.QtCore import QEvent, QSize, Qt, QTimer, Signal  # type: ignore
 from qtpy.QtGui import QColor, QFocusEvent, QPainter, QPixmap
 from qtpy.QtWidgets import (
     QHBoxLayout,
     QLabel,
     QListWidget,
     QListWidgetItem,
     QToolButton,
```

### Comparing `idtrackerai-5.1.5/src/idtrackerai_GUI_tools/widgets_utils/other_utils.py` & `idtrackerai-5.1.6/src/idtrackerai_GUI_tools/widgets_utils/other_utils.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.5/src/idtrackerai_GUI_tools/widgets_utils/video_paths_holder.py` & `idtrackerai-5.1.6/src/idtrackerai_GUI_tools/widgets_utils/video_paths_holder.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.5/src/idtrackerai_GUI_tools/widgets_utils/video_player.py` & `idtrackerai-5.1.6/src/idtrackerai_GUI_tools/widgets_utils/video_player.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 from contextlib import suppress
 from pathlib import Path
 from time import perf_counter
 
 import numpy as np
 import toml
-from qtpy.QtCore import QEvent, QRectF, QSize, Qt, QTimer, Signal
+from qtpy.QtCore import QEvent, QRectF, QSize, Qt, QTimer, Signal  # type: ignore
 from qtpy.QtGui import (
     QAction,
     QCloseEvent,
     QColor,
     QColorConstants,
     QIcon,
     QImage,
```

### Comparing `idtrackerai-5.1.5/src/idtrackerai_start_app/__main__.py` & `idtrackerai-5.1.6/src/idtrackerai_start_app/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,14 @@
     )
 
 import toml
 
 from idtrackerai.utils import (
     CustomError,
     check_version_on_console_thread,
-    conf,
     initLogger,
     pprint_dict,
     wrap_exceptions,
 )
 
 from .arg_parser import parse_args
 
@@ -54,37 +53,35 @@
 
         for key, value in toml_dict.items():
             if value == "":
                 toml_dict[key] = None
         if name:
             logging.info(pprint_dict(toml_dict, name), extra={"markup": True})
         return toml_dict
-    except Exception:
-        raise CustomError(f"Could not read {path}, bad format")
+    except Exception as exc:
+        raise CustomError(f"Could not read {path}.\n" + str(exc)) from exc
 
 
 @wrap_exceptions
 def main() -> bool:
     """The command `idtrackerai` runs this function"""
     parameters = {}
     initLogger(check_version=False)
 
-    constants = load_toml((files("idtrackerai") / "constants.toml"))  # type: ignore
-    parameters.update(constants)
+    parameters.update(load_toml((files("idtrackerai") / "constants.toml")))  # type: ignore
 
     if Path("local_settings.py").is_file():
         logging.warning("Deprecated local_settings format found in ./local_settings.py")
 
     local_settings_path = Path("local_settings.toml")
     if local_settings_path.is_file():
         local_settings_dict = load_toml(local_settings_path, "Local settings")
         parameters.update(local_settings_dict)
 
-    conf.set_dict(constants)  # TODO for weird parameters for GUI
-    terminal_args = parse_args(constants)
+    terminal_args = parse_args(parameters)
     ready_to_track = terminal_args.pop("track")
 
     if "general_settings" in terminal_args:
         general_settings = load_toml(
             terminal_args.pop("general_settings"), "General settings"
         )
         parameters.update(general_settings)
@@ -120,21 +117,21 @@
         return RunIdTrackerAi(parameters).track_video()
     return False
 
 
 def run_segmentation_GUI(params: dict):
     try:
         from idtrackerai_start_app.segmentation_GUI import SegmentationGUI
-    except ImportError:
+    except ImportError as exc:
         raise CustomError(
             "\n\tRUNNING AN IDTRACKER.AI INSTALLATION WITHOUT ANY QT BINDING.\n\tGUIs"
             " are not available, only tracking directly from the terminal with the"
             " `--track` flag.\n\tRun `pip install pyqt5` or `pip install pyqt6` to"
             " build a Qt binding."
-        )
+        ) from exc
     app = QApplication(sys.argv)
     window = SegmentationGUI(params)
     window.show()
     app.exec()
 
 
 @wrap_exceptions
@@ -144,15 +141,15 @@
     from .run_idtrackerai import RunIdTrackerAi
 
     COMPRESSED_VIDEO_PATH = Path(str(files("idtrackerai"))) / "data" / "test_B.avi"
 
     video_path = Path.cwd() / COMPRESSED_VIDEO_PATH.name
     shutil.copyfile(COMPRESSED_VIDEO_PATH, video_path)
 
-    initLogger(testing=True)
+    initLogger()
 
     params = load_toml((files("idtrackerai") / "constants.toml"))  # type: ignore
     params.update(
         {
             "session": "test",
             "video_paths": video_path,
             "tracking_intervals": None,
```

### Comparing `idtrackerai-5.1.5/src/idtrackerai_start_app/all_valid_parameters.dat` & `idtrackerai-5.1.6/src/idtrackerai_start_app/all_valid_parameters.dat`

 * *Files 11% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 identity_transfer
 resolution_reduction
 tracking_intervals
 use_bkg
 check_segmentation
 track_wo_identities
 roi_list
-sigma_gaussian_blurring
 model_area_sd_tolerance
 minimum_number_of_crossings_to_train_crossing_detector
 max_images_per_class_crossing_detector
 learning_rate_dcd
 keep_prob_dcd
 batch_size_dcd
 batch_size_predictions_dcd
```

### Comparing `idtrackerai-5.1.5/src/idtrackerai_start_app/arg_parser.py` & `idtrackerai-5.1.6/src/idtrackerai_start_app/arg_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,15 @@
     )
     add_argument(
         "video_paths",
         help="List of paths to the video files to track",
         type=path,
         nargs="+",
     )
-    add_argument("session", help="Name of the session", type=str, default=None)
+    add_argument("session", help="Name of the session", type=str)
     add_argument(
         "track_wo_identities",
         "Track the video ignoring identities (without AI)",
         type=Bool,
     )
     add_argument(
         "CONVERT_TRAJECTORIES_TO_CSV_AND_JSON",
```

### Comparing `idtrackerai-5.1.5/src/idtrackerai_start_app/run_idtrackerai.py` & `idtrackerai-5.1.6/src/idtrackerai_start_app/run_idtrackerai.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,14 @@
             "output_dir",
             "session",
             "tracking_intervals",
             "resolution_reduction",
             "roi_list",
             "use_bkg",
             "track_wo_identities",
-            "sigma_gaussian_blurring",
             "check_segmentation",
             "identity_transfer",
             "knowledge_transfer_folder",
         )
 
         if (
             user_parameters["number_of_animals"] == 0
```

### Comparing `idtrackerai-5.1.5/src/idtrackerai_start_app/segmentation_GUI.py` & `idtrackerai-5.1.6/src/idtrackerai_start_app/segmentation_GUI.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,19 +47,27 @@
 
         self.setWindowTitle("Segmentation App")
         self.user_params = GUI_out_params
         self.documentation_url = (
             "https://idtracker.ai/en/latest/user_guide/segmentation_app.html"
         )
 
-        self.open_widget = OpenVideoWidget(self)
+        self.open_widget = OpenVideoWidget(
+            self,
+            GUI_out_params["available_video_extension"],
+            GUI_out_params["frames_per_episode"],
+        )
         self.videoPlayer = VideoPlayer(self)
         self.frame_analyzer = FrameAnalyzer()
         self.blobInfo = BlobInfoWidget()
-        self.bkg_widget = BkgWidget(self)
+        self.bkg_widget = BkgWidget(
+            self,
+            GUI_out_params["number_of_frames_for_background"],
+            GUI_out_params["background_subtraction_stat"],
+        )
         self.ROI_Widget = ROIWidget(self)
         self.tracking_interval = TrackingIntervalsWidget(self)
         self.widgets_to_close.append(self.videoPlayer)
 
         self.intensity_thresholds = IntensityThresholds(self, min=0, max=255)
         self.area_thresholds = LabelRangeSlider(
             parent=self, min=1, max=60000, block_upper=False
```

### Comparing `idtrackerai-5.1.5/src/idtrackerai_start_app/segmentation_widgets/ROI_widget.py` & `idtrackerai-5.1.6/src/idtrackerai_start_app/segmentation_widgets/ROI_widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 from cv2 import fitEllipse
-from qtpy.QtCore import Qt, Signal
+from qtpy.QtCore import Qt, Signal  # type: ignore
 from qtpy.QtGui import QColor, QPainterPath
 from qtpy.QtWidgets import (
     QCheckBox,
     QDialog,
     QGridLayout,
     QHBoxLayout,
     QListView,
```

### Comparing `idtrackerai-5.1.5/src/idtrackerai_start_app/segmentation_widgets/bkg_widget.py` & `idtrackerai-5.1.6/src/idtrackerai_start_app/segmentation_widgets/bkg_widget.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-from qtpy.QtCore import Qt, QThread, QTimer, Signal
+from qtpy.QtCore import Qt, QThread, QTimer, Signal  # type: ignore
 from qtpy.QtGui import QImage, QPainter, QPixmap
 from qtpy.QtWidgets import (
     QCheckBox,
     QDialog,
     QHBoxLayout,
     QMessageBox,
     QProgressDialog,
@@ -11,50 +11,54 @@
     QWidget,
 )
 
 from idtrackerai.animals_detection.segmentation import (
     generate_background_from_frame_stack,
     generate_frame_stack,
 )
-from idtrackerai.utils import conf
 from idtrackerai_GUI_tools import Canvas
 
 
 class BkgComputationThread(QThread):
     progress_changed = Signal(int)
 
-    def __init__(self):
+    def __init__(self, n_frames_for_background: int, background_stat: str):
         super().__init__()
         self.frame_stack = None
         self.bkg = None
         self.abort = False
+        self.n_frames_for_background = n_frames_for_background
+        self.background_stat = background_stat
         self.finished.connect(
-            lambda: self.progress_changed.emit(conf.NUMBER_OF_FRAMES_FOR_BACKGROUND)
+            lambda: self.progress_changed.emit(n_frames_for_background)
         )
 
     def set_parameters(self, video_paths, episodes):
         self.video_paths = video_paths
         self.episodes = episodes
 
     def run(self):
         self.abort = False
         if self.bkg is None:
             if self.frame_stack is None:
                 self.frame_stack = generate_frame_stack(
                     self.video_paths,
                     self.episodes,
-                    progress_bar=self.progress_changed,
-                    abort=lambda: self.abort,
+                    self.n_frames_for_background,
+                    self.progress_changed,
+                    lambda: self.abort,
                 )
             if self.abort:
                 self.frame_stack = None
                 self.abort = False
                 return
 
-            self.bkg = generate_background_from_frame_stack(self.frame_stack)
+            self.bkg = generate_background_from_frame_stack(
+                self.frame_stack, self.background_stat
+            )
 
             if self.abort:
                 self.frame_stack = None
                 self.bkg = None
                 self.abort = False
                 return
 
@@ -99,29 +103,27 @@
         QTimer.singleShot(0, lambda: self.canvas.adjust_zoom_to(width, height))
         super().exec()
 
 
 class BkgWidget(QWidget):
     new_bkg_data = Signal(object)
 
-    def __init__(self, parent: QWidget):
+    def __init__(
+        self, parent: QWidget, n_frames_for_background: int, background_stat: str
+    ):
         super().__init__()
         self.checkBox = QCheckBox("Background subtraction")
         self.checkBox.stateChanged.connect(self.CheckBox_changed)
         self.view_bkg = QToolButton()
         self.view_bkg.setText("View background")
-        self.bkg_thread = BkgComputationThread()
+        self.bkg_thread = BkgComputationThread(n_frames_for_background, background_stat)
         self.view_bkg.setFocusPolicy(Qt.FocusPolicy.NoFocus)
         self.view_bkg.setVisible(False)
         self.progress_bar = QProgressDialog(
-            "Computing background",
-            "Cancel",
-            0,
-            conf.NUMBER_OF_FRAMES_FOR_BACKGROUND,
-            parent,
+            "Computing background", "Cancel", 0, n_frames_for_background, parent
         )
         self.progress_bar.cancel()
         self.progress_bar.setMinimumDuration(1000)
         self.progress_bar.setModal(True)
         self.progress_bar.canceled.connect(self.bkg_thread.quit)
         self.view_bkg.clicked.connect(self.view_bkg_clicked)
```

### Comparing `idtrackerai-5.1.5/src/idtrackerai_start_app/segmentation_widgets/blob_info_widget.py` & `idtrackerai-5.1.6/src/idtrackerai_start_app/segmentation_widgets/blob_info_widget.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.5/src/idtrackerai_start_app/segmentation_widgets/frame_analyzer.py` & `idtrackerai-5.1.6/src/idtrackerai_start_app/segmentation_widgets/frame_analyzer.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.5/src/idtrackerai_start_app/segmentation_widgets/intensity_ths.py` & `idtrackerai-5.1.6/src/idtrackerai_start_app/segmentation_widgets/intensity_ths.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from qtpy.QtCore import Qt, Signal
+from qtpy.QtCore import Qt, Signal  # type: ignore
 from qtpy.QtWidgets import QHBoxLayout, QLabel, QWidget
 
 from idtrackerai_GUI_tools import LabeledSlider, LabelRangeSlider
 
 
 class IntensityThresholds(QWidget):
     newValue = Signal(object)
```

### Comparing `idtrackerai-5.1.5/src/idtrackerai_start_app/segmentation_widgets/open_video_widget.py` & `idtrackerai-5.1.6/src/idtrackerai_start_app/segmentation_widgets/open_video_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 from pathlib import Path
 from typing import Sequence
 
-from qtpy.QtCore import Qt, Signal
+from qtpy.QtCore import Qt, Signal  # type: ignore
 from qtpy.QtGui import QFocusEvent
 from qtpy.QtWidgets import (
     QFileDialog,
     QHBoxLayout,
     QListView,
     QListWidget,
     QMessageBox,
     QPushButton,
     QSizePolicy,
     QWidget,
 )
 
 from idtrackerai import Video
-from idtrackerai.utils import conf
 from idtrackerai_GUI_tools import WrappedLabel, key_event_modifier
 
 
 class AdaptativeList(QListWidget):
     def __init__(self):
         super().__init__()
         self.setAlternatingRowColors(True)
@@ -59,19 +58,22 @@
 
 class OpenVideoWidget(QWidget):
     new_video_paths = Signal(list, tuple, int, int, list)
     path_clicked = Signal(int)
     video_paths_reordered = Signal(list)
     new_episodes = Signal(list, object)
 
-    def __init__(self, parent=None):
+    def __init__(
+        self, parent, avaliable_extensions: list[str], frames_per_episode: int
+    ):
         super().__init__()
         self.setLayout(QHBoxLayout())
         self.parent_widget = parent
-        self.avaliable_extensions = conf.AVAILABLE_VIDEO_EXTENSION
+        self.avaliable_extensions = avaliable_extensions
+        self.frames_per_episode = frames_per_episode
         self.extension_filter = (
             "Video (*" + " *".join(self.avaliable_extensions) + ");; All (*)"
         )
         self.button_open = QPushButton("Open video(s)")
         self.button_open.setShortcut("Ctrl+O")
         self.button_open.setFocusPolicy(Qt.FocusPolicy.NoFocus)
         self.button_open.clicked.connect(self.button_open_clicked)
@@ -101,15 +103,15 @@
         for video_path in self.video_paths:
             n_frames = self.video_path_n_frames[video_path]
             self.video_path_start[video_path] = (i, i + n_frames)
             i += n_frames
         self.video_paths_reordered.emit(self.video_paths)
         self.n_frames, video_paths_n_frames, _, self.episodes = (
             Video.get_processing_episodes(
-                self.video_paths, conf.frames_per_episode, self.tracking_intervals
+                self.video_paths, self.frames_per_episode, self.tracking_intervals
             )
         )
         self.new_episodes.emit(self.video_paths, self.episodes)
 
     def button_open_clicked(self):
         video_paths, _ = QFileDialog.getOpenFileNames(
             self.parent_widget,
@@ -119,15 +121,15 @@
         self.open_video_paths(sorted(video_paths))
 
     def open_video_paths(self, video_paths: Sequence[str | Path] | None):
         if not video_paths:
             return
         try:
             video_paths = [Path(path).expanduser().resolve() for path in video_paths]
-            Video.assert_video_paths(video_paths)
+            Video.assert_video_paths(video_paths, self.avaliable_extensions)
             self.video_width, self.video_height, self.fps = (
                 Video.get_info_from_video_paths(video_paths)
             )
         except (ValueError, AssertionError) as e:
             QMessageBox.warning(self, "Video paths error", str(e))
             return
 
@@ -139,15 +141,15 @@
             self.list_of_files.addItems(map(str, video_paths))
 
         self.single_file_label.setVisible(self.single_file)
         self.list_of_files.setVisible(not self.single_file)
 
         self.n_frames, video_paths_n_frames, _, self.episodes = (
             Video.get_processing_episodes(
-                video_paths, conf.frames_per_episode, self.tracking_intervals
+                video_paths, self.frames_per_episode, self.tracking_intervals
             )
         )
         self.video_path_n_frames = dict(zip(self.video_paths, video_paths_n_frames))
 
         self.video_path_start = {}
         i = 0
         for video_path in self.video_paths:
@@ -168,15 +170,15 @@
         self.tracking_intervals = tracking_intervals
 
         if not hasattr(self, "video_paths"):
             return
 
         self.n_frames, video_paths_n_frames, _, self.episodes = (
             Video.get_processing_episodes(
-                self.video_paths, conf.frames_per_episode, self.tracking_intervals
+                self.video_paths, self.frames_per_episode, self.tracking_intervals
             )
         )
         self.new_episodes.emit(self.video_paths, self.episodes)
 
     @property
     def video_paths(self):
         return self.getVideoPaths()
```

### Comparing `idtrackerai-5.1.5/src/idtrackerai_start_app/segmentation_widgets/track_intervals_widget.py` & `idtrackerai-5.1.6/src/idtrackerai_start_app/segmentation_widgets/track_intervals_widget.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.5/src/idtrackerai_start_app/tooltips.toml` & `idtrackerai-5.1.6/src/idtrackerai_start_app/tooltips.toml`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.5/src/idtrackerai_validator/__main__.py` & `idtrackerai-5.1.6/src/idtrackerai_validator/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,19 +7,15 @@
 from idtrackerai.utils import initLogger, wrap_exceptions
 from idtrackerai_validator.validation_GUI import ValidationGUI
 
 
 def input_args():
     parser = ArgumentParser()
     parser.add_argument(
-        "session_directory",
-        help="Session directory to validate",
-        type=Path,
-        default=None,
-        nargs="?",
+        "session_directory", help="Session directory to validate", type=Path, nargs="?"
     )
     return parser.parse_args()
 
 
 @wrap_exceptions
 def main():
     args = input_args()
```

### Comparing `idtrackerai-5.1.5/src/idtrackerai_validator/tooltips.toml` & `idtrackerai-5.1.6/src/idtrackerai_validator/tooltips.toml`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.5/src/idtrackerai_validator/validation_GUI.py` & `idtrackerai-5.1.6/src/idtrackerai_validator/validation_GUI.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 import sys
 from enum import Enum
 from pathlib import Path
 
 import numpy as np
 import toml
-from qtpy.QtCore import Qt, QThread, QTimer, Signal
+from qtpy.QtCore import Qt, QThread, QTimer, Signal  # type: ignore
 from qtpy.QtGui import QAction, QCloseEvent, QColor, QKeyEvent
 from qtpy.QtWidgets import (
     QApplication,
     QCheckBox,
     QDialog,
     QFileDialog,
     QHBoxLayout,
@@ -71,25 +71,24 @@
 
 
 class DblClickDialog(QDialog):
     class Answers(Enum):
         Cancel = 0
         ChangeId = 1
         Interpolate = 2
+        Reset = 3
 
     def __init__(self, parent: QWidget, n_animals: int):
         super().__init__(parent)
         self.spinbox = QSpinBox()
         self.spinbox.setMinimum(-1)
         self.spinbox.setMaximum(n_animals)
         main_layout = QVBoxLayout()
         self.setLayout(main_layout)
-        self.description = QLabel(
-            "0 means null identity and -1 means\nto return to assigned identity"
-        )
+        self.description = QLabel("0 means null identity")
         self.description.setAlignment(Qt.AlignmentFlag.AlignCenter)
         self.description.setWordWrap(True)
 
         self.propagate = QCheckBox("Propagate identity")
         self.propagate.setChecked(True)
         spin_row = QHBoxLayout()
         spin_row.addWidget(QLabel("New identity:"))
@@ -100,22 +99,27 @@
         style = self.style()
         cancel_btn = QPushButton(
             style.standardIcon(style.StandardPixmap.SP_DialogCancelButton), "Cancel"
         )
         change_id_btn = QPushButton(
             style.standardIcon(style.StandardPixmap.SP_DialogOkButton), "Change id"
         )
+        reset_id_btn = QPushButton(
+            style.standardIcon(style.StandardPixmap.SP_BrowserReload), "Reset id"
+        )
         self.interp_btn = QPushButton("Interpolate\nhere")
-        btn_row.addWidget(self.interp_btn)
         btn_row.addWidget(cancel_btn)
+        btn_row.addWidget(self.interp_btn)
+        btn_row.addWidget(reset_id_btn)
         btn_row.addWidget(change_id_btn)
         change_id_btn.setDefault(True)
 
         cancel_btn.clicked.connect(lambda: self.done(self.Answers.Cancel.value))
         change_id_btn.clicked.connect(lambda: self.done(self.Answers.ChangeId.value))
+        reset_id_btn.clicked.connect(lambda: self.done(self.Answers.Reset.value))
         self.interp_btn.clicked.connect(
             lambda: self.done(self.Answers.Interpolate.value)
         )
 
         main_layout.addLayout(spin_row)
         main_layout.addWidget(self.description)
         main_layout.addLayout(btn_row)
@@ -126,18 +130,15 @@
         if default is not None:
             self.spinbox.setValue(default)
         self.interp_btn.setEnabled(default is not None and default > 0)
 
         self.spinbox.setFocus()
         answer = self.Answers(super().exec())
 
-        new_id = self.spinbox.value()
-        if new_id == -1:
-            new_id = None
-        return answer, new_id, self.propagate.isChecked()
+        return answer, self.spinbox.value(), self.propagate.isChecked()
 
 
 class LoadSessionObjects(QThread):
     """Independent thread to load lists of Blobs/Fragments
     because they take too long for large sessions."""
 
     blobs: ListOfBlobs | None = None
@@ -156,14 +157,17 @@
         ):
             try:
                 self.blobs = ListOfBlobs.load(path)
                 break
             except FileNotFoundError:
                 pass
         else:
+            logging.warning(
+                "List of blobs not found in %s", self.video.blobs_path.parent
+            )
             self.blobs = None
 
         try:
             self.fragments = ListOfFragments.load(
                 self.video.fragments_path, reconnect=False
             ).fragments
             for index, fragment in enumerate(self.fragments):
@@ -426,52 +430,33 @@
 
     def keyPressEvent(self, event: QKeyEvent):
         if event.key() in (Qt.Key.Key_Return, Qt.Key.Key_Enter):
             self.id_groups.uncheck_edit_buttons()
             self.setup_points.add.setChecked(False)
 
     def go_to_error(
-        self,
-        kind: str,
-        start: int,
-        length: int,
-        where: np.ndarray | None,
-        identity: int,
+        self, kind: str, start: int, length: int, where: np.ndarray, identity: int
     ):
-        if where is None:
-            where = self.trajectories[start]
-            if kind == "No id":
-                for blob in self.blobs.blobs_in_video[start]:
-                    for blob_id, centroid in blob.final_ids_and_centroids:
-                        if blob_id in (None, 0):
-                            where = np.asarray(centroid)
-                            break
-            assert where is not None
-
         if where.ndim == 2:
             # Set the zoom to capture all positions of 'where'
             xmax, ymax = np.nanmax(where, axis=0)
             xmin, ymin = np.nanmin(where, axis=0)
             zoom_scale = max(
                 30 * self.median_speed, 1.8 * (xmax - xmin), 1.8 * (ymax - ymin)
             )
             self.video_player.center_canvas_at(
                 0.5 * (xmax + xmin), 0.5 * (ymin + ymax), zoom_scale=zoom_scale
             )
-            self.selection_last_location = (
-                None if np.any(np.isnan(where[0])) else tuple(where[0])
-            )
+            where = where[0]
         else:
             # Set the zoom to view ~50 time steps in the current canvas width
             self.video_player.center_canvas_at(
                 *where, zoom_scale=50 * self.median_speed
             )
-            self.selection_last_location = (
-                None if np.any(np.isnan(where)) else tuple(where)
-            )
+        self.selection_last_location = None if np.isnan(where).any() else tuple(where)
 
         self.selected_id = identity
         if kind in ("Jump", "Miss id"):
             self.interpolator.set_interpolation_params(identity, start, start + length)
         else:
             self.interpolator.setActivated(False)
         self.video_player.setCurrentFrame(
@@ -597,14 +582,15 @@
         )
 
         self.setup_points.load_points(video.setup_points)
         self.errorsExplorer.set_references(
             self.trajectories,
             self.unidentified,
             self.duplicated,
+            self.blobs,
             video.tracking_intervals,
         )
         self.interpolator.set_references(
             self.trajectories, self.unidentified, self.duplicated, self.blobs
         )
         self.video_player.update()
         self.unsaved_changes = False
@@ -650,20 +636,24 @@
             answer, new_id, propagate = self.dbl_click_dialog.exec_with_description(0)
             if answer == DblClickDialog.Answers.ChangeId:
                 self.selected_blob.add_centroid(event.xy_data, new_id)
                 self.update_trajectories_range(self.current_frame_number)
             return
 
         # clicked on a blob with centroid
-        assert self.selection_last_location is not None
         answer, new_id, propagate = self.dbl_click_dialog.exec_with_description(
             self.interpolator.animal_id + 1
             if self.interpolator.isEnabled()
             else self.selected_id
         )
+
+        if answer == DblClickDialog.Answers.Reset:
+            new_id = None
+            answer = DblClickDialog.Answers.ChangeId
+
         if answer == DblClickDialog.Answers.ChangeId:
             self.selected_blob.update_identity(
                 self.selected_id, new_id, self.selection_last_location
             )
             if propagate:
                 lower, upper = self.selected_blob.propagate_identity(
                     self.selected_id, new_id, self.selection_last_location
```

### Comparing `idtrackerai-5.1.5/src/idtrackerai_validator/validator_widgets/__init__.py` & `idtrackerai-5.1.6/src/idtrackerai_validator/validator_widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.5/src/idtrackerai_validator/validator_widgets/additional_info.py` & `idtrackerai-5.1.6/src/idtrackerai_validator/validator_widgets/additional_info.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.5/src/idtrackerai_validator/validator_widgets/errors_explorer.py` & `idtrackerai-5.1.6/src/idtrackerai_validator/validator_widgets/errors_explorer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import warnings
 
 import numpy as np
-from qtpy.QtCore import Qt, Signal
+from qtpy.QtCore import Qt, Signal  # type: ignore
 from qtpy.QtGui import QKeyEvent
 from qtpy.QtWidgets import (
     QAbstractItemView,
     QHBoxLayout,
     QHeaderView,
     QLabel,
     QTableWidget,
     QTableWidgetItem,
     QToolButton,
     QVBoxLayout,
     QWidget,
 )
 
+from idtrackerai import ListOfBlobs
 from idtrackerai_GUI_tools import LabeledSlider, key_event_modifier
 
 
 class CustomTableWidget(QTableWidget):
     def keyPressEvent(self, e: QKeyEvent):
         event = key_event_modifier(e)
         if event is not None:
@@ -39,15 +40,15 @@
     def __lt__(self, other: QTableWidgetItem) -> bool:
         return self.data(Qt.ItemDataRole.UserRole) < other.data(
             Qt.ItemDataRole.UserRole
         )
 
 
 class ErrorsExplorer(QWidget):
-    go_to_error = Signal(str, int, int, object, int)
+    go_to_error = Signal(str, int, int, np.ndarray, int)
     # kind, start, end, where, id
 
     def __init__(self):
         super().__init__()
         self.table = CustomTableWidget(1, 4)
         horizontalHeader = self.table.horizontalHeader()
         horizontalHeader.setSectionResizeMode(QHeaderView.ResizeMode.Stretch)
@@ -107,44 +108,64 @@
 
     def cell_clicked(self, row: int, col: int):
         if row < 0 or col < 0:
             return
 
         kind = self.table.item(row, 0).data(Qt.ItemDataRole.UserRole)
         identity = self.table.item(row, 1).data(Qt.ItemDataRole.UserRole)
-        start = self.table.item(row, 2).data(Qt.ItemDataRole.UserRole)
+        start: int = self.table.item(row, 2).data(Qt.ItemDataRole.UserRole)
         length = self.table.item(row, 3).data(Qt.ItemDataRole.UserRole)
         self.selected_error = kind, identity, start, length
 
-        where = None
+        where = self.trajectories[start]
         if kind in ("Jump", "Miss id"):
             if start > 0:
                 where = self.trajectories[start - 1 : start + length + 1, identity - 1]
             else:
                 where = self.trajectories[start : start + length + 1, identity - 1]
+        elif kind == "No id":
+            for blob in self.list_of_blobs.blobs_in_video[start]:
+                for blob_id, centroid in blob.final_ids_and_centroids:
+                    if blob_id in (None, 0):
+                        where = np.asarray(centroid)
+                        break
+        elif kind == "Dupl":
+            duplicated_centroids = []
+            for blob in self.list_of_blobs.blobs_in_video[start]:
+                for blob_id, centroid in blob.final_ids_and_centroids:
+                    if blob_id == identity:
+                        duplicated_centroids.append(centroid)
+            where = np.asarray(duplicated_centroids)
+        else:
+            raise ValueError(kind)
+
         self.go_to_error.emit(kind, start, length, where, identity)
 
     def set_references(
         self,
         traj: np.ndarray,
         unidentified: np.ndarray,
         duplicated: np.ndarray,
+        blobs: ListOfBlobs,
         tracking_intervals: list[list[int]],
     ):
         self.trajectories = traj
         self.unidentified = unidentified
         self.duplicated = duplicated
+        self.list_of_blobs = blobs
         self.non_accepted_jumps = np.ones((traj.shape[0] - 1, traj.shape[1]), bool)
         self.in_tracking_interval = np.zeros(traj.shape[0], bool)
         for start, end in tracking_intervals:
             self.in_tracking_interval[start:end] = True
 
         self.update_list_of_errors()
 
     def accepted_interpolation(self):
+        if not hasattr(self, "selected_error"):
+            return
         kind, identity, start, length = self.selected_error
         start -= 1
         if kind == "Jump":
             self.non_accepted_jumps[start : start + length, identity - 1] = False
 
     def getErrors(self) -> dict[str, list[tuple[int, np.ndarray, np.ndarray]]]:
         # TODO Add more errors (super-crossings)
```

### Comparing `idtrackerai-5.1.5/src/idtrackerai_validator/validator_widgets/id_groups.py` & `idtrackerai-5.1.6/src/idtrackerai_validator/validator_widgets/id_groups.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from qtpy.QtCore import Qt, Signal
+from qtpy.QtCore import Qt, Signal  # type: ignore
 from qtpy.QtGui import QColor
 from qtpy.QtWidgets import (
     QHBoxLayout,
     QInputDialog,
     QLabel,
     QToolButton,
     QVBoxLayout,
```

### Comparing `idtrackerai-5.1.5/src/idtrackerai_validator/validator_widgets/id_labels.py` & `idtrackerai-5.1.6/src/idtrackerai_validator/validator_widgets/id_labels.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from qtpy.QtCore import Qt, Signal
+from qtpy.QtCore import Qt, Signal  # type: ignore
 from qtpy.QtWidgets import QFormLayout, QLineEdit, QScrollArea, QWidget
 
 
 class IdLabels(QScrollArea):
     needToDraw = Signal()
     labels: list[str]
```

### Comparing `idtrackerai-5.1.5/src/idtrackerai_validator/validator_widgets/interpolator.py` & `idtrackerai-5.1.6/src/idtrackerai_validator/validator_widgets/interpolator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-from qtpy.QtCore import QEvent, QPointF, Qt, Signal
+from qtpy.QtCore import QEvent, QPointF, Qt, Signal  # type: ignore
 from qtpy.QtGui import QColorConstants, QKeyEvent
 from qtpy.QtWidgets import (
     QComboBox,
     QGroupBox,
     QHBoxLayout,
     QLabel,
     QMessageBox,
```

### Comparing `idtrackerai-5.1.5/src/idtrackerai_validator/validator_widgets/mark_properties.py` & `idtrackerai-5.1.6/src/idtrackerai_validator/validator_widgets/mark_properties.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from collections.abc import Iterable
 
-from qtpy.QtCore import Qt, Signal
+from qtpy.QtCore import Qt, Signal  # type: ignore
 from qtpy.QtWidgets import (
     QHBoxLayout,
     QRadioButton,
     QScrollArea,
     QSpinBox,
     QVBoxLayout,
     QWidget,
```

### Comparing `idtrackerai-5.1.5/src/idtrackerai_validator/validator_widgets/paint_blobs.py` & `idtrackerai-5.1.6/src/idtrackerai_validator/validator_widgets/paint_blobs.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,8 +187,8 @@
             alphas, centroids_trace[1:], centroids_trace[:-1]
         ):
             color.setAlpha(alpha)
             pen.setColor(color)
             trail_painter.setPen(pen)
             trail_painter.drawLine(QPointF(*pointA), QPointF(*pointB))
     trail_painter.end()
-    painter.drawImage(painter.window().toRectF(), canvas)
+    painter.drawImage(painter.window(), canvas)
```

### Comparing `idtrackerai-5.1.5/src/idtrackerai_validator/validator_widgets/setup_points.py` & `idtrackerai-5.1.6/src/idtrackerai_validator/validator_widgets/setup_points.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from re import compile
 
-from qtpy.QtCore import Qt, Signal
+from qtpy.QtCore import Qt, Signal  # type: ignore
 from qtpy.QtGui import QColor, QColorConstants
 from qtpy.QtWidgets import QInputDialog, QToolButton, QVBoxLayout, QWidget
 
 from idtrackerai_GUI_tools import CanvasMouseEvent, CanvasPainter, CustomList
 
 
 def has_invalid_chars(string):
@@ -42,26 +42,26 @@
         layout = QVBoxLayout()
         layout.setSpacing(2)
         self.setLayout(layout)
         layout.addWidget(self.add)
         layout.addWidget(self.list)
 
         self.add.toggled.connect(self.add_clicked)
-        self.setup_points_dict: dict[str, tuple[QColor, list[tuple[float, float]]]] = {}
+        self.setup_points_dict: dict[str, tuple[QColor, list[tuple[int, int]]]] = {}
         self.list.ListChanged.connect(self.needToDraw.emit)
         self.list.removedItem.connect(self.remove_item)
         self.color_count = -1
         self.setup_name = None
 
     def click_event(self, event: CanvasMouseEvent):
         if self.isVisible() and self.isEnabled() and self.setup_name is not None:
             points = self.setup_points_dict[self.setup_name][1]
             if event.button == Qt.MouseButton.LeftButton:
                 # Add clicked point
-                points.append(event.xy_data)
+                points.append(event.int_xy_data)
             elif event.button == Qt.MouseButton.RightButton:
                 # Remove nearest point
                 if not points:
                     return
                 distances = map(event.distance_to, points)
                 index, dist = min(enumerate(distances), key=lambda x: x[1])
                 if dist < 20 * event.zoom:  # 20 px threshold
@@ -100,42 +100,44 @@
             if self.setup_name is None:
                 return
             self.list.add_str(
                 self.setup_name
                 + ": "
                 + ",".join(
                     [
-                        f"[{x:.1f}, {y:.1f}]"
+                        f"[{x:d}, {y:d}]"
                         for x, y in self.setup_points_dict[self.setup_name][1]
                     ]
                 ),
                 color=self.setup_points_dict[self.setup_name][0],
             )
             self.setup_name = None
 
     def remove_item(self, data: str):
         self.setup_points_dict.pop(data.split(":")[0])
 
-    def load_points(self, values: dict[str, list[tuple[float, float]]]):
+    def load_points(self, values: dict[str, list[tuple[int, int]]]):
         self.list.clear()
         self.setup_points_dict.clear()
         if not isinstance(values, dict):
             return  # Loading from v4
 
         for name, points in values.items():
             self.color_count = (
                 0 if self.color_count == n_colors - 1 else self.color_count + 1
             )
             self.setup_points_dict[name] = (QColors[self.color_count], points)
             self.list.add_str(
-                name + ": " + ",".join([f"[{x:.1f}, {y:.1f}]" for x, y in points]),
+                name
+                + ": "
+                + ",".join([f"[{int(x):d}, {int(y):d}]" for x, y in points]),
                 color=QColors[self.color_count],
             )
 
-    def get_points(self) -> dict[str, list[tuple[float, float]]]:
+    def get_points(self) -> dict[str, list[tuple[int, int]]]:
         return {key: value[1] for key, value in self.setup_points_dict.items()}
 
     def paint_on_canvas(self, painter: CanvasPainter):
         painter.setPenColor(QColorConstants.Black)
         for color, points in self.setup_points_dict.values():
             painter.setBrush(color)
             for point in points:
```

### Comparing `idtrackerai-5.1.5/src/idtrackerai_video/general_video.py` & `idtrackerai-5.1.6/src/idtrackerai_video/general_video.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.5/src/idtrackerai_video/individual_videos.py` & `idtrackerai-5.1.6/src/idtrackerai_video/individual_videos.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.5/src/idtrackerai_video/main.py` & `idtrackerai-5.1.6/src/idtrackerai_video/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,15 +35,14 @@
     parser.add_argument(
         "--t",
         type=Path,
         help=(
             "Path to the trajectory file, default is "
             "session_dir/trajectories/trajectories_wo_gaps.npy"
         ),
-        default=None,
         metavar="",
     )
     parser.add_argument(
         "--tl",
         type=int,
         default=20,
         help=(
@@ -52,15 +51,15 @@
         ),
         metavar="",
     )
     parser.add_argument(
         "--s", type=int, default=0, help="Frame where to start the video", metavar=""
     )
     parser.add_argument(
-        "--e", type=int, default=None, help="Frame where to end the video", metavar=""
+        "--e", type=int, help="Frame where to end the video", metavar=""
     )
     args = parser.parse_args()
 
     video = Video.load(args.session_path)
 
     if args.t is None:
         possible_files = (
```

