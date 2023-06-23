# Comparing `tmp/pyxy3d-0.1.3.tar.gz` & `tmp/pyxy3d-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxy3d-0.1.3.tar", max compression
+gzip compressed data, was "pyxy3d-0.1.4.tar", max compression
```

## Comparing `pyxy3d-0.1.3.tar` & `pyxy3d-0.1.4.tar`

### file list

```diff
@@ -1,233 +1,232 @@
--rw-r--r--   0        0        0    35190 2023-06-14 20:19:57.480906 pyxy3d-0.1.3/LICENSE.md
--rw-r--r--   0        0        0      922 2023-06-22 13:04:36.844499 pyxy3d-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2644 2023-06-21 22:25:18.660194 pyxy3d-0.1.3/pyxy3d/__init__.py
--rw-r--r--   0        0        0      934 2023-06-12 22:15:42.388447 pyxy3d-0.1.3/pyxy3d/__main__.py
--rw-r--r--   0        0        0     7201 2023-04-16 14:08:55.358491 pyxy3d-0.1.3/pyxy3d/calibration/__pycache__/charuco.cpython-310.pyc
--rw-r--r--   0        0        0     7111 2023-04-13 18:16:32.164621 pyxy3d-0.1.3/pyxy3d/calibration/__pycache__/charuco.cpython-38.pyc
--rw-r--r--   0        0        0     3147 2023-04-13 14:11:35.706111 pyxy3d-0.1.3/pyxy3d/calibration/__pycache__/corner_tracker.cpython-38.pyc
--rw-r--r--   0        0        0     1525 2023-04-13 21:33:14.966692 pyxy3d-0.1.3/pyxy3d/calibration/__pycache__/draw_charuco.cpython-310.pyc
--rw-r--r--   0        0        0     1517 2023-03-16 18:37:10.539737 pyxy3d-0.1.3/pyxy3d/calibration/__pycache__/draw_charuco.cpython-38.pyc
--rw-r--r--   0        0        0     7208 2023-06-12 18:45:04.367154 pyxy3d-0.1.3/pyxy3d/calibration/__pycache__/monocalibrator.cpython-310.pyc
--rw-r--r--   0        0        0     7083 2023-04-13 18:16:59.718066 pyxy3d-0.1.3/pyxy3d/calibration/__pycache__/monocalibrator.cpython-38.pyc
--rw-r--r--   0        0        0    11365 2023-03-16 18:37:11.887671 pyxy3d-0.1.3/pyxy3d/calibration/__pycache__/omnicalibrator.cpython-38.pyc
--rw-r--r--   0        0        0     7979 2023-06-08 18:19:03.652989 pyxy3d-0.1.3/pyxy3d/calibration/__pycache__/stereocalibrator.cpython-310.pyc
--rw-r--r--   0        0        0     7845 2023-04-13 14:31:07.431535 pyxy3d-0.1.3/pyxy3d/calibration/__pycache__/stereocalibrator.cpython-38.pyc
--rw-r--r--   0        0        0     7001 2023-06-12 12:22:25.787593 pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/__pycache__/capture_volume.cpython-310.pyc
--rw-r--r--   0        0        0     8147 2023-04-11 10:38:21.551689 pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/__pycache__/capture_volume.cpython-38.pyc
--rw-r--r--   0        0        0     3205 2023-05-02 22:08:30.018323 pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/__pycache__/point_estimates.cpython-310.pyc
--rw-r--r--   0        0        0     3651 2023-04-09 20:26:50.741740 pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/__pycache__/point_estimates.cpython-38.pyc
--rw-r--r--   0        0        0     9626 2023-05-22 14:59:39.828020 pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/__pycache__/quality_controller.cpython-310.pyc
--rw-r--r--   0        0        0     9567 2023-04-13 18:47:12.691013 pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/__pycache__/quality_controller.cpython-38.pyc
--rw-r--r--   0        0        0     7294 2023-05-22 14:59:39.817019 pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/__pycache__/set_origin_functions.cpython-310.pyc
--rw-r--r--   0        0        0     7172 2023-04-06 11:06:35.216555 pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/__pycache__/set_origin_functions.cpython-38.pyc
--rw-r--r--   0        0        0    10148 2023-06-12 12:14:10.017140 pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/capture_volume.py
--rw-r--r--   0        0        0  1505952 2023-03-13 23:46:36.934749 pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/capture_volume_stage_1.pkl
--rw-r--r--   0        0        0     2813 2023-04-13 21:41:08.181971 pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_point_estimates.cpython-310.pyc
--rw-r--r--   0        0        0     2825 2023-03-16 18:37:13.420982 pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_point_estimates.cpython-38.pyc
--rw-r--r--   0        0        0     2938 2023-04-16 14:08:57.590539 pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_stereotriangulated_table.cpython-310.pyc
--rw-r--r--   0        0        0     2963 2023-04-13 14:11:34.686199 pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_stereotriangulated_table.cpython-38.pyc
--rw-r--r--   0        0        0     3898 2023-03-16 18:13:11.445058 pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/helper_functions/get_point_estimates.py
--rw-r--r--   0        0        0     4680 2023-04-16 12:58:12.386690 pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/helper_functions/get_stereotriangulated_table.py
--rw-r--r--   0        0        0     3631 2023-05-02 22:08:10.575286 pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/point_estimates.py
--rw-r--r--   0        0        0    15888 2023-05-22 13:44:00.083689 pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/quality_controller.py
--rw-r--r--   0        0        0     1766 2023-03-16 18:13:11.448058 pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/seaborn_summaries.py
--rw-r--r--   0        0        0    10868 2023-05-22 13:44:00.084688 pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/set_origin_functions.py
--rw-r--r--   0        0        0     9510 2023-04-16 12:58:12.392689 pyxy3d-0.1.3/pyxy3d/calibration/charuco.py
--rw-r--r--   0        0        0     1685 2023-03-16 18:13:11.451057 pyxy3d-0.1.3/pyxy3d/calibration/draw_charuco.py
--rw-r--r--   0        0        0     9886 2023-06-12 16:49:05.518131 pyxy3d-0.1.3/pyxy3d/calibration/monocalibrator.py
--rw-r--r--   0        0        0    12385 2023-06-08 18:18:45.456813 pyxy3d-0.1.3/pyxy3d/calibration/stereocalibrator.py
--rw-r--r--   0        0        0     7119 2023-05-22 16:42:44.186443 pyxy3d-0.1.3/pyxy3d/cameras/__pycache__/camera.cpython-310.pyc
--rw-r--r--   0        0        0     7171 2023-04-12 14:56:03.753093 pyxy3d-0.1.3/pyxy3d/cameras/__pycache__/camera.cpython-38.pyc
--rw-r--r--   0        0        0     6788 2023-06-10 20:39:00.834305 pyxy3d-0.1.3/pyxy3d/cameras/__pycache__/camera_array.cpython-310.pyc
--rw-r--r--   0        0        0     6811 2023-04-09 20:26:50.029740 pyxy3d-0.1.3/pyxy3d/cameras/__pycache__/camera_array.cpython-38.pyc
--rw-r--r--   0        0        0     9199 2023-05-02 22:08:30.006322 pyxy3d-0.1.3/pyxy3d/cameras/__pycache__/camera_array_initializer.cpython-310.pyc
--rw-r--r--   0        0        0     9153 2023-04-06 11:06:35.358553 pyxy3d-0.1.3/pyxy3d/cameras/__pycache__/camera_array_initializer.cpython-38.pyc
--rw-r--r--   0        0        0     3161 2023-04-13 21:33:14.970692 pyxy3d-0.1.3/pyxy3d/cameras/__pycache__/data_packets.cpython-310.pyc
--rw-r--r--   0        0        0     3147 2023-04-13 17:33:55.370369 pyxy3d-0.1.3/pyxy3d/cameras/__pycache__/data_packets.cpython-38.pyc
--rw-r--r--   0        0        0     8085 2023-06-10 20:05:09.584549 pyxy3d-0.1.3/pyxy3d/cameras/__pycache__/live_stream.cpython-310.pyc
--rw-r--r--   0        0        0     8585 2023-04-13 17:33:56.274500 pyxy3d-0.1.3/pyxy3d/cameras/__pycache__/live_stream.cpython-38.pyc
--rw-r--r--   0        0        0     9900 2023-06-22 12:39:44.642763 pyxy3d-0.1.3/pyxy3d/cameras/__pycache__/synchronizer.cpython-310.pyc
--rw-r--r--   0        0        0    11042 2023-04-13 18:30:26.417813 pyxy3d-0.1.3/pyxy3d/cameras/__pycache__/synchronizer.cpython-38.pyc
--rw-r--r--   0        0        0    10631 2023-05-22 16:41:37.293000 pyxy3d-0.1.3/pyxy3d/cameras/camera.py
--rw-r--r--   0        0        0     7710 2023-06-10 20:38:54.275345 pyxy3d-0.1.3/pyxy3d/cameras/camera_array.py
--rw-r--r--   0        0        0    12868 2023-05-02 22:08:10.579286 pyxy3d-0.1.3/pyxy3d/cameras/camera_array_initializer.py
--rw-r--r--   0        0        0    11935 2023-06-10 20:04:58.799532 pyxy3d-0.1.3/pyxy3d/cameras/live_stream.py
--rw-r--r--   0        0        0    13543 2023-06-15 18:45:15.726954 pyxy3d-0.1.3/pyxy3d/cameras/synchronizer.py
--rw-r--r--   0        0        0    13040 2023-06-12 12:14:10.019141 pyxy3d-0.1.3/pyxy3d/configurator.py
--rw-r--r--   0        0        0     7036 2023-05-18 21:56:09.817280 pyxy3d-0.1.3/pyxy3d/export.py
--rw-r--r--   0        0        0     3538 2023-06-12 18:45:08.762112 pyxy3d-0.1.3/pyxy3d/gui/__pycache__/calibrate_capture_volume_widget.cpython-310.pyc
--rw-r--r--   0        0        0     5691 2023-06-22 12:39:42.763393 pyxy3d-0.1.3/pyxy3d/gui/__pycache__/calibration_widget.cpython-310.pyc
--rw-r--r--   0        0        0     8693 2023-05-06 16:11:05.603259 pyxy3d-0.1.3/pyxy3d/gui/__pycache__/calibration_wizard.cpython-310.pyc
--rw-r--r--   0        0        0     7124 2023-06-08 18:19:04.615289 pyxy3d-0.1.3/pyxy3d/gui/__pycache__/charuco_widget.cpython-310.pyc
--rw-r--r--   0        0        0     8558 2023-06-22 12:39:48.156709 pyxy3d-0.1.3/pyxy3d/gui/__pycache__/extrinsic_calibration_widget.cpython-310.pyc
--rw-r--r--   0        0        0     2110 2023-05-29 12:41:08.382954 pyxy3d-0.1.3/pyxy3d/gui/__pycache__/log_widget.cpython-310.pyc
--rw-r--r--   0        0        0     8811 2023-05-02 22:10:09.955994 pyxy3d-0.1.3/pyxy3d/gui/__pycache__/main.cpython-310.pyc
--rw-r--r--   0        0        0     8445 2023-04-12 14:19:14.529651 pyxy3d-0.1.3/pyxy3d/gui/__pycache__/main.cpython-38.pyc
--rw-r--r--   0        0        0    11710 2023-06-22 12:39:49.307577 pyxy3d-0.1.3/pyxy3d/gui/__pycache__/main_widget.cpython-310.pyc
--rw-r--r--   0        0        0     2664 2023-06-08 18:19:04.619290 pyxy3d-0.1.3/pyxy3d/gui/__pycache__/navigation_bars.cpython-310.pyc
--rw-r--r--   0        0        0     2468 2023-06-02 00:29:24.448977 pyxy3d-0.1.3/pyxy3d/gui/__pycache__/playback_widget.cpython-310.pyc
--rw-r--r--   0        0        0     9611 2023-06-10 20:31:20.063896 pyxy3d-0.1.3/pyxy3d/gui/__pycache__/post_processing_widget.cpython-310.pyc
--rw-r--r--   0        0        0     1176 2023-05-29 13:25:02.424999 pyxy3d-0.1.3/pyxy3d/gui/__pycache__/progress_dialog.cpython-310.pyc
--rw-r--r--   0        0        0     2649 2023-05-22 15:00:23.510630 pyxy3d-0.1.3/pyxy3d/gui/__pycache__/qt_logger.cpython-310.pyc
--rw-r--r--   0        0        0     2623 2023-04-06 18:40:19.597418 pyxy3d-0.1.3/pyxy3d/gui/__pycache__/qt_logger.cpython-38.pyc
--rw-r--r--   0        0        0    11942 2023-06-22 12:39:49.300575 pyxy3d-0.1.3/pyxy3d/gui/__pycache__/recording_widget.cpython-310.pyc
--rw-r--r--   0        0        0     8798 2023-04-12 14:17:47.475386 pyxy3d-0.1.3/pyxy3d/gui/__pycache__/recording_widget.cpython-38.pyc
--rw-r--r--   0        0        0     2641 2023-04-13 21:41:10.861210 pyxy3d-0.1.3/pyxy3d/gui/__pycache__/widgets.cpython-310.pyc
--rw-r--r--   0        0        0     2969 2023-04-06 18:40:19.600418 pyxy3d-0.1.3/pyxy3d/gui/__pycache__/widgets.cpython-38.pyc
--rw-r--r--   0        0        0     6864 2023-05-29 12:41:07.242642 pyxy3d-0.1.3/pyxy3d/gui/__pycache__/wizard_charuco.cpython-310.pyc
--rw-r--r--   0        0        0     6979 2023-04-06 18:40:19.594417 pyxy3d-0.1.3/pyxy3d/gui/__pycache__/wizard_charuco.cpython-38.pyc
--rw-r--r--   0        0        0     4851 2023-05-02 13:40:54.299559 pyxy3d-0.1.3/pyxy3d/gui/__pycache__/wizard_directory.cpython-310.pyc
--rw-r--r--   0        0        0     4903 2023-04-06 18:40:19.608417 pyxy3d-0.1.3/pyxy3d/gui/__pycache__/wizard_directory.cpython-38.pyc
--rw-r--r--   0        0        0     4052 2023-06-12 16:49:05.519131 pyxy3d-0.1.3/pyxy3d/gui/calibrate_capture_volume_widget.py
--rw-r--r--   0        0        0     7459 2023-06-15 18:45:15.727954 pyxy3d-0.1.3/pyxy3d/gui/calibration_widget.py
--rw-r--r--   0        0        0    13085 2023-06-02 16:06:24.614359 pyxy3d-0.1.3/pyxy3d/gui/camera_config/__pycache__/camera_config_dialogue.cpython-310.pyc
--rw-r--r--   0        0        0    13777 2023-03-29 13:33:28.389797 pyxy3d-0.1.3/pyxy3d/gui/camera_config/__pycache__/camera_config_dialogue.cpython-38.pyc
--rw-r--r--   0        0        0     3658 2023-06-10 20:05:11.213579 pyxy3d-0.1.3/pyxy3d/gui/camera_config/__pycache__/camera_summary_widget.cpython-310.pyc
--rw-r--r--   0        0        0     4748 2023-06-01 14:22:06.839277 pyxy3d-0.1.3/pyxy3d/gui/camera_config/__pycache__/camera_tabs.cpython-310.pyc
--rw-r--r--   0        0        0     3850 2023-03-20 23:10:53.097964 pyxy3d-0.1.3/pyxy3d/gui/camera_config/__pycache__/camera_tabs.cpython-38.pyc
--rw-r--r--   0        0        0     3155 2023-06-02 14:30:41.590277 pyxy3d-0.1.3/pyxy3d/gui/camera_config/__pycache__/frame_emitter.cpython-310.pyc
--rw-r--r--   0        0        0     2704 2023-03-16 18:37:13.513000 pyxy3d-0.1.3/pyxy3d/gui/camera_config/__pycache__/frame_emitter.cpython-38.pyc
--rw-r--r--   0        0        0     3619 2023-06-10 20:39:01.831691 pyxy3d-0.1.3/pyxy3d/gui/camera_config/__pycache__/intrinsic_calibration_widget.cpython-310.pyc
--rw-r--r--   0        0        0    17771 2023-06-02 15:39:41.317656 pyxy3d-0.1.3/pyxy3d/gui/camera_config/camera_config_dialogue.py
--rw-r--r--   0        0        0     5794 2023-06-10 20:04:49.727607 pyxy3d-0.1.3/pyxy3d/gui/camera_config/camera_summary_widget.py
--rw-r--r--   0        0        0     3893 2023-06-02 00:28:42.145417 pyxy3d-0.1.3/pyxy3d/gui/camera_config/frame_emitter.py
--rw-r--r--   0        0        0     3760 2023-06-10 20:38:54.278346 pyxy3d-0.1.3/pyxy3d/gui/camera_config/intrinsic_calibration_widget.py
--rw-r--r--   0        0        0    11157 2023-06-08 18:18:45.460813 pyxy3d-0.1.3/pyxy3d/gui/charuco_widget.py
--rw-r--r--   0        0        0    10800 2023-06-15 18:45:15.728953 pyxy3d-0.1.3/pyxy3d/gui/extrinsic_calibration_widget.py
--rw-r--r--   0        0        0     7468 2023-06-01 18:24:14.049008 pyxy3d-0.1.3/pyxy3d/gui/frame_builders/__pycache__/extrinsic_calibration_widget.cpython-310.pyc
--rw-r--r--   0        0        0     9143 2023-03-16 18:37:13.553998 pyxy3d-0.1.3/pyxy3d/gui/frame_builders/__pycache__/omni_frame_builder.cpython-38.pyc
--rw-r--r--   0        0        0     5691 2023-03-16 18:37:13.539983 pyxy3d-0.1.3/pyxy3d/gui/frame_builders/__pycache__/omni_frame_widget.cpython-38.pyc
--rw-r--r--   0        0        0     9669 2023-06-22 12:39:48.162709 pyxy3d-0.1.3/pyxy3d/gui/frame_builders/__pycache__/paired_frame_builder.cpython-310.pyc
--rw-r--r--   0        0        0     9881 2023-06-01 18:24:14.063003 pyxy3d-0.1.3/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_builder.cpython-310.pyc
--rw-r--r--   0        0        0    11456 2023-04-13 17:55:04.283828 pyxy3d-0.1.3/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_builder.cpython-38.pyc
--rw-r--r--   0        0        0     7359 2023-06-01 14:22:06.856278 pyxy3d-0.1.3/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_widget.cpython-310.pyc
--rw-r--r--   0        0        0     7148 2023-04-13 18:41:31.149308 pyxy3d-0.1.3/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_widget.cpython-38.pyc
--rw-r--r--   0        0        0    13851 2023-06-15 18:45:15.729953 pyxy3d-0.1.3/pyxy3d/gui/frame_builders/paired_frame_builder.py
--rw-r--r--   0        0        0    19878 2023-04-07 19:40:35.259432 pyxy3d-0.1.3/pyxy3d/gui/icons/pyxy_logo.svg
--rw-r--r--   0        0        0      941 2023-03-16 18:13:11.463060 pyxy3d-0.1.3/pyxy3d/gui/icons/rotate-camera-left.svg
--rw-r--r--   0        0        0      944 2023-03-16 18:13:11.464059 pyxy3d-0.1.3/pyxy3d/gui/icons/rotate-camera-right.svg
--rw-r--r--   0        0        0     2460 2023-05-28 21:21:33.674553 pyxy3d-0.1.3/pyxy3d/gui/log_widget.py
--rw-r--r--   0        0        0    16047 2023-06-15 18:45:15.731956 pyxy3d-0.1.3/pyxy3d/gui/main_widget.py
--rw-r--r--   0        0        0     3292 2023-06-08 18:18:45.464814 pyxy3d-0.1.3/pyxy3d/gui/navigation_bars.py
--rw-r--r--   0        0        0     1988 2023-06-02 00:28:42.150417 pyxy3d-0.1.3/pyxy3d/gui/playback_widget.py
--rw-r--r--   0        0        0    11310 2023-06-10 20:29:24.686837 pyxy3d-0.1.3/pyxy3d/gui/post_processing_widget.py
--rw-r--r--   0        0        0      950 2023-05-28 21:21:33.677553 pyxy3d-0.1.3/pyxy3d/gui/progress_dialog.py
--rw-r--r--   0        0        0    14740 2023-06-15 18:45:15.732954 pyxy3d-0.1.3/pyxy3d/gui/recording_widget.py
--rw-r--r--   0        0        0     6275 2023-05-13 12:35:31.914917 pyxy3d-0.1.3/pyxy3d/gui/vizualize/__pycache__/camera_mesh.cpython-310.pyc
--rw-r--r--   0        0        0     6278 2023-04-10 15:11:26.319020 pyxy3d-0.1.3/pyxy3d/gui/vizualize/__pycache__/camera_mesh.cpython-38.pyc
--rw-r--r--   0        0        0     3198 2023-03-27 01:11:02.734179 pyxy3d-0.1.3/pyxy3d/gui/vizualize/__pycache__/capture_volume_dialog.cpython-38.pyc
--rw-r--r--   0        0        0     5013 2023-04-08 17:08:48.219160 pyxy3d-0.1.3/pyxy3d/gui/vizualize/__pycache__/capture_volume_visualizer.cpython-38.pyc
--rw-r--r--   0        0        0     5850 2023-04-08 17:08:47.292159 pyxy3d-0.1.3/pyxy3d/gui/vizualize/__pycache__/capture_volume_widget.cpython-38.pyc
--rw-r--r--   0        0        0     4920 2023-06-12 12:22:29.640003 pyxy3d-0.1.3/pyxy3d/gui/vizualize/__pycache__/playback_triangulation_widget.cpython-310.pyc
--rw-r--r--   0        0        0     4522 2023-04-16 14:08:58.474682 pyxy3d-0.1.3/pyxy3d/gui/vizualize/__pycache__/realtime_triangulation_widget.cpython-310.pyc
--rw-r--r--   0        0        0     2999 2023-06-08 18:19:05.638538 pyxy3d-0.1.3/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_visualizer.cpython-310.pyc
--rw-r--r--   0        0        0     3506 2023-04-10 15:11:26.253010 pyxy3d-0.1.3/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_visualizer.cpython-38.pyc
--rw-r--r--   0        0        0     5838 2023-06-12 12:22:27.405313 pyxy3d-0.1.3/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_widget.cpython-310.pyc
--rw-r--r--   0        0        0     5615 2023-04-13 18:47:41.885491 pyxy3d-0.1.3/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_widget.cpython-38.pyc
--rw-r--r--   0        0        0     3404 2023-06-08 18:18:45.466812 pyxy3d-0.1.3/pyxy3d/gui/vizualize/calibration/capture_volume_visualizer.py
--rw-r--r--   0        0        0     6843 2023-06-12 12:14:10.025140 pyxy3d-0.1.3/pyxy3d/gui/vizualize/calibration/capture_volume_widget.py
--rw-r--r--   0        0        0     9146 2023-05-12 22:51:00.876793 pyxy3d-0.1.3/pyxy3d/gui/vizualize/camera_mesh.py
--rw-r--r--   0        0        0     5054 2023-06-12 12:14:10.027140 pyxy3d-0.1.3/pyxy3d/gui/vizualize/playback_triangulation_widget.py
--rw-r--r--   0        0        0     5450 2023-05-22 13:44:00.101687 pyxy3d-0.1.3/pyxy3d/gui/vizualize/realtime_triangulation_widget.py
--rw-r--r--   0        0        0     1135 2023-05-18 17:09:55.119648 pyxy3d-0.1.3/pyxy3d/helper.py
--rw-r--r--   0        0        0     6646 2023-06-15 00:37:58.434754 pyxy3d-0.1.3/pyxy3d/interface.py
--rw-r--r--   0        0        0     3111 2023-06-01 14:21:56.756810 pyxy3d-0.1.3/pyxy3d/logger.py
--rw-r--r--   0        0        0     7100 2023-06-12 12:14:10.028141 pyxy3d-0.1.3/pyxy3d/post_processor.py
--rw-r--r--   0        0        0     8482 2023-05-29 13:25:01.175649 pyxy3d-0.1.3/pyxy3d/recording/__pycache__/recorded_stream.cpython-310.pyc
--rw-r--r--   0        0        0     7603 2023-04-13 17:33:56.707496 pyxy3d-0.1.3/pyxy3d/recording/__pycache__/recorded_stream.cpython-38.pyc
--rw-r--r--   0        0        0     5928 2023-06-12 12:22:27.383610 pyxy3d-0.1.3/pyxy3d/recording/__pycache__/video_recorder.cpython-310.pyc
--rw-r--r--   0        0        0     5376 2023-04-13 14:11:36.908257 pyxy3d-0.1.3/pyxy3d/recording/__pycache__/video_recorder.cpython-38.pyc
--rw-r--r--   0        0        0    11830 2023-05-28 21:21:33.684552 pyxy3d-0.1.3/pyxy3d/recording/recorded_stream.py
--rw-r--r--   0        0        0     8730 2023-06-12 12:14:10.029141 pyxy3d-0.1.3/pyxy3d/recording/video_recorder.py
--rw-r--r--   0        0        0     2818 2023-06-05 20:04:19.162433 pyxy3d-0.1.3/pyxy3d/session/__pycache__/get_stage.cpython-310.pyc
--rw-r--r--   0        0        0    16304 2023-06-22 12:39:42.776391 pyxy3d-0.1.3/pyxy3d/session/__pycache__/session.cpython-310.pyc
--rw-r--r--   0        0        0    21437 2023-06-15 18:45:15.733955 pyxy3d-0.1.3/pyxy3d/session/session.py
--rw-r--r--   0        0        0        0 2023-04-16 12:58:12.408688 pyxy3d-0.1.3/pyxy3d/trackers/__init__.py
--rw-r--r--   0        0        0      153 2023-04-16 14:08:55.370508 pyxy3d-0.1.3/pyxy3d/trackers/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3955 2023-05-13 12:35:24.878771 pyxy3d-0.1.3/pyxy3d/trackers/__pycache__/charuco_tracker.cpython-310.pyc
--rw-r--r--   0        0        0     3531 2023-05-13 12:35:26.254677 pyxy3d-0.1.3/pyxy3d/trackers/__pycache__/hand_tracker.cpython-310.pyc
--rw-r--r--   0        0        0     1123 2023-05-13 12:35:28.030304 pyxy3d-0.1.3/pyxy3d/trackers/__pycache__/helper.cpython-310.pyc
--rw-r--r--   0        0        0     6774 2023-05-18 18:02:52.161100 pyxy3d-0.1.3/pyxy3d/trackers/__pycache__/holistic_opensim_tracker.cpython-310.pyc
--rw-r--r--   0        0        0     6262 2023-05-13 12:35:28.041314 pyxy3d-0.1.3/pyxy3d/trackers/__pycache__/holistic_tracker.cpython-310.pyc
--rw-r--r--   0        0        0     3797 2023-05-13 12:35:28.036311 pyxy3d-0.1.3/pyxy3d/trackers/__pycache__/pose_tracker.cpython-310.pyc
--rw-r--r--   0        0        0     3515 2023-05-12 22:32:19.505484 pyxy3d-0.1.3/pyxy3d/trackers/__pycache__/threaded_hand_tracker.cpython-310.pyc
--rw-r--r--   0        0        0     1017 2023-05-18 18:02:48.968666 pyxy3d-0.1.3/pyxy3d/trackers/__pycache__/tracker_enum.cpython-310.pyc
--rw-r--r--   0        0        0     5004 2023-05-12 22:51:00.882792 pyxy3d-0.1.3/pyxy3d/trackers/charuco_tracker.py
--rw-r--r--   0        0        0     4651 2023-05-12 22:51:00.883791 pyxy3d-0.1.3/pyxy3d/trackers/hand_tracker.py
--rw-r--r--   0        0        0     1330 2023-05-12 22:51:00.884792 pyxy3d-0.1.3/pyxy3d/trackers/helper.py
--rw-r--r--   0        0        0    10677 2023-05-18 17:09:55.120646 pyxy3d-0.1.3/pyxy3d/trackers/holistic_opensim_tracker.py
--rw-r--r--   0        0        0     9419 2023-05-12 22:51:00.885792 pyxy3d-0.1.3/pyxy3d/trackers/holistic_tracker.py
--rw-r--r--   0        0        0     4239 2023-05-12 22:51:00.885792 pyxy3d-0.1.3/pyxy3d/trackers/pose_tracker.py
--rw-r--r--   0        0        0      669 2023-05-18 17:09:55.121648 pyxy3d-0.1.3/pyxy3d/trackers/tracker_enum.py
--rw-r--r--   0        0        0     5629 2023-04-16 14:08:57.598538 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/array_stereo_triangulator.cpython-310.pyc
--rw-r--r--   0        0        0     5656 2023-04-13 17:33:55.945379 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/array_stereo_triangulator.cpython-38.pyc
--rw-r--r--   0        0        0      564 2023-04-24 13:44:16.864821 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/helper.cpython-310.pyc
--rw-r--r--   0        0        0     5809 2023-05-03 19:22:07.093614 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.cpython-310.pyc
--rw-r--r--   0        0        0     4640 2023-04-11 11:20:24.830020 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.cpython-38.pyc
--rw-r--r--   0        0        0   277847 2023-04-17 18:50:37.938076 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.1.nbc
--rw-r--r--   0        0        0   278178 2023-04-17 18:47:53.733008 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.2.nbc
--rw-r--r--   0        0        0     1853 2023-04-17 18:50:37.934076 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.nbi
--rw-r--r--   0        0        0   278065 2023-04-15 22:26:29.919720 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py310.1.nbc
--rw-r--r--   0        0        0     1795 2023-04-15 22:26:29.916718 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py310.nbi
--rw-r--r--   0        0        0   277525 2023-04-13 14:11:54.518242 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py38.1.nbc
--rw-r--r--   0        0        0     1794 2023-04-13 14:11:54.515242 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py38.nbi
--rw-r--r--   0        0        0   277847 2023-04-15 16:24:55.484079 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-138.py310.1.nbc
--rw-r--r--   0        0        0     1853 2023-04-15 16:24:55.480077 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-138.py310.nbi
--rw-r--r--   0        0        0   277847 2023-04-15 21:02:04.894614 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-139.py310.1.nbc
--rw-r--r--   0        0        0     1853 2023-04-15 21:02:04.889631 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-139.py310.nbi
--rw-r--r--   0        0        0   277790 2023-04-09 20:05:59.716347 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-86.py38.1.nbc
--rw-r--r--   0        0        0     1793 2023-04-09 20:05:59.712345 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-86.py38.nbi
--rw-r--r--   0        0        0   277795 2023-04-09 20:08:37.404028 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-88.py38.1.nbc
--rw-r--r--   0        0        0     1793 2023-04-09 20:08:37.400042 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-88.py38.nbi
--rw-r--r--   0        0        0    80840 2023-04-17 18:50:25.192073 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.unique_with_counts-118.py310.1.nbc
--rw-r--r--   0        0        0     1278 2023-04-17 18:50:25.189073 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.unique_with_counts-118.py310.nbi
--rw-r--r--   0        0        0     4903 2023-04-16 14:08:57.603539 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/stereo_points_builder.cpython-310.pyc
--rw-r--r--   0        0        0     4910 2023-04-13 17:33:55.950369 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/stereo_points_builder.cpython-38.pyc
--rw-r--r--   0        0        0     5522 2023-06-08 19:16:30.042145 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.cpython-310.pyc
--rw-r--r--   0        0        0   277993 2023-06-10 20:35:53.847895 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.1.nbc
--rw-r--r--   0        0        0   278337 2023-06-10 20:36:00.364127 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.2.nbc
--rw-r--r--   0        0        0   275198 2023-06-10 20:36:15.587107 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.3.nbc
--rw-r--r--   0        0        0     3826 2023-06-10 20:36:15.585108 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.nbi
--rw-r--r--   0        0        0   274936 2023-05-07 17:31:11.859065 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-170.py310.1.nbc
--rw-r--r--   0        0        0     1819 2023-05-07 17:31:11.856057 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-170.py310.nbi
--rw-r--r--   0        0        0   280483 2023-05-11 20:37:44.633248 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-186.py310.1.nbc
--rw-r--r--   0        0        0     1855 2023-05-11 20:37:44.630243 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-186.py310.nbi
--rw-r--r--   0        0        0   277957 2023-05-11 19:51:33.032983 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.1.nbc
--rw-r--r--   0        0        0   278013 2023-05-11 17:55:35.449169 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.2.nbc
--rw-r--r--   0        0        0   278357 2023-05-11 17:56:15.957610 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.3.nbc
--rw-r--r--   0        0        0     1855 2023-05-11 19:51:33.028983 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.nbi
--rw-r--r--   0        0        0   277977 2023-05-11 20:58:46.910959 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.1.nbc
--rw-r--r--   0        0        0   274956 2023-05-11 22:29:46.557422 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.2.nbc
--rw-r--r--   0        0        0   280725 2023-05-12 22:34:01.184507 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.3.nbc
--rw-r--r--   0        0        0     3913 2023-05-12 22:34:01.181521 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.nbi
--rw-r--r--   0        0        0   274956 2023-05-13 12:36:45.045739 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.1.nbc
--rw-r--r--   0        0        0   277993 2023-05-14 17:03:11.852980 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.2.nbc
--rw-r--r--   0        0        0   278337 2023-05-14 17:03:18.755882 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.3.nbc
--rw-r--r--   0        0        0     3855 2023-05-14 17:03:18.752878 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.nbi
--rw-r--r--   0        0        0   278215 2023-05-12 22:36:41.576195 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-195.py310.1.nbc
--rw-r--r--   0        0        0     1797 2023-05-12 22:36:41.573185 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-195.py310.nbi
--rw-r--r--   0        0        0    80914 2023-06-10 20:35:46.176596 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.1.nbc
--rw-r--r--   0        0        0    77589 2023-06-10 20:36:11.729164 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.2.nbc
--rw-r--r--   0        0        0     2292 2023-06-10 20:36:11.727174 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.nbi
--rw-r--r--   0        0        0    77589 2023-05-10 14:04:48.307277 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.1.nbc
--rw-r--r--   0        0        0    80894 2023-05-09 20:10:40.338051 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.2.nbc
--rw-r--r--   0        0        0     1280 2023-05-10 14:04:48.305276 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.nbi
--rw-r--r--   0        0        0    80894 2023-05-11 20:37:03.860602 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-170.py310.1.nbc
--rw-r--r--   0        0        0     1280 2023-05-11 20:37:03.857602 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-170.py310.nbi
--rw-r--r--   0        0        0    80894 2023-05-11 19:51:22.690984 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.1.nbc
--rw-r--r--   0        0        0    80894 2023-05-11 17:55:29.550170 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.2.nbc
--rw-r--r--   0        0        0     1280 2023-05-11 19:51:22.687981 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.nbi
--rw-r--r--   0        0        0    80894 2023-05-11 20:58:36.790966 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.1.nbc
--rw-r--r--   0        0        0    77589 2023-05-11 22:29:37.429700 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.2.nbc
--rw-r--r--   0        0        0     2321 2023-05-11 22:29:37.426700 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.nbi
--rw-r--r--   0        0        0    77589 2023-05-13 12:36:36.027208 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.1.nbc
--rw-r--r--   0        0        0    80894 2023-05-14 17:03:04.107988 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.2.nbc
--rw-r--r--   0        0        0     2292 2023-05-14 17:03:04.102988 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.nbi
--rw-r--r--   0        0        0    80894 2023-05-12 22:36:32.819436 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-179.py310.1.nbc
--rw-r--r--   0        0        0     1280 2023-05-12 22:36:32.816430 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-179.py310.nbi
--rw-r--r--   0        0        0     5598 2023-04-04 19:53:34.784759 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/triangulator.cpython-38.pyc
--rw-r--r--   0        0        0     8778 2023-04-16 12:58:12.413689 pyxy3d-0.1.3/pyxy3d/triangulate/array_stereo_triangulator.py
--rw-r--r--   0        0        0     5762 2023-04-16 12:58:12.416688 pyxy3d-0.1.3/pyxy3d/triangulate/stereo_points_builder.py
--rw-r--r--   0        0        0     7616 2023-06-08 19:15:56.173904 pyxy3d-0.1.3/pyxy3d/triangulate/sync_packet_triangulator.py
--rw-r--r--   0        0        0     6742 2023-06-22 12:20:08.052238 pyxy3d-0.1.3/README.md
--rw-r--r--   0        0        0     7560 1970-01-01 00:00:00.000000 pyxy3d-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    35190 2023-06-14 20:19:57.480906 pyxy3d-0.1.4/LICENSE.md
+-rw-r--r--   0        0        0      964 2023-06-23 18:50:49.716635 pyxy3d-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2644 2023-06-21 22:25:18.660194 pyxy3d-0.1.4/pyxy3d/__init__.py
+-rw-r--r--   0        0        0      686 2023-06-23 18:50:36.211967 pyxy3d-0.1.4/pyxy3d/__main__.py
+-rw-r--r--   0        0        0     7201 2023-04-16 14:08:55.358491 pyxy3d-0.1.4/pyxy3d/calibration/__pycache__/charuco.cpython-310.pyc
+-rw-r--r--   0        0        0     7111 2023-04-13 18:16:32.164621 pyxy3d-0.1.4/pyxy3d/calibration/__pycache__/charuco.cpython-38.pyc
+-rw-r--r--   0        0        0     3147 2023-04-13 14:11:35.706111 pyxy3d-0.1.4/pyxy3d/calibration/__pycache__/corner_tracker.cpython-38.pyc
+-rw-r--r--   0        0        0     1525 2023-04-13 21:33:14.966692 pyxy3d-0.1.4/pyxy3d/calibration/__pycache__/draw_charuco.cpython-310.pyc
+-rw-r--r--   0        0        0     1517 2023-03-16 18:37:10.539737 pyxy3d-0.1.4/pyxy3d/calibration/__pycache__/draw_charuco.cpython-38.pyc
+-rw-r--r--   0        0        0     7208 2023-06-12 18:45:04.367154 pyxy3d-0.1.4/pyxy3d/calibration/__pycache__/monocalibrator.cpython-310.pyc
+-rw-r--r--   0        0        0     7083 2023-04-13 18:16:59.718066 pyxy3d-0.1.4/pyxy3d/calibration/__pycache__/monocalibrator.cpython-38.pyc
+-rw-r--r--   0        0        0    11365 2023-03-16 18:37:11.887671 pyxy3d-0.1.4/pyxy3d/calibration/__pycache__/omnicalibrator.cpython-38.pyc
+-rw-r--r--   0        0        0     7979 2023-06-08 18:19:03.652989 pyxy3d-0.1.4/pyxy3d/calibration/__pycache__/stereocalibrator.cpython-310.pyc
+-rw-r--r--   0        0        0     7845 2023-04-13 14:31:07.431535 pyxy3d-0.1.4/pyxy3d/calibration/__pycache__/stereocalibrator.cpython-38.pyc
+-rw-r--r--   0        0        0     7001 2023-06-12 12:22:25.787593 pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/__pycache__/capture_volume.cpython-310.pyc
+-rw-r--r--   0        0        0     8147 2023-04-11 10:38:21.551689 pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/__pycache__/capture_volume.cpython-38.pyc
+-rw-r--r--   0        0        0     3517 2023-06-23 17:33:53.743685 pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/__pycache__/point_estimates.cpython-310.pyc
+-rw-r--r--   0        0        0     3651 2023-04-09 20:26:50.741740 pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/__pycache__/point_estimates.cpython-38.pyc
+-rw-r--r--   0        0        0     9626 2023-05-22 14:59:39.828020 pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/__pycache__/quality_controller.cpython-310.pyc
+-rw-r--r--   0        0        0     9567 2023-04-13 18:47:12.691013 pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/__pycache__/quality_controller.cpython-38.pyc
+-rw-r--r--   0        0        0     7294 2023-05-22 14:59:39.817019 pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/__pycache__/set_origin_functions.cpython-310.pyc
+-rw-r--r--   0        0        0     7172 2023-04-06 11:06:35.216555 pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/__pycache__/set_origin_functions.cpython-38.pyc
+-rw-r--r--   0        0        0    10148 2023-06-12 12:14:10.017140 pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/capture_volume.py
+-rw-r--r--   0        0        0  1505952 2023-03-13 23:46:36.934749 pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/capture_volume_stage_1.pkl
+-rw-r--r--   0        0        0     2813 2023-04-13 21:41:08.181971 pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_point_estimates.cpython-310.pyc
+-rw-r--r--   0        0        0     2825 2023-03-16 18:37:13.420982 pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_point_estimates.cpython-38.pyc
+-rw-r--r--   0        0        0     2938 2023-04-16 14:08:57.590539 pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_stereotriangulated_table.cpython-310.pyc
+-rw-r--r--   0        0        0     2963 2023-04-13 14:11:34.686199 pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_stereotriangulated_table.cpython-38.pyc
+-rw-r--r--   0        0        0     3898 2023-03-16 18:13:11.445058 pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/helper_functions/get_point_estimates.py
+-rw-r--r--   0        0        0     4680 2023-04-16 12:58:12.386690 pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/helper_functions/get_stereotriangulated_table.py
+-rw-r--r--   0        0        0     4010 2023-06-23 18:50:36.212965 pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/point_estimates.py
+-rw-r--r--   0        0        0    15888 2023-05-22 13:44:00.083689 pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/quality_controller.py
+-rw-r--r--   0        0        0     1766 2023-03-16 18:13:11.448058 pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/seaborn_summaries.py
+-rw-r--r--   0        0        0    10868 2023-05-22 13:44:00.084688 pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/set_origin_functions.py
+-rw-r--r--   0        0        0     9510 2023-04-16 12:58:12.392689 pyxy3d-0.1.4/pyxy3d/calibration/charuco.py
+-rw-r--r--   0        0        0     1685 2023-03-16 18:13:11.451057 pyxy3d-0.1.4/pyxy3d/calibration/draw_charuco.py
+-rw-r--r--   0        0        0     9886 2023-06-12 16:49:05.518131 pyxy3d-0.1.4/pyxy3d/calibration/monocalibrator.py
+-rw-r--r--   0        0        0    12385 2023-06-08 18:18:45.456813 pyxy3d-0.1.4/pyxy3d/calibration/stereocalibrator.py
+-rw-r--r--   0        0        0     7119 2023-05-22 16:42:44.186443 pyxy3d-0.1.4/pyxy3d/cameras/__pycache__/camera.cpython-310.pyc
+-rw-r--r--   0        0        0     7171 2023-04-12 14:56:03.753093 pyxy3d-0.1.4/pyxy3d/cameras/__pycache__/camera.cpython-38.pyc
+-rw-r--r--   0        0        0     6788 2023-06-10 20:39:00.834305 pyxy3d-0.1.4/pyxy3d/cameras/__pycache__/camera_array.cpython-310.pyc
+-rw-r--r--   0        0        0     6811 2023-04-09 20:26:50.029740 pyxy3d-0.1.4/pyxy3d/cameras/__pycache__/camera_array.cpython-38.pyc
+-rw-r--r--   0        0        0     9199 2023-05-02 22:08:30.006322 pyxy3d-0.1.4/pyxy3d/cameras/__pycache__/camera_array_initializer.cpython-310.pyc
+-rw-r--r--   0        0        0     9153 2023-04-06 11:06:35.358553 pyxy3d-0.1.4/pyxy3d/cameras/__pycache__/camera_array_initializer.cpython-38.pyc
+-rw-r--r--   0        0        0     3161 2023-04-13 21:33:14.970692 pyxy3d-0.1.4/pyxy3d/cameras/__pycache__/data_packets.cpython-310.pyc
+-rw-r--r--   0        0        0     3147 2023-04-13 17:33:55.370369 pyxy3d-0.1.4/pyxy3d/cameras/__pycache__/data_packets.cpython-38.pyc
+-rw-r--r--   0        0        0     8085 2023-06-10 20:05:09.584549 pyxy3d-0.1.4/pyxy3d/cameras/__pycache__/live_stream.cpython-310.pyc
+-rw-r--r--   0        0        0     8585 2023-04-13 17:33:56.274500 pyxy3d-0.1.4/pyxy3d/cameras/__pycache__/live_stream.cpython-38.pyc
+-rw-r--r--   0        0        0     9898 2023-06-23 18:06:50.115857 pyxy3d-0.1.4/pyxy3d/cameras/__pycache__/synchronizer.cpython-310.pyc
+-rw-r--r--   0        0        0    11042 2023-04-13 18:30:26.417813 pyxy3d-0.1.4/pyxy3d/cameras/__pycache__/synchronizer.cpython-38.pyc
+-rw-r--r--   0        0        0    10631 2023-05-22 16:41:37.293000 pyxy3d-0.1.4/pyxy3d/cameras/camera.py
+-rw-r--r--   0        0        0     7710 2023-06-10 20:38:54.275345 pyxy3d-0.1.4/pyxy3d/cameras/camera_array.py
+-rw-r--r--   0        0        0    12868 2023-05-02 22:08:10.579286 pyxy3d-0.1.4/pyxy3d/cameras/camera_array_initializer.py
+-rw-r--r--   0        0        0    11935 2023-06-10 20:04:58.799532 pyxy3d-0.1.4/pyxy3d/cameras/live_stream.py
+-rw-r--r--   0        0        0    13543 2023-06-23 18:06:44.991101 pyxy3d-0.1.4/pyxy3d/cameras/synchronizer.py
+-rw-r--r--   0        0        0    13040 2023-06-12 12:14:10.019141 pyxy3d-0.1.4/pyxy3d/configurator.py
+-rw-r--r--   0        0        0     7036 2023-05-18 21:56:09.817280 pyxy3d-0.1.4/pyxy3d/export.py
+-rw-r--r--   0        0        0     3538 2023-06-12 18:45:08.762112 pyxy3d-0.1.4/pyxy3d/gui/__pycache__/calibrate_capture_volume_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     5691 2023-06-22 12:39:42.763393 pyxy3d-0.1.4/pyxy3d/gui/__pycache__/calibration_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     8693 2023-05-06 16:11:05.603259 pyxy3d-0.1.4/pyxy3d/gui/__pycache__/calibration_wizard.cpython-310.pyc
+-rw-r--r--   0        0        0     7124 2023-06-08 18:19:04.615289 pyxy3d-0.1.4/pyxy3d/gui/__pycache__/charuco_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     8558 2023-06-22 12:39:48.156709 pyxy3d-0.1.4/pyxy3d/gui/__pycache__/extrinsic_calibration_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     2110 2023-05-29 12:41:08.382954 pyxy3d-0.1.4/pyxy3d/gui/__pycache__/log_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     8811 2023-05-02 22:10:09.955994 pyxy3d-0.1.4/pyxy3d/gui/__pycache__/main.cpython-310.pyc
+-rw-r--r--   0        0        0     8445 2023-04-12 14:19:14.529651 pyxy3d-0.1.4/pyxy3d/gui/__pycache__/main.cpython-38.pyc
+-rw-r--r--   0        0        0    11663 2023-06-23 18:41:19.758263 pyxy3d-0.1.4/pyxy3d/gui/__pycache__/main_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     2664 2023-06-08 18:19:04.619290 pyxy3d-0.1.4/pyxy3d/gui/__pycache__/navigation_bars.cpython-310.pyc
+-rw-r--r--   0        0        0     2468 2023-06-02 00:29:24.448977 pyxy3d-0.1.4/pyxy3d/gui/__pycache__/playback_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     9611 2023-06-10 20:31:20.063896 pyxy3d-0.1.4/pyxy3d/gui/__pycache__/post_processing_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     1176 2023-05-29 13:25:02.424999 pyxy3d-0.1.4/pyxy3d/gui/__pycache__/progress_dialog.cpython-310.pyc
+-rw-r--r--   0        0        0     2649 2023-05-22 15:00:23.510630 pyxy3d-0.1.4/pyxy3d/gui/__pycache__/qt_logger.cpython-310.pyc
+-rw-r--r--   0        0        0     2623 2023-04-06 18:40:19.597418 pyxy3d-0.1.4/pyxy3d/gui/__pycache__/qt_logger.cpython-38.pyc
+-rw-r--r--   0        0        0    12241 2023-06-23 18:41:17.940707 pyxy3d-0.1.4/pyxy3d/gui/__pycache__/recording_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     8798 2023-04-12 14:17:47.475386 pyxy3d-0.1.4/pyxy3d/gui/__pycache__/recording_widget.cpython-38.pyc
+-rw-r--r--   0        0        0     2641 2023-04-13 21:41:10.861210 pyxy3d-0.1.4/pyxy3d/gui/__pycache__/widgets.cpython-310.pyc
+-rw-r--r--   0        0        0     2969 2023-04-06 18:40:19.600418 pyxy3d-0.1.4/pyxy3d/gui/__pycache__/widgets.cpython-38.pyc
+-rw-r--r--   0        0        0     6864 2023-05-29 12:41:07.242642 pyxy3d-0.1.4/pyxy3d/gui/__pycache__/wizard_charuco.cpython-310.pyc
+-rw-r--r--   0        0        0     6979 2023-04-06 18:40:19.594417 pyxy3d-0.1.4/pyxy3d/gui/__pycache__/wizard_charuco.cpython-38.pyc
+-rw-r--r--   0        0        0     4851 2023-05-02 13:40:54.299559 pyxy3d-0.1.4/pyxy3d/gui/__pycache__/wizard_directory.cpython-310.pyc
+-rw-r--r--   0        0        0     4903 2023-04-06 18:40:19.608417 pyxy3d-0.1.4/pyxy3d/gui/__pycache__/wizard_directory.cpython-38.pyc
+-rw-r--r--   0        0        0     4052 2023-06-12 16:49:05.519131 pyxy3d-0.1.4/pyxy3d/gui/calibrate_capture_volume_widget.py
+-rw-r--r--   0        0        0    13085 2023-06-02 16:06:24.614359 pyxy3d-0.1.4/pyxy3d/gui/camera_config/__pycache__/camera_config_dialogue.cpython-310.pyc
+-rw-r--r--   0        0        0    13777 2023-03-29 13:33:28.389797 pyxy3d-0.1.4/pyxy3d/gui/camera_config/__pycache__/camera_config_dialogue.cpython-38.pyc
+-rw-r--r--   0        0        0     3658 2023-06-10 20:05:11.213579 pyxy3d-0.1.4/pyxy3d/gui/camera_config/__pycache__/camera_summary_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     4748 2023-06-01 14:22:06.839277 pyxy3d-0.1.4/pyxy3d/gui/camera_config/__pycache__/camera_tabs.cpython-310.pyc
+-rw-r--r--   0        0        0     3850 2023-03-20 23:10:53.097964 pyxy3d-0.1.4/pyxy3d/gui/camera_config/__pycache__/camera_tabs.cpython-38.pyc
+-rw-r--r--   0        0        0     3155 2023-06-02 14:30:41.590277 pyxy3d-0.1.4/pyxy3d/gui/camera_config/__pycache__/frame_emitter.cpython-310.pyc
+-rw-r--r--   0        0        0     2704 2023-03-16 18:37:13.513000 pyxy3d-0.1.4/pyxy3d/gui/camera_config/__pycache__/frame_emitter.cpython-38.pyc
+-rw-r--r--   0        0        0     3619 2023-06-10 20:39:01.831691 pyxy3d-0.1.4/pyxy3d/gui/camera_config/__pycache__/intrinsic_calibration_widget.cpython-310.pyc
+-rw-r--r--   0        0        0    17771 2023-06-02 15:39:41.317656 pyxy3d-0.1.4/pyxy3d/gui/camera_config/camera_config_dialogue.py
+-rw-r--r--   0        0        0     5794 2023-06-10 20:04:49.727607 pyxy3d-0.1.4/pyxy3d/gui/camera_config/camera_summary_widget.py
+-rw-r--r--   0        0        0     3893 2023-06-02 00:28:42.145417 pyxy3d-0.1.4/pyxy3d/gui/camera_config/frame_emitter.py
+-rw-r--r--   0        0        0     3760 2023-06-10 20:38:54.278346 pyxy3d-0.1.4/pyxy3d/gui/camera_config/intrinsic_calibration_widget.py
+-rw-r--r--   0        0        0    11157 2023-06-08 18:18:45.460813 pyxy3d-0.1.4/pyxy3d/gui/charuco_widget.py
+-rw-r--r--   0        0        0    10800 2023-06-15 18:45:15.728953 pyxy3d-0.1.4/pyxy3d/gui/extrinsic_calibration_widget.py
+-rw-r--r--   0        0        0     7468 2023-06-01 18:24:14.049008 pyxy3d-0.1.4/pyxy3d/gui/frame_builders/__pycache__/extrinsic_calibration_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     9143 2023-03-16 18:37:13.553998 pyxy3d-0.1.4/pyxy3d/gui/frame_builders/__pycache__/omni_frame_builder.cpython-38.pyc
+-rw-r--r--   0        0        0     5691 2023-03-16 18:37:13.539983 pyxy3d-0.1.4/pyxy3d/gui/frame_builders/__pycache__/omni_frame_widget.cpython-38.pyc
+-rw-r--r--   0        0        0     9669 2023-06-22 12:39:48.162709 pyxy3d-0.1.4/pyxy3d/gui/frame_builders/__pycache__/paired_frame_builder.cpython-310.pyc
+-rw-r--r--   0        0        0     9881 2023-06-01 18:24:14.063003 pyxy3d-0.1.4/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_builder.cpython-310.pyc
+-rw-r--r--   0        0        0    11456 2023-04-13 17:55:04.283828 pyxy3d-0.1.4/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_builder.cpython-38.pyc
+-rw-r--r--   0        0        0     7359 2023-06-01 14:22:06.856278 pyxy3d-0.1.4/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     7148 2023-04-13 18:41:31.149308 pyxy3d-0.1.4/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_widget.cpython-38.pyc
+-rw-r--r--   0        0        0    13851 2023-06-15 18:45:15.729953 pyxy3d-0.1.4/pyxy3d/gui/frame_builders/paired_frame_builder.py
+-rw-r--r--   0        0        0    19878 2023-04-07 19:40:35.259432 pyxy3d-0.1.4/pyxy3d/gui/icons/pyxy_logo.svg
+-rw-r--r--   0        0        0      941 2023-03-16 18:13:11.463060 pyxy3d-0.1.4/pyxy3d/gui/icons/rotate-camera-left.svg
+-rw-r--r--   0        0        0      944 2023-03-16 18:13:11.464059 pyxy3d-0.1.4/pyxy3d/gui/icons/rotate-camera-right.svg
+-rw-r--r--   0        0        0     2460 2023-05-28 21:21:33.674553 pyxy3d-0.1.4/pyxy3d/gui/log_widget.py
+-rw-r--r--   0        0        0    16022 2023-06-23 18:50:36.214966 pyxy3d-0.1.4/pyxy3d/gui/main_widget.py
+-rw-r--r--   0        0        0     3292 2023-06-08 18:18:45.464814 pyxy3d-0.1.4/pyxy3d/gui/navigation_bars.py
+-rw-r--r--   0        0        0     1988 2023-06-02 00:28:42.150417 pyxy3d-0.1.4/pyxy3d/gui/playback_widget.py
+-rw-r--r--   0        0        0    11310 2023-06-10 20:29:24.686837 pyxy3d-0.1.4/pyxy3d/gui/post_processing_widget.py
+-rw-r--r--   0        0        0      950 2023-05-28 21:21:33.677553 pyxy3d-0.1.4/pyxy3d/gui/progress_dialog.py
+-rw-r--r--   0        0        0    15210 2023-06-23 18:50:36.215967 pyxy3d-0.1.4/pyxy3d/gui/recording_widget.py
+-rw-r--r--   0        0        0     6275 2023-05-13 12:35:31.914917 pyxy3d-0.1.4/pyxy3d/gui/vizualize/__pycache__/camera_mesh.cpython-310.pyc
+-rw-r--r--   0        0        0     6278 2023-04-10 15:11:26.319020 pyxy3d-0.1.4/pyxy3d/gui/vizualize/__pycache__/camera_mesh.cpython-38.pyc
+-rw-r--r--   0        0        0     3198 2023-03-27 01:11:02.734179 pyxy3d-0.1.4/pyxy3d/gui/vizualize/__pycache__/capture_volume_dialog.cpython-38.pyc
+-rw-r--r--   0        0        0     5013 2023-04-08 17:08:48.219160 pyxy3d-0.1.4/pyxy3d/gui/vizualize/__pycache__/capture_volume_visualizer.cpython-38.pyc
+-rw-r--r--   0        0        0     5850 2023-04-08 17:08:47.292159 pyxy3d-0.1.4/pyxy3d/gui/vizualize/__pycache__/capture_volume_widget.cpython-38.pyc
+-rw-r--r--   0        0        0     4920 2023-06-12 12:22:29.640003 pyxy3d-0.1.4/pyxy3d/gui/vizualize/__pycache__/playback_triangulation_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     4522 2023-04-16 14:08:58.474682 pyxy3d-0.1.4/pyxy3d/gui/vizualize/__pycache__/realtime_triangulation_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     2999 2023-06-08 18:19:05.638538 pyxy3d-0.1.4/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_visualizer.cpython-310.pyc
+-rw-r--r--   0        0        0     3506 2023-04-10 15:11:26.253010 pyxy3d-0.1.4/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_visualizer.cpython-38.pyc
+-rw-r--r--   0        0        0     5838 2023-06-12 12:22:27.405313 pyxy3d-0.1.4/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     5615 2023-04-13 18:47:41.885491 pyxy3d-0.1.4/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_widget.cpython-38.pyc
+-rw-r--r--   0        0        0     3404 2023-06-08 18:18:45.466812 pyxy3d-0.1.4/pyxy3d/gui/vizualize/calibration/capture_volume_visualizer.py
+-rw-r--r--   0        0        0     6843 2023-06-12 12:14:10.025140 pyxy3d-0.1.4/pyxy3d/gui/vizualize/calibration/capture_volume_widget.py
+-rw-r--r--   0        0        0     9146 2023-05-12 22:51:00.876793 pyxy3d-0.1.4/pyxy3d/gui/vizualize/camera_mesh.py
+-rw-r--r--   0        0        0     5054 2023-06-12 12:14:10.027140 pyxy3d-0.1.4/pyxy3d/gui/vizualize/playback_triangulation_widget.py
+-rw-r--r--   0        0        0     5450 2023-05-22 13:44:00.101687 pyxy3d-0.1.4/pyxy3d/gui/vizualize/realtime_triangulation_widget.py
+-rw-r--r--   0        0        0     1135 2023-05-18 17:09:55.119648 pyxy3d-0.1.4/pyxy3d/helper.py
+-rw-r--r--   0        0        0     6646 2023-06-15 00:37:58.434754 pyxy3d-0.1.4/pyxy3d/interface.py
+-rw-r--r--   0        0        0     3111 2023-06-23 18:15:31.076726 pyxy3d-0.1.4/pyxy3d/logger.py
+-rw-r--r--   0        0        0     7131 2023-06-23 18:50:36.216966 pyxy3d-0.1.4/pyxy3d/post_processor.py
+-rw-r--r--   0        0        0     8482 2023-05-29 13:25:01.175649 pyxy3d-0.1.4/pyxy3d/recording/__pycache__/recorded_stream.cpython-310.pyc
+-rw-r--r--   0        0        0     7603 2023-04-13 17:33:56.707496 pyxy3d-0.1.4/pyxy3d/recording/__pycache__/recorded_stream.cpython-38.pyc
+-rw-r--r--   0        0        0     6089 2023-06-23 18:18:50.373825 pyxy3d-0.1.4/pyxy3d/recording/__pycache__/video_recorder.cpython-310.pyc
+-rw-r--r--   0        0        0     5376 2023-04-13 14:11:36.908257 pyxy3d-0.1.4/pyxy3d/recording/__pycache__/video_recorder.cpython-38.pyc
+-rw-r--r--   0        0        0    11830 2023-05-28 21:21:33.684552 pyxy3d-0.1.4/pyxy3d/recording/recorded_stream.py
+-rw-r--r--   0        0        0     9108 2023-06-23 18:50:36.219967 pyxy3d-0.1.4/pyxy3d/recording/video_recorder.py
+-rw-r--r--   0        0        0     2818 2023-06-05 20:04:19.162433 pyxy3d-0.1.4/pyxy3d/session/__pycache__/get_stage.cpython-310.pyc
+-rw-r--r--   0        0        0    16634 2023-06-23 17:48:49.082871 pyxy3d-0.1.4/pyxy3d/session/__pycache__/session.cpython-310.pyc
+-rw-r--r--   0        0        0    21689 2023-06-23 18:50:36.220967 pyxy3d-0.1.4/pyxy3d/session/session.py
+-rw-r--r--   0        0        0        0 2023-04-16 12:58:12.408688 pyxy3d-0.1.4/pyxy3d/trackers/__init__.py
+-rw-r--r--   0        0        0      153 2023-04-16 14:08:55.370508 pyxy3d-0.1.4/pyxy3d/trackers/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3955 2023-05-13 12:35:24.878771 pyxy3d-0.1.4/pyxy3d/trackers/__pycache__/charuco_tracker.cpython-310.pyc
+-rw-r--r--   0        0        0     3531 2023-05-13 12:35:26.254677 pyxy3d-0.1.4/pyxy3d/trackers/__pycache__/hand_tracker.cpython-310.pyc
+-rw-r--r--   0        0        0     1123 2023-05-13 12:35:28.030304 pyxy3d-0.1.4/pyxy3d/trackers/__pycache__/helper.cpython-310.pyc
+-rw-r--r--   0        0        0     6774 2023-05-18 18:02:52.161100 pyxy3d-0.1.4/pyxy3d/trackers/__pycache__/holistic_opensim_tracker.cpython-310.pyc
+-rw-r--r--   0        0        0     6262 2023-05-13 12:35:28.041314 pyxy3d-0.1.4/pyxy3d/trackers/__pycache__/holistic_tracker.cpython-310.pyc
+-rw-r--r--   0        0        0     3797 2023-05-13 12:35:28.036311 pyxy3d-0.1.4/pyxy3d/trackers/__pycache__/pose_tracker.cpython-310.pyc
+-rw-r--r--   0        0        0     3515 2023-05-12 22:32:19.505484 pyxy3d-0.1.4/pyxy3d/trackers/__pycache__/threaded_hand_tracker.cpython-310.pyc
+-rw-r--r--   0        0        0     1017 2023-05-18 18:02:48.968666 pyxy3d-0.1.4/pyxy3d/trackers/__pycache__/tracker_enum.cpython-310.pyc
+-rw-r--r--   0        0        0     5004 2023-05-12 22:51:00.882792 pyxy3d-0.1.4/pyxy3d/trackers/charuco_tracker.py
+-rw-r--r--   0        0        0     4651 2023-05-12 22:51:00.883791 pyxy3d-0.1.4/pyxy3d/trackers/hand_tracker.py
+-rw-r--r--   0        0        0     1330 2023-05-12 22:51:00.884792 pyxy3d-0.1.4/pyxy3d/trackers/helper.py
+-rw-r--r--   0        0        0    10677 2023-05-18 17:09:55.120646 pyxy3d-0.1.4/pyxy3d/trackers/holistic_opensim_tracker.py
+-rw-r--r--   0        0        0     9419 2023-05-12 22:51:00.885792 pyxy3d-0.1.4/pyxy3d/trackers/holistic_tracker.py
+-rw-r--r--   0        0        0     4239 2023-05-12 22:51:00.885792 pyxy3d-0.1.4/pyxy3d/trackers/pose_tracker.py
+-rw-r--r--   0        0        0      669 2023-05-18 17:09:55.121648 pyxy3d-0.1.4/pyxy3d/trackers/tracker_enum.py
+-rw-r--r--   0        0        0     5629 2023-04-16 14:08:57.598538 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/array_stereo_triangulator.cpython-310.pyc
+-rw-r--r--   0        0        0     5656 2023-04-13 17:33:55.945379 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/array_stereo_triangulator.cpython-38.pyc
+-rw-r--r--   0        0        0      564 2023-04-24 13:44:16.864821 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/helper.cpython-310.pyc
+-rw-r--r--   0        0        0     5809 2023-05-03 19:22:07.093614 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.cpython-310.pyc
+-rw-r--r--   0        0        0     4640 2023-04-11 11:20:24.830020 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.cpython-38.pyc
+-rw-r--r--   0        0        0   277847 2023-04-17 18:50:37.938076 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.1.nbc
+-rw-r--r--   0        0        0   278178 2023-04-17 18:47:53.733008 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.2.nbc
+-rw-r--r--   0        0        0     1853 2023-04-17 18:50:37.934076 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.nbi
+-rw-r--r--   0        0        0   278065 2023-04-15 22:26:29.919720 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py310.1.nbc
+-rw-r--r--   0        0        0     1795 2023-04-15 22:26:29.916718 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py310.nbi
+-rw-r--r--   0        0        0   277525 2023-04-13 14:11:54.518242 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py38.1.nbc
+-rw-r--r--   0        0        0     1794 2023-04-13 14:11:54.515242 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py38.nbi
+-rw-r--r--   0        0        0   277847 2023-04-15 16:24:55.484079 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-138.py310.1.nbc
+-rw-r--r--   0        0        0     1853 2023-04-15 16:24:55.480077 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-138.py310.nbi
+-rw-r--r--   0        0        0   277847 2023-04-15 21:02:04.894614 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-139.py310.1.nbc
+-rw-r--r--   0        0        0     1853 2023-04-15 21:02:04.889631 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-139.py310.nbi
+-rw-r--r--   0        0        0   277790 2023-04-09 20:05:59.716347 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-86.py38.1.nbc
+-rw-r--r--   0        0        0     1793 2023-04-09 20:05:59.712345 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-86.py38.nbi
+-rw-r--r--   0        0        0   277795 2023-04-09 20:08:37.404028 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-88.py38.1.nbc
+-rw-r--r--   0        0        0     1793 2023-04-09 20:08:37.400042 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-88.py38.nbi
+-rw-r--r--   0        0        0    80840 2023-04-17 18:50:25.192073 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.unique_with_counts-118.py310.1.nbc
+-rw-r--r--   0        0        0     1278 2023-04-17 18:50:25.189073 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.unique_with_counts-118.py310.nbi
+-rw-r--r--   0        0        0     4903 2023-04-16 14:08:57.603539 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/stereo_points_builder.cpython-310.pyc
+-rw-r--r--   0        0        0     4910 2023-04-13 17:33:55.950369 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/stereo_points_builder.cpython-38.pyc
+-rw-r--r--   0        0        0     5522 2023-06-08 19:16:30.042145 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.cpython-310.pyc
+-rw-r--r--   0        0        0   277993 2023-06-10 20:35:53.847895 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.1.nbc
+-rw-r--r--   0        0        0   278337 2023-06-10 20:36:00.364127 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.2.nbc
+-rw-r--r--   0        0        0   275198 2023-06-10 20:36:15.587107 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.3.nbc
+-rw-r--r--   0        0        0     3826 2023-06-10 20:36:15.585108 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.nbi
+-rw-r--r--   0        0        0   274936 2023-05-07 17:31:11.859065 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-170.py310.1.nbc
+-rw-r--r--   0        0        0     1819 2023-05-07 17:31:11.856057 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-170.py310.nbi
+-rw-r--r--   0        0        0   280483 2023-05-11 20:37:44.633248 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-186.py310.1.nbc
+-rw-r--r--   0        0        0     1855 2023-05-11 20:37:44.630243 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-186.py310.nbi
+-rw-r--r--   0        0        0   277957 2023-05-11 19:51:33.032983 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.1.nbc
+-rw-r--r--   0        0        0   278013 2023-05-11 17:55:35.449169 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.2.nbc
+-rw-r--r--   0        0        0   278357 2023-05-11 17:56:15.957610 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.3.nbc
+-rw-r--r--   0        0        0     1855 2023-05-11 19:51:33.028983 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.nbi
+-rw-r--r--   0        0        0   277977 2023-05-11 20:58:46.910959 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.1.nbc
+-rw-r--r--   0        0        0   274956 2023-05-11 22:29:46.557422 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.2.nbc
+-rw-r--r--   0        0        0   280725 2023-05-12 22:34:01.184507 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.3.nbc
+-rw-r--r--   0        0        0     3913 2023-05-12 22:34:01.181521 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.nbi
+-rw-r--r--   0        0        0   274956 2023-05-13 12:36:45.045739 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.1.nbc
+-rw-r--r--   0        0        0   277993 2023-05-14 17:03:11.852980 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.2.nbc
+-rw-r--r--   0        0        0   278337 2023-05-14 17:03:18.755882 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.3.nbc
+-rw-r--r--   0        0        0     3855 2023-05-14 17:03:18.752878 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.nbi
+-rw-r--r--   0        0        0   278215 2023-05-12 22:36:41.576195 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-195.py310.1.nbc
+-rw-r--r--   0        0        0     1797 2023-05-12 22:36:41.573185 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-195.py310.nbi
+-rw-r--r--   0        0        0    80914 2023-06-10 20:35:46.176596 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.1.nbc
+-rw-r--r--   0        0        0    77589 2023-06-10 20:36:11.729164 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.2.nbc
+-rw-r--r--   0        0        0     2292 2023-06-10 20:36:11.727174 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.nbi
+-rw-r--r--   0        0        0    77589 2023-05-10 14:04:48.307277 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.1.nbc
+-rw-r--r--   0        0        0    80894 2023-05-09 20:10:40.338051 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.2.nbc
+-rw-r--r--   0        0        0     1280 2023-05-10 14:04:48.305276 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.nbi
+-rw-r--r--   0        0        0    80894 2023-05-11 20:37:03.860602 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-170.py310.1.nbc
+-rw-r--r--   0        0        0     1280 2023-05-11 20:37:03.857602 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-170.py310.nbi
+-rw-r--r--   0        0        0    80894 2023-05-11 19:51:22.690984 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.1.nbc
+-rw-r--r--   0        0        0    80894 2023-05-11 17:55:29.550170 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.2.nbc
+-rw-r--r--   0        0        0     1280 2023-05-11 19:51:22.687981 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.nbi
+-rw-r--r--   0        0        0    80894 2023-05-11 20:58:36.790966 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.1.nbc
+-rw-r--r--   0        0        0    77589 2023-05-11 22:29:37.429700 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.2.nbc
+-rw-r--r--   0        0        0     2321 2023-05-11 22:29:37.426700 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.nbi
+-rw-r--r--   0        0        0    77589 2023-05-13 12:36:36.027208 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.1.nbc
+-rw-r--r--   0        0        0    80894 2023-05-14 17:03:04.107988 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.2.nbc
+-rw-r--r--   0        0        0     2292 2023-05-14 17:03:04.102988 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.nbi
+-rw-r--r--   0        0        0    80894 2023-05-12 22:36:32.819436 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-179.py310.1.nbc
+-rw-r--r--   0        0        0     1280 2023-05-12 22:36:32.816430 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-179.py310.nbi
+-rw-r--r--   0        0        0     5598 2023-04-04 19:53:34.784759 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/triangulator.cpython-38.pyc
+-rw-r--r--   0        0        0     8778 2023-04-16 12:58:12.413689 pyxy3d-0.1.4/pyxy3d/triangulate/array_stereo_triangulator.py
+-rw-r--r--   0        0        0     5762 2023-04-16 12:58:12.416688 pyxy3d-0.1.4/pyxy3d/triangulate/stereo_points_builder.py
+-rw-r--r--   0        0        0     7616 2023-06-08 19:15:56.173904 pyxy3d-0.1.4/pyxy3d/triangulate/sync_packet_triangulator.py
+-rw-r--r--   0        0        0     7485 2023-06-23 18:50:36.209967 pyxy3d-0.1.4/README.md
+-rw-r--r--   0        0        0     8244 1970-01-01 00:00:00.000000 pyxy3d-0.1.4/PKG-INFO
```

### Comparing `pyxy3d-0.1.3/LICENSE.md` & `pyxy3d-0.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyproject.toml` & `pyxy3d-0.1.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "pyxy3d"
-version = "0.1.3"
+version = "0.1.4"
 description = "A package for calibrating standard webcams to enable 3d motion tracking"
 authors = ["Mac Prible <prible@gmail.com>"]
 license = "AGPL-3.0-only"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = ">=3.10, <3.12"
+python = ">=3.10, <3.10.11"  #frequent segfaults in python 3.10.11
 opencv-contrib-python = "^4.7"
 PyQt6 = "^6.4.0"
 pandas = "^1.5.0"
 scipy = "^1.10.1"
 pyqtgraph = "^0.13.2"
 PyOpenGL = "^3.1.6"
 toml = "^0.10.2"
```

### Comparing `pyxy3d-0.1.3/pyxy3d/__init__.py` & `pyxy3d-0.1.4/pyxy3d/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/calibration/__pycache__/charuco.cpython-310.pyc` & `pyxy3d-0.1.4/pyxy3d/calibration/__pycache__/charuco.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/calibration/__pycache__/charuco.cpython-38.pyc` & `pyxy3d-0.1.4/pyxy3d/calibration/__pycache__/charuco.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/calibration/__pycache__/corner_tracker.cpython-38.pyc` & `pyxy3d-0.1.4/pyxy3d/calibration/__pycache__/corner_tracker.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/calibration/__pycache__/draw_charuco.cpython-310.pyc` & `pyxy3d-0.1.4/pyxy3d/calibration/__pycache__/draw_charuco.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/calibration/__pycache__/draw_charuco.cpython-38.pyc` & `pyxy3d-0.1.4/pyxy3d/calibration/__pycache__/draw_charuco.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/calibration/__pycache__/monocalibrator.cpython-310.pyc` & `pyxy3d-0.1.4/pyxy3d/calibration/__pycache__/monocalibrator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/calibration/__pycache__/monocalibrator.cpython-38.pyc` & `pyxy3d-0.1.4/pyxy3d/calibration/__pycache__/monocalibrator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/calibration/__pycache__/omnicalibrator.cpython-38.pyc` & `pyxy3d-0.1.4/pyxy3d/calibration/__pycache__/omnicalibrator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/calibration/__pycache__/stereocalibrator.cpython-310.pyc` & `pyxy3d-0.1.4/pyxy3d/calibration/__pycache__/stereocalibrator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/calibration/__pycache__/stereocalibrator.cpython-38.pyc` & `pyxy3d-0.1.4/pyxy3d/calibration/__pycache__/stereocalibrator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/__pycache__/capture_volume.cpython-310.pyc` & `pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/__pycache__/capture_volume.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/__pycache__/capture_volume.cpython-38.pyc` & `pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/__pycache__/capture_volume.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/__pycache__/point_estimates.cpython-310.pyc` & `pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/__pycache__/point_estimates.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue May  2 22:08:10 2023 UTC, .py size: 3631 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 15% similar despite different names*

```diff
@@ -1,201 +1,229 @@
-00000000: 6f0d 0d0a 0000 0000 ca89 5164 2f0e 0000  o.........Qd/...
+00000000: 550d 0d0a 0000 0000 511f 3364 7810 0000  U.......Q.3dx...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 8000 0000 6400  .....@...s....d.
+00000020: 0004 0000 0040 0000 0073 e000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6501 6a02 a003 6504 a101  d.l.Z.e.j...e...
 00000040: 5a02 6400 6402 6c05 6d06 5a06 0100 6400  Z.d.d.l.m.Z...d.
 00000050: 6403 6c07 6d08 5a08 0100 6400 6401 6c09  d.l.m.Z...d.d.l.
 00000060: 5a0a 6400 6401 6c0b 5a0c 6400 6404 6c0d  Z.d.d.l.Z.d.d.l.
 00000070: 6d0e 5a0e 0100 6400 6405 6c0f 6d10 5a10  m.Z...d.d.l.m.Z.
-00000080: 0100 6406 5a11 650e 4700 6407 6408 8400  ..d.Z.e.G.d.d...
-00000090: 6408 8302 8301 5a12 6409 6513 640a 6512  d.....Z.d.e.d.e.
-000000a0: 6604 640b 640c 8404 5a14 6401 5300 290d  f.d.d...Z.d.S.).
-000000b0: e900 0000 004e 2901 da04 5061 7468 2901  .....N)...Path).
-000000c0: da0a 6c69 6c5f 6d61 7472 6978 2901 da09  ..lil_matrix)...
-000000d0: 6461 7461 636c 6173 7329 01da 1c67 6574  dataclass)...get
-000000e0: 5f73 7465 7265 6f74 7269 616e 6775 6c61  _stereotriangula
-000000f0: 7465 645f 7461 626c 65e9 0600 0000 6300  ted_table.....c.
-00000100: 0000 0000 0000 0000 0000 0000 0000 0003  ................
-00000110: 0000 0040 0000 0073 8200 0000 6500 5a01  ...@...s....e.Z.
-00000120: 6400 5a02 5500 6401 5a03 6504 6a05 6506  d.Z.U.d.Z.e.j.e.
-00000130: 6402 3c00 6504 6a05 6506 6403 3c00 6504  d.<.e.j.e.d.<.e.
-00000140: 6a05 6506 6404 3c00 6504 6a05 6506 6405  j.e.d.<.e.j.e.d.
-00000150: 3c00 6504 6a05 6506 6406 3c00 6504 6a05  <.e.j.e.d.<.e.j.
-00000160: 6506 6407 3c00 6507 6408 6409 8400 8301  e.d.<.e.d.d.....
-00000170: 5a08 6507 640a 640b 8400 8301 5a09 6507  Z.e.d.d.....Z.e.
-00000180: 640c 640d 8400 8301 5a0a 640e 640f 8400  d.d.....Z.d.d...
-00000190: 5a0b 6410 6411 8400 5a0c 6412 5300 2913  Z.d.d...Z.d.S.).
-000001a0: da0e 506f 696e 7445 7374 696d 6174 6573  ..PointEstimates
-000001b0: 6128 0100 000a 2020 2020 496e 6974 6961  a(....    Initia
-000001c0: 6c69 7a65 6420 6672 6f6d 2074 7269 616e  lized from trian
-000001d0: 6775 6c61 7465 645f 706f 696e 7473 2e63  gulated_points.c
-000001e0: 7376 2074 6f20 7072 6f76 6964 6520 7468  sv to provide th
-000001f0: 6520 666f 726d 6174 7469 6e67 206f 6620  e formatting of 
-00000200: 6461 7461 2072 6571 7569 7265 6420 666f  data required fo
-00000210: 7220 6275 6e64 6c65 2061 646a 7573 746d  r bundle adjustm
-00000220: 656e 740a 2020 2020 2266 756c 6c22 2069  ent.    "full" i
-00000230: 7320 7573 6564 2068 6572 6520 6265 6361  s used here beca
-00000240: 7573 6520 7468 6572 6520 6973 2063 7572  use there is cur
-00000250: 7265 6e74 6c79 2061 206d 6574 686f 6420  rently a method 
-00000260: 746f 2066 696c 7465 7220 7468 6520 6461  to filter the da
-00000270: 7461 2062 6173 6564 206f 6e20 7265 7072  ta based on repr
-00000280: 6f6a 6563 7469 6f6e 2065 7272 6f72 0a20  ojection error. 
-00000290: 2020 204e 6f74 2073 7572 6520 6966 2069     Not sure if i
-000002a0: 7420 7769 6c6c 2062 6520 7573 6564 2067  t will be used g
-000002b0: 6f69 6e67 2066 6f72 7761 7264 2c20 6275  oing forward, bu
-000002c0: 7420 6974 2072 656d 6169 6e73 2068 6572  t it remains her
-000002d0: 6520 6966 2073 6f2e 0a20 2020 205a 0c73  e if so..    Z.s
-000002e0: 796e 635f 696e 6469 6365 73da 0e63 616d  ync_indices..cam
-000002f0: 6572 615f 696e 6469 6365 73da 0870 6f69  era_indices..poi
-00000300: 6e74 5f69 64da 0369 6d67 da0b 6f62 6a5f  nt_id..img..obj_
-00000310: 696e 6469 6365 73da 036f 626a 6301 0000  indices..objc...
-00000320: 0000 0000 0000 0000 0001 0000 0003 0000  ................
-00000330: 0043 0000 0073 0e00 0000 7400 a001 7c00  .C...s....t...|.
-00000340: 6a02 a101 6a03 5300 2901 4e29 04da 026e  j...j.S.).N)...n
-00000350: 70da 0675 6e69 7175 6572 0800 0000 da04  p..uniquer......
-00000360: 7369 7a65 a901 da04 7365 6c66 a900 7212  size....self..r.
-00000370: 0000 00fa 5543 3a5c 5573 6572 735c 4d61  ....UC:\Users\Ma
-00000380: 6320 5072 6962 6c65 5c72 6570 6f73 5c70  c Prible\repos\p
-00000390: 7978 7933 645c 7079 7879 3364 5c63 616c  yxy3d\pyxy3d\cal
-000003a0: 6962 7261 7469 6f6e 5c63 6170 7475 7265  ibration\capture
-000003b0: 5f76 6f6c 756d 655c 706f 696e 745f 6573  _volume\point_es
-000003c0: 7469 6d61 7465 732e 7079 da09 6e5f 6361  timates.py..n_ca
-000003d0: 6d65 7261 7326 0000 0073 0200 0000 0e02  meras&...s......
-000003e0: 7a18 506f 696e 7445 7374 696d 6174 6573  z.PointEstimates
-000003f0: 2e6e 5f63 616d 6572 6173 6301 0000 0000  .n_camerasc.....
-00000400: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
-00000410: 0000 00f3 0c00 0000 7c00 6a00 6a01 6401  ........|.j.j.d.
-00000420: 1900 5300 a902 4e72 0100 0000 2902 720c  ..S...Nr....).r.
-00000430: 0000 00da 0573 6861 7065 7210 0000 0072  .....shaper....r
-00000440: 1200 0000 7212 0000 0072 1300 0000 da0c  ....r....r......
-00000450: 6e5f 6f62 6a5f 706f 696e 7473 2a00 0000  n_obj_points*...
-00000460: f302 0000 000c 027a 1b50 6f69 6e74 4573  .......z.PointEs
-00000470: 7469 6d61 7465 732e 6e5f 6f62 6a5f 706f  timates.n_obj_po
-00000480: 696e 7473 6301 0000 0000 0000 0000 0000  intsc...........
-00000490: 0001 0000 0002 0000 0043 0000 0072 1500  .........C...r..
-000004a0: 0000 7216 0000 0029 0272 0a00 0000 7217  ..r....).r....r.
-000004b0: 0000 0072 1000 0000 7212 0000 0072 1200  ...r....r....r..
-000004c0: 0000 7213 0000 00da 0c6e 5f69 6d67 5f70  ..r......n_img_p
-000004d0: 6f69 6e74 732e 0000 0072 1900 0000 7a1b  oints....r....z.
-000004e0: 506f 696e 7445 7374 696d 6174 6573 2e6e  PointEstimates.n
-000004f0: 5f69 6d67 5f70 6f69 6e74 7363 0100 0000  _img_pointsc....
-00000500: 0000 0000 0000 0000 0600 0000 0700 0000  ................
-00000510: 4300 0000 73e2 0000 007c 006a 006a 0164  C...s....|.j.j.d
-00000520: 0114 007d 017c 006a 0274 0314 007c 006a  ...}.|.j.t...|.j
-00000530: 0464 0214 0017 007d 0274 057c 017c 0266  .d.....}.t.|.|.f
-00000540: 0274 0664 038d 027d 0374 07a0 087c 006a  .t.d...}.t...|.j
-00000550: 006a 01a1 017d 0474 0974 0383 0144 005d  .j...}.t.t...D.]
-00000560: 1e7d 0564 047c 0364 017c 0414 007c 006a  .}.d.|.d.|...|.j
-00000570: 0074 0314 007c 0517 0066 023c 0064 047c  .t...|...f.<.d.|
-00000580: 0364 017c 0414 0064 0417 007c 006a 0074  .d.|...d...|.j.t
-00000590: 0314 007c 0517 0066 023c 0071 2374 0964  ...|...f.<.q#t.d
-000005a0: 0283 0144 005d 287d 0564 047c 0364 017c  ...D.](}.d.|.d.|
-000005b0: 0414 007c 006a 0274 0314 007c 006a 0a64  ...|.j.t...|.j.d
-000005c0: 0214 0017 007c 0517 0066 023c 0064 047c  .....|...f.<.d.|
-000005d0: 0364 017c 0414 0064 0417 007c 006a 0274  .d.|...d...|.j.t
-000005e0: 0314 007c 006a 0a64 0214 0017 007c 0517  ...|.j.d.....|..
-000005f0: 0066 023c 0071 467c 0353 0029 0561 2401  .f.<.qF|.S.).a$.
-00000600: 0000 7072 6f76 6964 6520 7468 6520 7370  ..provide the sp
-00000610: 6172 7369 7479 2073 7472 7563 7475 7265  arsity structure
-00000620: 2066 6f72 2074 6865 204a 6163 6f62 6961   for the Jacobia
-00000630: 6e20 2865 6c65 6d65 6e74 7320 7468 6174  n (elements that
-00000640: 2061 7265 206e 6f74 207a 6572 6f29 0a20   are not zero). 
-00000650: 2020 2020 2020 206e 5f70 6f69 6e74 733a         n_points:
-00000660: 206e 756d 6265 7220 6f66 2075 6e69 7175   number of uniqu
-00000670: 6520 3364 2070 6f69 6e74 733b 2074 6865  e 3d points; the
-00000680: 7365 2077 696c 6c20 6561 6368 2068 6176  se will each hav
-00000690: 6520 6174 206c 6561 7374 206f 6e65 2062  e at least one b
-000006a0: 7574 2070 6f74 656e 7469 616c 6c79 206d  ut potentially m
-000006b0: 6f72 6520 6173 736f 6369 6174 6564 2032  ore associated 2
-000006c0: 6420 706f 696e 7473 0a20 2020 2020 2020  d points.       
-000006d0: 2070 6f69 6e74 5f69 6e64 6963 6573 3a20   point_indices: 
-000006e0: 6120 7665 6374 6f72 2074 6861 7420 6d61  a vector that ma
-000006f0: 7073 2074 6865 2032 6420 706f 696e 7473  ps the 2d points
-00000700: 2074 6f20 7468 6569 7220 6173 736f 6369   to their associ
-00000710: 6174 6564 2033 6420 706f 696e 740a 2020  ated 3d point.  
-00000720: 2020 2020 2020 e902 0000 00e9 0300 0000        ..........
-00000730: 2901 da05 6474 7970 65e9 0100 0000 290b  )...dtype.....).
-00000740: 7208 0000 0072 0f00 0000 7214 0000 00da  r....r....r.....
-00000750: 1243 414d 4552 415f 5041 5241 4d5f 434f  .CAMERA_PARAM_CO
-00000760: 554e 5472 1800 0000 7203 0000 00da 0369  UNTr....r......i
-00000770: 6e74 720d 0000 00da 0661 7261 6e67 65da  ntr......arange.
-00000780: 0572 616e 6765 720b 0000 0029 0672 1100  .ranger....).r..
-00000790: 0000 da01 6dda 016e da01 41da 0169 da01  ....m..n..A..i..
-000007a0: 7372 1200 0000 7212 0000 0072 1300 0000  sr....r....r....
-000007b0: da14 6765 745f 7370 6172 7369 7479 5f70  ..get_sparsity_p
-000007c0: 6174 7465 726e 3200 0000 7320 0000 000c  attern2...s ....
-000007d0: 0614 0110 010e 020c 011a 0120 010c 0224  ........... ...$
-000007e0: 0102 0402 fd0a 0116 0102 ff04 ff04 057a  ...............z
-000007f0: 2350 6f69 6e74 4573 7469 6d61 7465 732e  #PointEstimates.
-00000800: 6765 745f 7370 6172 7369 7479 5f70 6174  get_sparsity_pat
-00000810: 7465 726e 6302 0000 0000 0000 0000 0000  ternc...........
-00000820: 0003 0000 0004 0000 0043 0000 0073 2800  .........C...s(.
-00000830: 0000 7c01 7c00 6a00 7401 1400 6401 8502  ..|.|.j.t...d...
-00000840: 1900 7d02 7c02 a002 6402 6403 a102 7d02  ..}.|...d.d...}.
-00000850: 7c02 7c00 5f03 6401 5300 2904 7ab7 0a20  |.|._.d.S.).z.. 
-00000860: 2020 2020 2020 2050 726f 7669 6465 6420         Provided 
-00000870: 7769 7468 2074 6865 206c 6561 7374 5f73  with the least_s
-00000880: 7175 6172 6573 2065 7374 696d 6174 6520  quares estimate 
-00000890: 6f66 2074 6865 2062 6573 7420 6669 7420  of the best fit 
-000008a0: 6f66 206d 6f64 656c 2070 6172 616d 6574  of model paramet
-000008b0: 6572 7320 2869 6e63 6c75 6469 6e67 2063  ers (including c
-000008c0: 616d 6572 6120 3644 6f46 290a 2020 2020  amera 6DoF).    
-000008d0: 2020 2020 7061 7273 6520 6f75 7420 7468      parse out th
-000008e0: 6520 782c 792c 7a20 6f62 6a65 6374 2070  e x,y,z object p
-000008f0: 6f73 6974 696f 6e73 2061 6e64 2075 7064  ositions and upd
-00000900: 6174 6520 7365 6c66 2e6f 626a 0a20 2020  ate self.obj.   
-00000910: 2020 2020 204e e9ff ffff ff72 1c00 0000       N.....r....
-00000920: 2904 7214 0000 0072 1f00 0000 da07 7265  ).r....r......re
-00000930: 7368 6170 6572 0c00 0000 2903 7211 0000  shaper....).r...
-00000940: 00da 116c 6561 7374 5f73 715f 7265 7375  ...least_sq_resu
-00000950: 6c74 5f78 5a03 7879 7a72 1200 0000 7212  lt_xZ.xyzr....r.
-00000960: 0000 0072 1300 0000 da0e 7570 6461 7465  ...r......update
-00000970: 5f6f 626a 5f78 797a 4a00 0000 7306 0000  _obj_xyzJ...s...
-00000980: 0012 060c 010a 027a 1d50 6f69 6e74 4573  .......z.PointEs
-00000990: 7469 6d61 7465 732e 7570 6461 7465 5f6f  timates.update_o
-000009a0: 626a 5f78 797a 4e29 0dda 085f 5f6e 616d  bj_xyzN)...__nam
-000009b0: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
-000009c0: 0c5f 5f71 7561 6c6e 616d 655f 5fda 075f  .__qualname__.._
-000009d0: 5f64 6f63 5f5f 720d 0000 00da 076e 6461  _doc__r......nda
-000009e0: 7272 6179 da0f 5f5f 616e 6e6f 7461 7469  rray..__annotati
-000009f0: 6f6e 735f 5fda 0870 726f 7065 7274 7972  ons__..propertyr
-00000a00: 1400 0000 7218 0000 0072 1a00 0000 7228  ....r....r....r(
-00000a10: 0000 0072 2c00 0000 7212 0000 0072 1200  ...r,...r....r..
-00000a20: 0000 7212 0000 0072 1300 0000 7207 0000  ..r....r....r...
-00000a30: 0015 0000 0073 2000 0000 0a00 0402 0a06  .....s .........
-00000a40: 0a01 0a01 0a01 0a01 0a01 0204 0a01 0203  ................
-00000a50: 0a01 0203 0a01 0803 0c18 7207 0000 00da  ..........r.....
-00000a60: 0663 6f6e 6669 67da 0672 6574 7572 6e63  .config..returnc
-00000a70: 0100 0000 0000 0000 0000 0000 0500 0000  ................
-00000a80: 0400 0000 4300 0000 733a 0000 007c 0064  ....C...s:...|.d
-00000a90: 0119 007d 017c 01a0 00a1 0044 005d 0b5c  ...}.|.....D.].\
-00000aa0: 027d 027d 0374 01a0 027c 03a1 017c 017c  .}.}.t...|...|.|
-00000ab0: 023c 0071 0874 0364 0269 007c 01a4 018e  .<.q.t.d.i.|....
-00000ac0: 017d 047c 0453 0029 034e da0f 706f 696e  .}.|.S.).N..poin
-00000ad0: 745f 6573 7469 6d61 7465 7372 1200 0000  t_estimatesr....
-00000ae0: 2904 da05 6974 656d 7372 0d00 0000 da05  )...itemsr......
-00000af0: 6172 7261 7972 0700 0000 2905 7234 0000  arrayr....).r4..
-00000b00: 005a 1470 6f69 6e74 5f65 7374 696d 6174  .Z.point_estimat
-00000b10: 6573 5f64 6963 74da 036b 6579 da05 7661  es_dict..key..va
-00000b20: 6c75 6572 3600 0000 7212 0000 0072 1200  luer6...r....r..
-00000b30: 0000 7213 0000 00da 146c 6f61 645f 706f  ..r......load_po
-00000b40: 696e 745f 6573 7469 6d61 7465 7358 0000  int_estimatesX..
-00000b50: 0073 0a00 0000 0801 1002 1001 0e02 0401  .s..............
-00000b60: 723b 0000 0029 15da 0d70 7978 7933 642e  r;...)...pyxy3d.
-00000b70: 6c6f 6767 6572 da06 7079 7879 3364 da06  logger..pyxy3d..
-00000b80: 6c6f 6767 6572 da03 6765 7472 2d00 0000  logger..getr-...
-00000b90: da07 7061 7468 6c69 6272 0200 0000 5a0c  ..pathlibr....Z.
-00000ba0: 7363 6970 792e 7370 6172 7365 7203 0000  scipy.sparser...
-00000bb0: 00da 0670 616e 6461 73da 0270 64da 056e  ...pandas..pd..n
-00000bc0: 756d 7079 720d 0000 00da 0b64 6174 6163  umpyr......datac
-00000bd0: 6c61 7373 6573 7204 0000 005a 4f70 7978  lassesr....ZOpyx
-00000be0: 7933 642e 6361 6c69 6272 6174 696f 6e2e  y3d.calibration.
-00000bf0: 6361 7074 7572 655f 766f 6c75 6d65 2e68  capture_volume.h
-00000c00: 656c 7065 725f 6675 6e63 7469 6f6e 732e  elper_functions.
-00000c10: 6765 745f 7374 6572 656f 7472 6961 6e67  get_stereotriang
-00000c20: 756c 6174 6564 5f74 6162 6c65 7205 0000  ulated_tabler...
-00000c30: 0072 1f00 0000 7207 0000 00da 0464 6963  .r....r......dic
-00000c40: 7472 3b00 0000 7212 0000 0072 1200 0000  tr;...r....r....
-00000c50: 7212 0000 0072 1300 0000 da08 3c6d 6f64  r....r......<mod
-00000c60: 756c 653e 0100 0000 7318 0000 0008 050c  ule>....s.......
-00000c70: 010c 020c 0208 0208 010c 010c 0104 0202  ................
-00000c80: 0310 0116 42                             ....B
+00000080: 6d11 5a11 0100 6400 6406 6c12 6d13 5a13  m.Z...d.d.l.m.Z.
+00000090: 0100 6407 5a14 650e 4700 6408 6409 8400  ..d.Z.e.G.d.d...
+000000a0: 6409 8302 8301 5a15 6516 6515 640a 9c02  d.....Z.e.e.d...
+000000b0: 640b 640c 8404 5a17 6504 640d 6b02 72dc  d.d...Z.e.d.k.r.
+000000c0: 6400 640e 6c01 6d18 5a18 0100 6400 640f  d.d.l.m.Z...d.d.
+000000d0: 6c19 6d1a 5a1a 0100 6506 6518 6410 6411  l.m.Z...e.e.d.d.
+000000e0: 8303 5a1b 6506 651b 6412 8302 5a1c 651d  ..Z.e.e.d...Z.e.
+000000f0: 6506 651b 6413 8302 8301 a011 a100 5a1e  e.e.d.........Z.
+00000100: 651a 651e 651c 8302 5a1f 6401 5300 2914  e.e.e...Z.d.S.).
+00000110: e900 0000 004e 2901 da04 5061 7468 2901  .....N)...Path).
+00000120: da0a 6c69 6c5f 6d61 7472 6978 2901 da09  ..lil_matrix)...
+00000130: 6461 7461 636c 6173 7329 02da 0b43 616d  dataclass)...Cam
+00000140: 6572 6141 7272 6179 da10 6765 745f 6361  eraArray..get_ca
+00000150: 6d65 7261 5f61 7272 6179 2901 da1c 6765  mera_array)...ge
+00000160: 745f 7374 6572 656f 7472 6961 6e67 756c  t_stereotriangul
+00000170: 6174 6564 5f74 6162 6c65 e906 0000 0063  ated_table.....c
+00000180: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000190: 0300 0000 4000 0000 7382 0000 0065 005a  ....@...s....e.Z
+000001a0: 0164 005a 0255 0064 015a 0365 046a 0565  .d.Z.U.d.Z.e.j.e
+000001b0: 0664 023c 0065 046a 0565 0664 033c 0065  .d.<.e.j.e.d.<.e
+000001c0: 046a 0565 0664 043c 0065 046a 0565 0664  .j.e.d.<.e.j.e.d
+000001d0: 053c 0065 046a 0565 0664 063c 0065 046a  .<.e.j.e.d.<.e.j
+000001e0: 0565 0664 073c 0065 0764 0864 0984 0083  .e.d.<.e.d.d....
+000001f0: 015a 0865 0764 0a64 0b84 0083 015a 0965  .Z.e.d.d.....Z.e
+00000200: 0764 0c64 0d84 0083 015a 0a64 0e64 0f84  .d.d.....Z.d.d..
+00000210: 005a 0b64 1064 1184 005a 0c64 1253 0029  .Z.d.d...Z.d.S.)
+00000220: 13da 0e50 6f69 6e74 4573 7469 6d61 7465  ...PointEstimate
+00000230: 7361 2801 0000 0a20 2020 2049 6e69 7469  sa(....    Initi
+00000240: 616c 697a 6564 2066 726f 6d20 7472 6961  alized from tria
+00000250: 6e67 756c 6174 6564 5f70 6f69 6e74 732e  ngulated_points.
+00000260: 6373 7620 746f 2070 726f 7669 6465 2074  csv to provide t
+00000270: 6865 2066 6f72 6d61 7474 696e 6720 6f66  he formatting of
+00000280: 2064 6174 6120 7265 7175 6972 6564 2066   data required f
+00000290: 6f72 2062 756e 646c 6520 6164 6a75 7374  or bundle adjust
+000002a0: 6d65 6e74 0a20 2020 2022 6675 6c6c 2220  ment.    "full" 
+000002b0: 6973 2075 7365 6420 6865 7265 2062 6563  is used here bec
+000002c0: 6175 7365 2074 6865 7265 2069 7320 6375  ause there is cu
+000002d0: 7272 656e 746c 7920 6120 6d65 7468 6f64  rrently a method
+000002e0: 2074 6f20 6669 6c74 6572 2074 6865 2064   to filter the d
+000002f0: 6174 6120 6261 7365 6420 6f6e 2072 6570  ata based on rep
+00000300: 726f 6a65 6374 696f 6e20 6572 726f 720a  rojection error.
+00000310: 2020 2020 4e6f 7420 7375 7265 2069 6620      Not sure if 
+00000320: 6974 2077 696c 6c20 6265 2075 7365 6420  it will be used 
+00000330: 676f 696e 6720 666f 7277 6172 642c 2062  going forward, b
+00000340: 7574 2069 7420 7265 6d61 696e 7320 6865  ut it remains he
+00000350: 7265 2069 6620 736f 2e0a 2020 2020 5a0c  re if so..    Z.
+00000360: 7379 6e63 5f69 6e64 6963 6573 da0e 6361  sync_indices..ca
+00000370: 6d65 7261 5f69 6e64 6963 6573 da08 706f  mera_indices..po
+00000380: 696e 745f 6964 da03 696d 67da 0b6f 626a  int_id..img..obj
+00000390: 5f69 6e64 6963 6573 da03 6f62 6a63 0100  _indices..objc..
+000003a0: 0000 0000 0000 0000 0000 0100 0000 0300  ................
+000003b0: 0000 4300 0000 730e 0000 0074 00a0 017c  ..C...s....t...|
+000003c0: 006a 02a1 016a 0353 0029 014e 2904 da02  .j...j.S.).N)...
+000003d0: 6e70 da06 756e 6971 7565 720a 0000 00da  np..uniquer.....
+000003e0: 0473 697a 65a9 01da 0473 656c 66a9 0072  .size....self..r
+000003f0: 1400 0000 fa55 433a 5c55 7365 7273 5c4d  .....UC:\Users\M
+00000400: 6163 2050 7269 626c 655c 7265 706f 735c  ac Prible\repos\
+00000410: 7079 7879 3364 5c70 7978 7933 645c 6361  pyxy3d\pyxy3d\ca
+00000420: 6c69 6272 6174 696f 6e5c 6361 7074 7572  libration\captur
+00000430: 655f 766f 6c75 6d65 5c70 6f69 6e74 5f65  e_volume\point_e
+00000440: 7374 696d 6174 6573 2e70 79da 096e 5f63  stimates.py..n_c
+00000450: 616d 6572 6173 2700 0000 7302 0000 0000  ameras'...s.....
+00000460: 027a 1850 6f69 6e74 4573 7469 6d61 7465  .z.PointEstimate
+00000470: 732e 6e5f 6361 6d65 7261 7363 0100 0000  s.n_camerasc....
+00000480: 0000 0000 0000 0000 0100 0000 0200 0000  ................
+00000490: 4300 0000 730c 0000 007c 006a 006a 0164  C...s....|.j.j.d
+000004a0: 0119 0053 00a9 024e 7201 0000 0029 0272  ...S...Nr....).r
+000004b0: 0e00 0000 da05 7368 6170 6572 1200 0000  ......shaper....
+000004c0: 7214 0000 0072 1400 0000 7215 0000 00da  r....r....r.....
+000004d0: 0c6e 5f6f 626a 5f70 6f69 6e74 732b 0000  .n_obj_points+..
+000004e0: 0073 0200 0000 0002 7a1b 506f 696e 7445  .s......z.PointE
+000004f0: 7374 696d 6174 6573 2e6e 5f6f 626a 5f70  stimates.n_obj_p
+00000500: 6f69 6e74 7363 0100 0000 0000 0000 0000  ointsc..........
+00000510: 0000 0100 0000 0200 0000 4300 0000 730c  ..........C...s.
+00000520: 0000 007c 006a 006a 0164 0119 0053 0072  ...|.j.j.d...S.r
+00000530: 1700 0000 2902 720c 0000 0072 1800 0000  ....).r....r....
+00000540: 7212 0000 0072 1400 0000 7214 0000 0072  r....r....r....r
+00000550: 1500 0000 da0c 6e5f 696d 675f 706f 696e  ......n_img_poin
+00000560: 7473 2f00 0000 7302 0000 0000 027a 1b50  ts/...s......z.P
+00000570: 6f69 6e74 4573 7469 6d61 7465 732e 6e5f  ointEstimates.n_
+00000580: 696d 675f 706f 696e 7473 6301 0000 0000  img_pointsc.....
+00000590: 0000 0000 0000 0006 0000 0007 0000 0043  ...............C
+000005a0: 0000 0073 e200 0000 7c00 6a00 6a01 6401  ...s....|.j.j.d.
+000005b0: 1400 7d01 7c00 6a02 7403 1400 7c00 6a04  ..}.|.j.t...|.j.
+000005c0: 6402 1400 1700 7d02 7405 7c01 7c02 6602  d.....}.t.|.|.f.
+000005d0: 7406 6403 8d02 7d03 7407 a008 7c00 6a00  t.d...}.t...|.j.
+000005e0: 6a01 a101 7d04 7409 7403 8301 4400 5d3c  j...}.t.t...D.]<
+000005f0: 7d05 6404 7c03 6401 7c04 1400 7c00 6a00  }.d.|.d.|...|.j.
+00000600: 7403 1400 7c05 1700 6602 3c00 6404 7c03  t...|...f.<.d.|.
+00000610: 6401 7c04 1400 6404 1700 7c00 6a00 7403  d.|...d...|.j.t.
+00000620: 1400 7c05 1700 6602 3c00 7146 7409 6402  ..|...f.<.qFt.d.
+00000630: 8301 4400 5d50 7d05 6404 7c03 6401 7c04  ..D.]P}.d.|.d.|.
+00000640: 1400 7c00 6a02 7403 1400 7c00 6a0a 6402  ..|.j.t...|.j.d.
+00000650: 1400 1700 7c05 1700 6602 3c00 6404 7c03  ....|...f.<.d.|.
+00000660: 6401 7c04 1400 6404 1700 7c00 6a02 7403  d.|...d...|.j.t.
+00000670: 1400 7c00 6a0a 6402 1400 1700 7c05 1700  ..|.j.d.....|...
+00000680: 6602 3c00 718c 7c03 5300 2905 6124 0100  f.<.q.|.S.).a$..
+00000690: 0070 726f 7669 6465 2074 6865 2073 7061  .provide the spa
+000006a0: 7273 6974 7920 7374 7275 6374 7572 6520  rsity structure 
+000006b0: 666f 7220 7468 6520 4a61 636f 6269 616e  for the Jacobian
+000006c0: 2028 656c 656d 656e 7473 2074 6861 7420   (elements that 
+000006d0: 6172 6520 6e6f 7420 7a65 726f 290a 2020  are not zero).  
+000006e0: 2020 2020 2020 6e5f 706f 696e 7473 3a20        n_points: 
+000006f0: 6e75 6d62 6572 206f 6620 756e 6971 7565  number of unique
+00000700: 2033 6420 706f 696e 7473 3b20 7468 6573   3d points; thes
+00000710: 6520 7769 6c6c 2065 6163 6820 6861 7665  e will each have
+00000720: 2061 7420 6c65 6173 7420 6f6e 6520 6275   at least one bu
+00000730: 7420 706f 7465 6e74 6961 6c6c 7920 6d6f  t potentially mo
+00000740: 7265 2061 7373 6f63 6961 7465 6420 3264  re associated 2d
+00000750: 2070 6f69 6e74 730a 2020 2020 2020 2020   points.        
+00000760: 706f 696e 745f 696e 6469 6365 733a 2061  point_indices: a
+00000770: 2076 6563 746f 7220 7468 6174 206d 6170   vector that map
+00000780: 7320 7468 6520 3264 2070 6f69 6e74 7320  s the 2d points 
+00000790: 746f 2074 6865 6972 2061 7373 6f63 6961  to their associa
+000007a0: 7465 6420 3364 2070 6f69 6e74 0a20 2020  ted 3d point.   
+000007b0: 2020 2020 20e9 0200 0000 e903 0000 0029       ..........)
+000007c0: 01da 0564 7479 7065 e901 0000 0029 0b72  ...dtype.....).r
+000007d0: 0a00 0000 7211 0000 0072 1600 0000 da12  ....r....r......
+000007e0: 4341 4d45 5241 5f50 4152 414d 5f43 4f55  CAMERA_PARAM_COU
+000007f0: 4e54 7219 0000 0072 0300 0000 da03 696e  NTr....r......in
+00000800: 7472 0f00 0000 da06 6172 616e 6765 da05  tr......arange..
+00000810: 7261 6e67 6572 0d00 0000 2906 7213 0000  ranger....).r...
+00000820: 00da 016d da01 6eda 0141 da01 69da 0173  ...m..n..A..i..s
+00000830: 7214 0000 0072 1400 0000 7215 0000 00da  r....r....r.....
+00000840: 1467 6574 5f73 7061 7273 6974 795f 7061  .get_sparsity_pa
+00000850: 7474 6572 6e33 0000 0073 2000 0000 0006  ttern3...s .....
+00000860: 0c01 1401 1002 0e01 0c01 1a01 2002 0c01  ............ ...
+00000870: 2404 02fd 0201 0a01 16ff 02ff 0405 7a23  $.............z#
+00000880: 506f 696e 7445 7374 696d 6174 6573 2e67  PointEstimates.g
+00000890: 6574 5f73 7061 7273 6974 795f 7061 7474  et_sparsity_patt
+000008a0: 6572 6e63 0200 0000 0000 0000 0000 0000  ernc............
+000008b0: 0300 0000 0400 0000 4300 0000 7328 0000  ........C...s(..
+000008c0: 007c 017c 006a 0074 0114 0064 0185 0219  .|.|.j.t...d....
+000008d0: 007d 027c 02a0 0264 0264 03a1 027d 027c  .}.|...d.d...}.|
+000008e0: 027c 005f 0364 0153 0029 047a b70a 2020  .|._.d.S.).z..  
+000008f0: 2020 2020 2020 5072 6f76 6964 6564 2077        Provided w
+00000900: 6974 6820 7468 6520 6c65 6173 745f 7371  ith the least_sq
+00000910: 7561 7265 7320 6573 7469 6d61 7465 206f  uares estimate o
+00000920: 6620 7468 6520 6265 7374 2066 6974 206f  f the best fit o
+00000930: 6620 6d6f 6465 6c20 7061 7261 6d65 7465  f model paramete
+00000940: 7273 2028 696e 636c 7564 696e 6720 6361  rs (including ca
+00000950: 6d65 7261 2036 446f 4629 0a20 2020 2020  mera 6DoF).     
+00000960: 2020 2070 6172 7365 206f 7574 2074 6865     parse out the
+00000970: 2078 2c79 2c7a 206f 626a 6563 7420 706f   x,y,z object po
+00000980: 7369 7469 6f6e 7320 616e 6420 7570 6461  sitions and upda
+00000990: 7465 2073 656c 662e 6f62 6a0a 2020 2020  te self.obj.    
+000009a0: 2020 2020 4ee9 ffff ffff 721c 0000 0029      N.....r....)
+000009b0: 0472 1600 0000 721f 0000 00da 0772 6573  .r....r......res
+000009c0: 6861 7065 720e 0000 0029 0372 1300 0000  haper....).r....
+000009d0: da11 6c65 6173 745f 7371 5f72 6573 756c  ..least_sq_resul
+000009e0: 745f 785a 0378 797a 7214 0000 0072 1400  t_xZ.xyzr....r..
+000009f0: 0000 7215 0000 00da 0e75 7064 6174 655f  ..r......update_
+00000a00: 6f62 6a5f 7879 7a4b 0000 0073 0600 0000  obj_xyzK...s....
+00000a10: 0006 1201 0c02 7a1d 506f 696e 7445 7374  ......z.PointEst
+00000a20: 696d 6174 6573 2e75 7064 6174 655f 6f62  imates.update_ob
+00000a30: 6a5f 7879 7a4e 290d da08 5f5f 6e61 6d65  j_xyzN)...__name
+00000a40: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
+00000a50: 5f5f 7175 616c 6e61 6d65 5f5f da07 5f5f  __qualname__..__
+00000a60: 646f 635f 5f72 0f00 0000 da07 6e64 6172  doc__r......ndar
+00000a70: 7261 79da 0f5f 5f61 6e6e 6f74 6174 696f  ray..__annotatio
+00000a80: 6e73 5f5f da08 7072 6f70 6572 7479 7216  ns__..propertyr.
+00000a90: 0000 0072 1900 0000 721a 0000 0072 2800  ...r....r....r(.
+00000aa0: 0000 722c 0000 0072 1400 0000 7214 0000  ..r,...r....r...
+00000ab0: 0072 1400 0000 7215 0000 0072 0900 0000  .r....r....r....
+00000ac0: 1600 0000 731e 0000 000a 0204 060a 010a  ....s...........
+00000ad0: 010a 010a 010a 010a 0402 010a 0302 010a  ................
+00000ae0: 0302 010a 0308 1872 0900 0000 2902 da06  .......r....)...
+00000af0: 636f 6e66 6967 da06 7265 7475 726e 6301  config..returnc.
+00000b00: 0000 0000 0000 0000 0000 0005 0000 0004  ................
+00000b10: 0000 0043 0000 0073 3600 0000 7c00 6401  ...C...s6...|.d.
+00000b20: 1900 7d01 7c01 a000 a100 4400 5d16 5c02  ..}.|.....D.].\.
+00000b30: 7d02 7d03 7401 a002 7c03 a101 7c01 7c02  }.}.t...|...|.|.
+00000b40: 3c00 7110 7403 6600 7c01 8e01 7d04 7c04  <.q.t.f.|...}.|.
+00000b50: 5300 2902 4eda 0f70 6f69 6e74 5f65 7374  S.).N..point_est
+00000b60: 696d 6174 6573 2904 da05 6974 656d 7372  imates)...itemsr
+00000b70: 0f00 0000 da05 6172 7261 7972 0900 0000  ......arrayr....
+00000b80: 2905 7234 0000 00da 1470 6f69 6e74 5f65  ).r4.....point_e
+00000b90: 7374 696d 6174 6573 5f64 6963 74da 036b  stimates_dict..k
+00000ba0: 6579 da05 7661 6c75 6572 3600 0000 7214  ey..valuer6...r.
+00000bb0: 0000 0072 1400 0000 7215 0000 00da 146c  ...r....r......l
+00000bc0: 6f61 645f 706f 696e 745f 6573 7469 6d61  oad_point_estima
+00000bd0: 7465 7359 0000 0073 0a00 0000 0001 0802  tesY...s........
+00000be0: 1001 1002 0a01 723c 0000 00da 085f 5f6d  ......r<.....__m
+00000bf0: 6169 6e5f 5f29 01da 085f 5f72 6f6f 745f  ain__)...__root_
+00000c00: 5f29 01da 1367 6574 5f70 6f69 6e74 5f65  _)...get_point_e
+00000c10: 7374 696d 6174 6573 da05 7465 7374 735a  stimates..testsZ
+00000c20: 1334 5f63 616d 6572 6173 5f62 6567 696e  .4_cameras_begin
+00000c30: 6e69 6e67 7a0e 706f 696e 745f 6461 7461  ningz.point_data
+00000c40: 2e63 7376 7a0b 636f 6e66 6967 2e74 6f6d  .csvz.config.tom
+00000c50: 6c29 20da 0d70 7978 7933 642e 6c6f 6767  l) ..pyxy3d.logg
+00000c60: 6572 da06 7079 7879 3364 da06 6c6f 6767  er..pyxy3d..logg
+00000c70: 6572 da03 6765 7472 2d00 0000 da07 7061  er..getr-.....pa
+00000c80: 7468 6c69 6272 0200 0000 da0c 7363 6970  thlibr......scip
+00000c90: 792e 7370 6172 7365 7203 0000 00da 0670  y.sparser......p
+00000ca0: 616e 6461 73da 0270 64da 056e 756d 7079  andas..pd..numpy
+00000cb0: 720f 0000 00da 0b64 6174 6163 6c61 7373  r......dataclass
+00000cc0: 6573 7204 0000 00da 1b70 7978 7933 642e  esr......pyxy3d.
+00000cd0: 6361 6d65 7261 732e 6361 6d65 7261 5f61  cameras.camera_a
+00000ce0: 7272 6179 7205 0000 0072 0600 0000 5a4f  rrayr....r....ZO
+00000cf0: 7079 7879 3364 2e63 616c 6962 7261 7469  pyxy3d.calibrati
+00000d00: 6f6e 2e63 6170 7475 7265 5f76 6f6c 756d  on.capture_volum
+00000d10: 652e 6865 6c70 6572 5f66 756e 6374 696f  e.helper_functio
+00000d20: 6e73 2e67 6574 5f73 7465 7265 6f74 7269  ns.get_stereotri
+00000d30: 616e 6775 6c61 7465 645f 7461 626c 6572  angulated_tabler
+00000d40: 0700 0000 721f 0000 0072 0900 0000 da04  ....r....r......
+00000d50: 6469 6374 723c 0000 0072 3e00 0000 5a46  dictr<...r>...ZF
+00000d60: 7079 7879 3364 2e63 616c 6962 7261 7469  pyxy3d.calibrati
+00000d70: 6f6e 2e63 6170 7475 7265 5f76 6f6c 756d  on.capture_volum
+00000d80: 652e 6865 6c70 6572 5f66 756e 6374 696f  e.helper_functio
+00000d90: 6e73 2e67 6574 5f70 6f69 6e74 5f65 7374  ns.get_point_est
+00000da0: 696d 6174 6573 723f 0000 00da 1173 6573  imatesr?.....ses
+00000db0: 7369 6f6e 5f64 6972 6563 746f 7279 5a0f  sion_directoryZ.
+00000dc0: 706f 696e 745f 6461 7461 5f70 6174 685a  point_data_pathZ
+00000dd0: 1243 616d 6572 6141 7272 6179 4275 696c  .CameraArrayBuil
+00000de0: 6465 72da 0c63 616d 6572 615f 6172 7261  der..camera_arra
+00000df0: 7972 3600 0000 7214 0000 0072 1400 0000  yr6...r....r....
+00000e00: 7214 0000 0072 1500 0000 da08 3c6d 6f64  r....r......<mod
+00000e10: 756c 653e 0600 0000 7326 0000 0008 010c  ule>....s&......
+00000e20: 020c 020c 0208 0108 010c 0110 010c 0204  ................
+00000e30: 0302 0110 4210 0c08 020c 010c 010c 010a  ....B...........
+00000e40: 0212 02                                  ...
```

### Comparing `pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/__pycache__/quality_controller.cpython-310.pyc` & `pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/__pycache__/quality_controller.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/__pycache__/quality_controller.cpython-38.pyc` & `pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/__pycache__/quality_controller.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/__pycache__/set_origin_functions.cpython-310.pyc` & `pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/__pycache__/set_origin_functions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/__pycache__/set_origin_functions.cpython-38.pyc` & `pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/__pycache__/set_origin_functions.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/capture_volume.py` & `pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/capture_volume.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/capture_volume_stage_1.pkl` & `pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/capture_volume_stage_1.pkl`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_point_estimates.cpython-310.pyc` & `pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_point_estimates.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_point_estimates.cpython-38.pyc` & `pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_point_estimates.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_stereotriangulated_table.cpython-310.pyc` & `pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_stereotriangulated_table.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_stereotriangulated_table.cpython-38.pyc` & `pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_stereotriangulated_table.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/helper_functions/get_point_estimates.py` & `pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/helper_functions/get_point_estimates.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/helper_functions/get_stereotriangulated_table.py` & `pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/helper_functions/get_stereotriangulated_table.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/point_estimates.py` & `pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/point_estimates.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,15 +29,23 @@
     sync_indices: np.ndarray  # the sync_index from when the image was taken
     camera_indices: np.ndarray  # camera id associated with the img point
     point_id: np.ndarray # point id (i.e. charuco corner currently)
     img: np.ndarray  # x,y coords of point
     obj_indices: np.ndarray # mapping of x,y img points to their respective list of estimated x,y,z obj points
     obj: np.ndarray  # x,y,z estimates of object points
     # obj_corner_id: np.ndarray # the charuco corner ID of the xyz object point; is this necessary?
-    
+
+
+    def __post_init__(self):
+        self.sync_indices = self.sync_indices.astype(np.int32)
+        self.camera_indices = self.camera_indices.astype(np.int16)
+        self.point_id = self.point_id.astype(np.uint16)
+        self.img = self.img.astype(np.float64)
+        self.obj_indices = self.obj_indices.astype(np.int32)
+        self.obj = self.obj.astype(np.float64)    
 
     @property
     def n_cameras(self):
         return np.unique(self.camera_indices).size
 
     @property
     def n_obj_points(self):
```

### Comparing `pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/quality_controller.py` & `pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/quality_controller.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/seaborn_summaries.py` & `pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/seaborn_summaries.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/set_origin_functions.py` & `pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/set_origin_functions.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/calibration/charuco.py` & `pyxy3d-0.1.4/pyxy3d/calibration/charuco.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/calibration/draw_charuco.py` & `pyxy3d-0.1.4/pyxy3d/calibration/draw_charuco.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/calibration/monocalibrator.py` & `pyxy3d-0.1.4/pyxy3d/calibration/monocalibrator.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/calibration/stereocalibrator.py` & `pyxy3d-0.1.4/pyxy3d/calibration/stereocalibrator.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/cameras/__pycache__/camera.cpython-310.pyc` & `pyxy3d-0.1.4/pyxy3d/cameras/__pycache__/camera.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/cameras/__pycache__/camera.cpython-38.pyc` & `pyxy3d-0.1.4/pyxy3d/cameras/__pycache__/camera.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/cameras/__pycache__/camera_array.cpython-310.pyc` & `pyxy3d-0.1.4/pyxy3d/cameras/__pycache__/camera_array.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/cameras/__pycache__/camera_array.cpython-38.pyc` & `pyxy3d-0.1.4/pyxy3d/cameras/__pycache__/camera_array.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/cameras/__pycache__/camera_array_initializer.cpython-310.pyc` & `pyxy3d-0.1.4/pyxy3d/cameras/__pycache__/camera_array_initializer.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/cameras/__pycache__/camera_array_initializer.cpython-38.pyc` & `pyxy3d-0.1.4/pyxy3d/cameras/__pycache__/camera_array_initializer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/cameras/__pycache__/data_packets.cpython-310.pyc` & `pyxy3d-0.1.4/pyxy3d/cameras/__pycache__/data_packets.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/cameras/__pycache__/data_packets.cpython-38.pyc` & `pyxy3d-0.1.4/pyxy3d/cameras/__pycache__/data_packets.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/cameras/__pycache__/live_stream.cpython-310.pyc` & `pyxy3d-0.1.4/pyxy3d/cameras/__pycache__/live_stream.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/cameras/__pycache__/live_stream.cpython-38.pyc` & `pyxy3d-0.1.4/pyxy3d/cameras/__pycache__/live_stream.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/cameras/__pycache__/synchronizer.cpython-310.pyc` & `pyxy3d-0.1.4/pyxy3d/cameras/__pycache__/synchronizer.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jun 15 18:45:15 2023 UTC, .py size: 13543 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3b5c 8b64 e734 0000  o.......;\.d.4..
+00000000: 6f0d 0d0a 0000 0000 34df 9564 e734 0000  o.......4..d.4..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 7e00 0000 6400  .....@...s~...d.
 00000030: 6401 6c00 5a01 6501 6a02 a003 6504 a101  d.l.Z.e.j...e...
 00000040: 5a02 6400 6401 6c05 5a05 6400 6401 6c06  Z.d.d.l.Z.d.d.l.
 00000050: 5a06 6400 6402 6c07 6d08 5a08 0100 6400  Z.d.d.l.m.Z...d.
 00000060: 6403 6c09 6d0a 5a0a 0100 6400 6404 6c0b  d.l.m.Z...d.d.l.
 00000070: 6d0c 5a0c 6d0d 5a0d 0100 6400 6401 6c0e  m.Z.m.Z...d.d.l.
@@ -573,47 +573,47 @@
 000023c0: 6c69 6573 745f 6e65 7874 5a0e 6c61 7465  liest_nextZ.late
 000023d0: 7374 5f63 7572 7265 6e74 720f 0000 005a  st_currentr....Z
 000023e0: 1363 7572 7265 6e74 5f66 7261 6d65 5f69  .current_frame_i
 000023f0: 6e64 6578 5a0e 706f 7274 5f69 6e64 6578  ndexZ.port_index
 00002400: 5f6b 6579 5a14 6375 7272 656e 745f 6672  _keyZ.current_fr
 00002410: 616d 655f 7061 636b 6574 725d 0000 0072  ame_packetr]...r
 00002420: 2700 0000 720c 0000 0072 0c00 0000 7210  '...r....r....r.
-00002430: 0000 0072 4d00 0000 e200 0000 7378 0000  ...rM.......sx..
+00002430: 0000 0072 4d00 0000 e200 0000 7376 0000  ...rM.......sv..
 00002440: 000a 0204 020a 020c 0104 0204 0204 0404  ................
 00002450: 010a 020e 010e 010c 010a 020a 010e 020a  ................
-00002460: 0106 010c 0308 0214 0116 0202 ff08 0504  ................
-00002470: 010a 0106 ff06 0502 0108 ff12 040a 0104  ................
-00002480: 0114 0106 ff16 0412 020c 0208 0208 020a  ................
-00002490: 020a 0106 010a 0410 010c 010a 020c 010c  ................
-000024a0: 0116 0114 0112 0314 0102 800a 0212 011e  ................
-000024b0: 0102 ff0a 030a ad0e 557a 2053 796e 6368  ........Uz Synch
-000024c0: 726f 6e69 7a65 722e 7379 6e63 685f 6672  ronizer.synch_fr
-000024d0: 616d 6573 5f77 6f72 6b65 724e 2901 7209  ames_workerN).r.
-000024e0: 0000 0029 1ada 085f 5f6e 616d 655f 5fda  ...)...__name__.
-000024f0: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
-00002500: 7561 6c6e 616d 655f 5fda 0464 6963 7472  ualname__..dictr
-00002510: 2800 0000 da04 626f 6f6c 722c 0000 0072  (.....boolr,...r
-00002520: 3000 0000 da08 7072 6f70 6572 7479 7234  0.....propertyr4
-00002530: 0000 0072 1e00 0000 721d 0000 0072 3d00  ...r....r....r=.
-00002540: 0000 7243 0000 0072 2200 0000 7223 0000  ..rC...r"...r#..
-00002550: 0072 5000 0000 7253 0000 0072 5400 0000  .rP...rS...rT...
-00002560: 7256 0000 0072 4c00 0000 7267 0000 0072  rV...rL...rg...r
-00002570: 6a00 0000 726c 0000 0072 6f00 0000 724d  j...rl...ro...rM
-00002580: 0000 0072 0c00 0000 720c 0000 0072 0c00  ...r....r....r..
-00002590: 0000 7210 0000 0072 0800 0000 1300 0000  ..r....r........
-000025a0: 732c 0000 0008 0010 010e 2208 0402 070a  s,........".....
-000025b0: 0108 0708 0608 0608 0608 0608 0608 0e08  ................
-000025c0: 0708 0808 0408 0408 1408 2408 0c08 090c  ..........$.....
-000025d0: 0972 0800 0000 2915 da0d 7079 7879 3364  .r....)...pyxy3d
-000025e0: 2e6c 6f67 6765 72da 0670 7978 7933 6472  .logger..pyxy3dr
-000025f0: 3500 0000 725a 0000 0072 7600 0000 da07  5...rZ...rv.....
-00002600: 6c6f 6767 696e 6772 6100 0000 da07 7061  loggingra.....pa
-00002610: 7468 6c69 6272 0200 0000 da05 7175 6575  thlibr......queu
-00002620: 6572 0300 0000 da09 7468 7265 6164 696e  er......threadin
-00002630: 6772 0400 0000 7205 0000 00da 0363 7632  gr....r......cv2
-00002640: da05 6e75 6d70 7972 3100 0000 da10 7079  ..numpyr1.....py
-00002650: 7879 3364 2e69 6e74 6572 6661 6365 7206  xy3d.interfacer.
-00002660: 0000 0072 2f00 0000 7208 0000 0072 0c00  ...r/...r....r..
-00002670: 0000 720c 0000 0072 0c00 0000 7210 0000  ..r....r....r...
-00002680: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
-00002690: 1800 0000 0800 0c02 0801 0804 0c01 0c01  ................
-000026a0: 1001 0802 0801 0c01 0402 1202            ............
+00002460: 0106 010c 0308 0214 0118 0208 0404 010a  ................
+00002470: 0106 ff06 0502 0108 ff12 040a 0104 0114  ................
+00002480: 0106 ff16 0412 020c 0208 0208 020a 020a  ................
+00002490: 0106 010a 0410 010c 010a 020c 010c 0116  ................
+000024a0: 0114 0112 0314 0102 800a 0212 011e 0102  ................
+000024b0: ff0a 030a ad0e 557a 2053 796e 6368 726f  ......Uz Synchro
+000024c0: 6e69 7a65 722e 7379 6e63 685f 6672 616d  nizer.synch_fram
+000024d0: 6573 5f77 6f72 6b65 724e 2901 7209 0000  es_workerN).r...
+000024e0: 0029 1ada 085f 5f6e 616d 655f 5fda 0a5f  .)...__name__.._
+000024f0: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
+00002500: 6c6e 616d 655f 5fda 0464 6963 7472 2800  lname__..dictr(.
+00002510: 0000 da04 626f 6f6c 722c 0000 0072 3000  ....boolr,...r0.
+00002520: 0000 da08 7072 6f70 6572 7479 7234 0000  ....propertyr4..
+00002530: 0072 1e00 0000 721d 0000 0072 3d00 0000  .r....r....r=...
+00002540: 7243 0000 0072 2200 0000 7223 0000 0072  rC...r"...r#...r
+00002550: 5000 0000 7253 0000 0072 5400 0000 7256  P...rS...rT...rV
+00002560: 0000 0072 4c00 0000 7267 0000 0072 6a00  ...rL...rg...rj.
+00002570: 0000 726c 0000 0072 6f00 0000 724d 0000  ..rl...ro...rM..
+00002580: 0072 0c00 0000 720c 0000 0072 0c00 0000  .r....r....r....
+00002590: 7210 0000 0072 0800 0000 1300 0000 732c  r....r........s,
+000025a0: 0000 0008 0010 010e 2208 0402 070a 0108  ........".......
+000025b0: 0708 0608 0608 0608 0608 0608 0e08 0708  ................
+000025c0: 0808 0408 0408 1408 2408 0c08 090c 0972  ........$......r
+000025d0: 0800 0000 2915 da0d 7079 7879 3364 2e6c  ....)...pyxy3d.l
+000025e0: 6f67 6765 72da 0670 7978 7933 6472 3500  ogger..pyxy3dr5.
+000025f0: 0000 725a 0000 0072 7600 0000 da07 6c6f  ..rZ...rv.....lo
+00002600: 6767 696e 6772 6100 0000 da07 7061 7468  ggingra.....path
+00002610: 6c69 6272 0200 0000 da05 7175 6575 6572  libr......queuer
+00002620: 0300 0000 da09 7468 7265 6164 696e 6772  ......threadingr
+00002630: 0400 0000 7205 0000 00da 0363 7632 da05  ....r......cv2..
+00002640: 6e75 6d70 7972 3100 0000 da10 7079 7879  numpyr1.....pyxy
+00002650: 3364 2e69 6e74 6572 6661 6365 7206 0000  3d.interfacer...
+00002660: 0072 2f00 0000 7208 0000 0072 0c00 0000  .r/...r....r....
+00002670: 720c 0000 0072 0c00 0000 7210 0000 00da  r....r....r.....
+00002680: 083c 6d6f 6475 6c65 3e01 0000 0073 1800  .<module>....s..
+00002690: 0000 0800 0c02 0801 0804 0c01 0c01 1001  ................
+000026a0: 0802 0801 0c01 0402 1202                 ..........
```

### Comparing `pyxy3d-0.1.3/pyxy3d/cameras/__pycache__/synchronizer.cpython-38.pyc` & `pyxy3d-0.1.4/pyxy3d/cameras/__pycache__/synchronizer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/cameras/camera.py` & `pyxy3d-0.1.4/pyxy3d/cameras/camera.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/cameras/camera_array.py` & `pyxy3d-0.1.4/pyxy3d/cameras/camera_array.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/cameras/camera_array_initializer.py` & `pyxy3d-0.1.4/pyxy3d/cameras/camera_array_initializer.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/cameras/live_stream.py` & `pyxy3d-0.1.4/pyxy3d/cameras/live_stream.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/cameras/synchronizer.py` & `pyxy3d-0.1.4/pyxy3d/cameras/synchronizer.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/configurator.py` & `pyxy3d-0.1.4/pyxy3d/configurator.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/export.py` & `pyxy3d-0.1.4/pyxy3d/export.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/__pycache__/calibrate_capture_volume_widget.cpython-310.pyc` & `pyxy3d-0.1.4/pyxy3d/gui/__pycache__/calibrate_capture_volume_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/__pycache__/calibration_widget.cpython-310.pyc` & `pyxy3d-0.1.4/pyxy3d/gui/__pycache__/calibration_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/__pycache__/calibration_wizard.cpython-310.pyc` & `pyxy3d-0.1.4/pyxy3d/gui/__pycache__/calibration_wizard.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/__pycache__/charuco_widget.cpython-310.pyc` & `pyxy3d-0.1.4/pyxy3d/gui/__pycache__/charuco_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/__pycache__/extrinsic_calibration_widget.cpython-310.pyc` & `pyxy3d-0.1.4/pyxy3d/gui/__pycache__/extrinsic_calibration_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/__pycache__/log_widget.cpython-310.pyc` & `pyxy3d-0.1.4/pyxy3d/gui/__pycache__/log_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/__pycache__/main.cpython-310.pyc` & `pyxy3d-0.1.4/pyxy3d/gui/__pycache__/main.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/__pycache__/main.cpython-38.pyc` & `pyxy3d-0.1.4/pyxy3d/gui/__pycache__/main.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/__pycache__/main_widget.cpython-310.pyc` & `pyxy3d-0.1.4/pyxy3d/gui/__pycache__/main_widget.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jun 15 18:45:15 2023 UTC, .py size: 16047 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-00000000: 6f0d 0d0a 0000 0000 3b5c 8b64 af3e 0000  o.......;\.d.>..
+00000000: 6f0d 0d0a 0000 0000 17e7 9564 963e 0000  o..........d.>..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 9201 0000 6400  .....@...s....d.
+00000020: 0004 0000 0040 0000 0073 8601 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c00 5a01 6501  d.l.Z.d.d.l.Z.e.
 00000040: 6a02 a003 6504 a101 5a02 6400 6402 6c05  j...e...Z.d.d.l.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 0100 6501  m.Z.m.Z.m.Z...e.
 00000060: 6a02 a003 6504 a101 5a02 6400 6403 6c09  j...e...Z.d.d.l.
 00000070: 6d0a 5a0a 0100 6400 6404 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
 00000080: 0100 6400 6401 6c0d 5a0d 6400 6405 6c05  ..d.d.l.Z.d.d.l.
 00000090: 6d0e 5a0e 6d06 5a06 6d07 5a07 6d0f 5a0f  m.Z.m.Z.m.Z.m.Z.
@@ -16,717 +16,714 @@
 000000f0: 6409 6c01 6d1f 5a1f 6d20 5a20 6d21 5a21  d.l.m.Z.m Z m!Z!
 00000100: 0100 6400 640a 6c22 6d23 5a23 6d24 5a24  ..d.d.l"m#Z#m$Z$
 00000110: 0100 6400 640b 6c25 6d26 5a26 0100 6400  ..d.d.l%m&Z&..d.
 00000120: 640c 6c27 6d28 5a28 0100 6400 640d 6c29  d.l'm(Z(..d.d.l)
 00000130: 6d2a 5a2a 0100 6400 640e 6c2b 6d2c 5a2c  m*Z*..d.d.l+m,Z,
 00000140: 0100 6400 640f 6c2d 6d2e 5a2e 0100 6400  ..d.d.l-m.Z...d.
 00000150: 6410 6c2f 6d30 5a30 0100 6400 6411 6c31  d.l/m0Z0..d.d.l1
-00000160: 6d32 5a32 0100 6400 6412 6c33 6d34 5a34  m2Z2..d.d.l3m4Z4
-00000170: 0100 4700 6413 6414 8400 6414 6517 8303  ..G.d.d...d.e...
-00000180: 5a35 4700 6415 6416 8400 6416 6506 8303  Z5G.d.d...d.e...
-00000190: 5a36 4700 6417 6418 8400 6418 6514 8303  Z6G.d.d...d.e...
-000001a0: 5a37 6419 641a 8400 5a38 6504 641b 6b02  Z7d.d...Z8e.d.k.
-000001b0: 72c7 6538 8300 0100 6401 5300 6401 5300  r.e8....d.S.d.S.
-000001c0: 291c e900 0000 004e 2903 da0b 514d 6169  )......N)...QMai
-000001d0: 6e57 696e 646f 77da 0e51 5374 6163 6b65  nWindow..QStacke
-000001e0: 644c 6179 6f75 74da 0b51 4669 6c65 4469  dLayout..QFileDi
-000001f0: 616c 6f67 2901 da04 5061 7468 2901 da06  alog)...Path)...
-00000200: 5468 7265 6164 2909 da0c 5141 7070 6c69  Thread)...QAppli
-00000210: 6361 7469 6f6e 7202 0000 0072 0300 0000  cationr....r....
-00000220: da07 5157 6964 6765 74da 0b51 446f 636b  ..QWidget..QDock
-00000230: 5769 6467 6574 da0b 5156 426f 784c 6179  Widget..QVBoxLay
-00000240: 6f75 74da 0551 4d65 6e75 da08 514d 656e  out..QMenu..QMen
-00000250: 7542 6172 da0a 5154 6162 5769 6467 6574  uBar..QTabWidget
-00000260: 2901 da04 456e 756d 2904 da05 5149 636f  )...Enum)...QIco
-00000270: 6eda 0751 4163 7469 6f6e da0c 514b 6579  n..QAction..QKey
-00000280: 5365 7175 656e 6365 da09 5153 686f 7274  Sequence..QShort
-00000290: 6375 7429 01da 0251 7429 03da 085f 5f72  cut)...Qt)...__r
-000002a0: 6f6f 745f 5fda 115f 5f73 6574 7469 6e67  oot__..__setting
-000002b0: 735f 7061 7468 5f5f da0c 5f5f 7573 6572  s_path__..__user
-000002c0: 5f64 6972 5f5f 2902 da07 5365 7373 696f  _dir__)...Sessio
-000002d0: 6eda 0b53 6573 7369 6f6e 4d6f 6465 2901  n..SessionMode).
-000002e0: da09 4c6f 6757 6964 6765 7429 01da 0c43  ..LogWidget)...C
-000002f0: 6f6e 6669 6775 7261 746f 7229 01da 1143  onfigurator)...C
-00000300: 616c 6962 7261 7469 6f6e 5769 6467 6574  alibrationWidget
-00000310: 2901 da0d 4368 6172 7563 6f57 6964 6765  )...CharucoWidge
-00000320: 7429 01da 1a49 6e74 7269 6e73 6963 4361  t)...IntrinsicCa
-00000330: 6c69 6272 6174 696f 6e57 6964 6765 7429  librationWidget)
-00000340: 01da 1c43 616c 6962 7261 7465 4361 7074  ...CalibrateCapt
-00000350: 7572 6556 6f6c 756d 6557 6964 6765 7429  ureVolumeWidget)
-00000360: 01da 0f52 6563 6f72 6469 6e67 5769 6467  ...RecordingWidg
-00000370: 6574 2901 da14 506f 7374 5072 6f63 6573  et)...PostProces
-00000380: 7369 6e67 5769 6467 6574 6300 0000 0000  singWidgetc.....
-00000390: 0000 0000 0000 0000 0000 0001 0000 0040  ...............@
-000003a0: 0000 0073 2000 0000 6500 5a01 6400 5a02  ...s ...e.Z.d.Z.
-000003b0: 6401 5a03 6402 5a04 6403 5a05 6404 5a06  d.Z.d.Z.d.Z.d.Z.
-000003c0: 6405 5a07 6406 5300 2907 da08 5461 6249  d.Z.d.S.)...TabI
-000003d0: 6e64 6578 7201 0000 00e9 0100 0000 e902  ndexr...........
-000003e0: 0000 00e9 0300 0000 e904 0000 004e 2908  .............N).
-000003f0: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
-00000400: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
-00000410: 6d65 5f5f da07 4368 6172 7563 6fda 0743  me__..Charuco..C
-00000420: 616d 6572 6173 da0d 4361 7074 7572 6556  ameras..CaptureV
-00000430: 6f6c 756d 65da 0952 6563 6f72 6469 6e67  olume..Recording
-00000440: da0a 5072 6f63 6573 7369 6e67 a900 722e  ..Processing..r.
-00000450: 0000 0072 2e00 0000 fa3a 433a 5c55 7365  ...r.....:C:\Use
-00000460: 7273 5c4d 6163 2050 7269 626c 655c 7265  rs\Mac Prible\re
-00000470: 706f 735c 7079 7879 3364 5c70 7978 7933  pos\pyxy3d\pyxy3
-00000480: 645c 6775 695c 6d61 696e 5f77 6964 6765  d\gui\main_widge
-00000490: 742e 7079 7221 0000 0029 0000 0073 0c00  t.pyr!...)...s..
-000004a0: 0000 0800 0401 0401 0401 0401 0801 7221  ..............r!
-000004b0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-000004c0: 0000 0000 0300 0000 0000 0000 73b0 0000  ............s...
-000004d0: 0065 005a 0164 005a 0287 0066 0164 0164  .e.Z.d.Z...f.d.d
-000004e0: 0284 085a 0364 0364 0484 005a 0464 0564  ...Z.d.d...Z.d.d
-000004f0: 0684 005a 0564 0764 0884 005a 0664 0964  ...Z.d.d...Z.d.d
-00000500: 0a84 005a 0764 0b64 0c84 005a 0864 0d65  ...Z.d.d...Z.d.e
-00000510: 0966 0264 0e64 0f84 045a 0a64 1064 1184  .f.d.d...Z.d.d..
-00000520: 005a 0b64 1264 1384 005a 0c64 1464 1584  .Z.d.d...Z.d.d..
-00000530: 005a 0d64 1664 1784 005a 0e64 1864 1984  .Z.d.d...Z.d.d..
-00000540: 005a 0f64 1a64 1b84 005a 1064 1c65 0966  .Z.d.d...Z.d.e.f
-00000550: 0264 1d64 1e84 045a 1164 1f64 2084 005a  .d.d...Z.d.d ..Z
-00000560: 1264 2164 2284 005a 1364 2364 2484 005a  .d!d"..Z.d#d$..Z
-00000570: 1464 2564 2684 005a 1587 0004 005a 1653  .d%d&..Z.....Z.S
-00000580: 0029 27da 0a4d 6169 6e57 696e 646f 7763  .)'..MainWindowc
-00000590: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-000005a0: 0700 0000 0300 0000 73aa 0100 0074 0074  ........s....t.t
-000005b0: 017c 0083 02a0 02a1 0001 0074 03a0 0474  .|.........t...t
-000005c0: 05a1 017c 005f 067c 00a0 0764 01a1 0101  ...|._.|...d....
-000005d0: 007c 00a0 0874 0974 0a74 0b74 0c64 0283  .|...t.t.t.t.d..
-000005e0: 0283 0183 01a1 0101 007c 00a0 0d64 0364  .........|...d.d
-000005f0: 03a1 0201 007c 00a0 0ea1 007c 005f 0f7c  .....|.....|._.|
-00000600: 006a 0fa0 1064 04a1 017c 005f 1174 1264  .j...d...|._.t.d
-00000610: 057c 0083 027c 005f 137c 006a 136a 14a0  .|...|._.|.j.j..
-00000620: 157c 006a 16a1 0101 007c 006a 11a0 177c  .|.j.....|.j...|
-00000630: 006a 13a1 0101 0074 1864 067c 0083 027c  .j.....t.d.|...|
-00000640: 005f 1974 1a7c 006a 0664 0719 0083 0144  ._.t.|.j.d.....D
-00000650: 005d 077d 017c 00a0 1b7c 01a1 0101 0071  .].}.|...|.....q
-00000660: 527c 006a 11a0 107c 006a 19a1 0101 0074  R|.j...|.j.....t
-00000670: 1264 087c 0083 027c 005f 1c7c 006a 11a0  .d.|...|._.|.j..
-00000680: 177c 006a 1ca1 0101 007c 006a 0fa0 1064  .|.j.....|.j...d
-00000690: 09a1 017c 005f 1d74 1264 0a7c 0083 027c  ...|._.t.d.|...|
-000006a0: 005f 1e7c 006a 1da0 177c 006a 1ea1 0101  ._.|.j...|.j....
-000006b0: 007c 006a 1ea0 1f64 0ba1 0101 0074 1264  .|.j...d.....t.d
-000006c0: 0c7c 0083 027c 005f 207c 006a 1da0 177c  .|...|._ |.j...|
-000006d0: 006a 20a1 0101 007c 006a 20a0 1f64 0ba1  .j ....|.j ..d..
-000006e0: 0101 007c 00a0 21a1 0001 0074 2283 007c  ...|..!....t"..|
-000006f0: 005f 237c 00a0 247c 006a 23a1 0101 0074  ._#|..$|.j#....t
-00000700: 2564 0d7c 0083 027c 005f 267c 006a 26a0  %d.|...|._&|.j&.
-00000710: 2774 256a 286a 29a1 0101 007c 006a 26a0  't%j(j)....|.j&.
-00000720: 2a74 2b6a 2c6a 2da1 0101 0074 2e83 007c  *t+j,j-....t...|
-00000730: 005f 2f7c 006a 26a0 307c 006a 2fa1 0101  ._/|.j&.0|.j/...
-00000740: 007c 00a0 3174 2b6a 2c6a 2d7c 006a 26a1  .|..1t+j,j-|.j&.
-00000750: 0201 0064 0053 0029 0e4e 5a06 5079 7879  ...d.S.).NZ.Pyxy
-00000760: 3344 7a1e 7079 7879 3364 2f67 7569 2f69  3Dz.pyxy3d/gui/i
-00000770: 636f 6e73 2f70 7978 795f 6c6f 676f 2e73  cons/pyxy_logo.s
-00000780: 7667 69f4 0100 00da 0446 696c 657a 104e  vgi......Filez.N
-00000790: 6577 2f4f 7065 6e20 5072 6f6a 6563 747a  ew/Open Projectz
-000007a0: 1252 6563 656e 7420 5072 6f6a 6563 7473  .Recent Projects
-000007b0: 2e2e 2eda 0f72 6563 656e 745f 7072 6f6a  .....recent_proj
-000007c0: 6563 7473 5a04 4578 6974 722a 0000 007a  ectsZ.Exitr*...z
-000007d0: 0f43 6f6e 6e65 6374 2043 616d 6572 6173  .Connect Cameras
-000007e0: 467a 1244 6973 636f 6e6e 6563 7420 4361  Fz.Disconnect Ca
-000007f0: 6d65 7261 735a 034c 6f67 2932 da05 7375  merasZ.Log)2..su
-00000800: 7065 7272 3000 0000 da08 5f5f 696e 6974  perr0.....__init
-00000810: 5f5f da04 746f 6d6c da04 6c6f 6164 7215  __..toml..loadr.
-00000820: 0000 00da 0c61 7070 5f73 6574 7469 6e67  .....app_setting
-00000830: 73da 0e73 6574 5769 6e64 6f77 5469 746c  s..setWindowTitl
-00000840: 65da 0d73 6574 5769 6e64 6f77 4963 6f6e  e..setWindowIcon
-00000850: 720f 0000 00da 0373 7472 7205 0000 0072  r......strr....r
-00000860: 1400 0000 da0e 7365 744d 696e 696d 756d  ......setMinimum
-00000870: 5369 7a65 5a07 6d65 6e75 4261 72da 046d  SizeZ.menuBar..m
-00000880: 656e 75da 0761 6464 4d65 6e75 5a09 6669  enu..addMenuZ.fi
-00000890: 6c65 5f6d 656e 7572 1000 0000 5a13 6f70  le_menur....Z.op
-000008a0: 656e 5f70 726f 6a65 6374 5f61 6374 696f  en_project_actio
-000008b0: 6eda 0974 7269 6767 6572 6564 da07 636f  n..triggered..co
-000008c0: 6e6e 6563 74da 1963 7265 6174 655f 6e65  nnect..create_ne
-000008d0: 775f 7072 6f6a 6563 745f 666f 6c64 6572  w_project_folder
-000008e0: da09 6164 6441 6374 696f 6e72 0b00 0000  ..addActionr....
-000008f0: da1b 6f70 656e 5f72 6563 656e 745f 7072  ..open_recent_pr
-00000900: 6f6a 6563 745f 7375 626d 656e 75da 0872  oject_submenu..r
-00000910: 6576 6572 7365 64da 1561 6464 5f74 6f5f  eversed..add_to_
-00000920: 7265 6365 6e74 5f70 726f 6a65 6374 da12  recent_project..
-00000930: 6578 6974 5f70 7978 7933 645f 6163 7469  exit_pyxy3d_acti
-00000940: 6f6e 5a0c 6361 6d65 7261 735f 6d65 6e75  onZ.cameras_menu
-00000950: da16 636f 6e6e 6563 745f 6361 6d65 7261  ..connect_camera
-00000960: 735f 6163 7469 6f6e da0a 7365 7445 6e61  s_action..setEna
-00000970: 626c 6564 da19 6469 7363 6f6e 6e65 6374  bled..disconnect
-00000980: 5f63 616d 6572 6173 5f61 6374 696f 6eda  _cameras_action.
-00000990: 1463 6f6e 6e65 6374 5f6d 656e 755f 6163  .connect_menu_ac
-000009a0: 7469 6f6e 7372 0d00 0000 da0a 7461 625f  tionsr......tab_
-000009b0: 7769 6467 6574 da10 7365 7443 656e 7472  widget..setCentr
-000009c0: 616c 5769 6467 6574 7209 0000 005a 0d64  alWidgetr....Z.d
-000009d0: 6f63 6b65 645f 6c6f 6767 6572 5a0b 7365  ocked_loggerZ.se
-000009e0: 7446 6561 7475 7265 735a 1144 6f63 6b57  tFeaturesZ.DockW
-000009f0: 6964 6765 7446 6561 7475 7265 5a11 446f  idgetFeatureZ.Do
-00000a00: 636b 5769 6467 6574 4d6f 7661 626c 655a  ckWidgetMovableZ
-00000a10: 0f73 6574 416c 6c6f 7765 6441 7265 6173  .setAllowedAreas
-00000a20: 7213 0000 00da 0e44 6f63 6b57 6964 6765  r......DockWidge
-00000a30: 7441 7265 61da 1442 6f74 746f 6d44 6f63  tArea..BottomDoc
-00000a40: 6b57 6964 6765 7441 7265 6172 1900 0000  kWidgetArear....
-00000a50: 5a0a 6c6f 675f 7769 6467 6574 da09 7365  Z.log_widget..se
-00000a60: 7457 6964 6765 74da 0d61 6464 446f 636b  tWidget..addDock
-00000a70: 5769 6467 6574 2902 da04 7365 6c66 da0c  Widget)...self..
-00000a80: 7072 6f6a 6563 745f 7061 7468 a901 da09  project_path....
-00000a90: 5f5f 636c 6173 735f 5f72 2e00 0000 722f  __class__r....r/
-00000aa0: 0000 0072 3400 0000 3200 0000 7340 0000  ...r4...2...s@..
-00000ab0: 000e 010c 020a 0218 010c 010a 030e 010c  ................
-00000ac0: 0310 010e 010c 0312 030c 010e 020c 020e  ................
-00000ad0: 010e 020c 010e 010c 010c 020e 010c 0108  ................
-00000ae0: 0208 030c 020c 0310 0110 0108 010e 0116  ................
-00000af0: 027a 134d 6169 6e57 696e 646f 772e 5f5f  .z.MainWindow.__
-00000b00: 696e 6974 5f5f 6301 0000 0000 0000 0000  init__c.........
-00000b10: 0000 0001 0000 0004 0000 0043 0000 0073  ...........C...s
-00000b20: 3800 0000 7c00 6a00 6a01 a002 7c00 6a03  8...|.j.j...|.j.
-00000b30: a101 0100 7c00 6a04 6a01 a002 7405 a006  ....|.j.j...t...
-00000b40: a100 6a07 a101 0100 7c00 6a08 6a01 a002  ..j.....|.j.j...
-00000b50: 7c00 6a09 a101 0100 6400 5300 a901 4e29  |.j.....d.S...N)
-00000b60: 0a72 4600 0000 723e 0000 0072 3f00 0000  .rF...r>...r?...
-00000b70: da11 6c6f 6164 5f73 7472 6561 6d5f 746f  ..load_stream_to
-00000b80: 6f6c 7372 4500 0000 7207 0000 00da 0869  olsrE...r......i
-00000b90: 6e73 7461 6e63 65da 0471 7569 7472 4800  nstance..quitrH.
-00000ba0: 0000 da12 6469 7363 6f6e 6e65 6374 5f63  ....disconnect_c
-00000bb0: 616d 6572 6173 a901 7250 0000 0072 2e00  ameras..rP...r..
-00000bc0: 0000 722e 0000 0072 2f00 0000 7249 0000  ..r....r/...rI..
-00000bd0: 006b 0000 0073 0600 0000 1001 1401 1401  .k...s..........
-00000be0: 7a1f 4d61 696e 5769 6e64 6f77 2e63 6f6e  z.MainWindow.con
-00000bf0: 6e65 6374 5f6d 656e 755f 6163 7469 6f6e  nect_menu_action
-00000c00: 7363 0100 0000 0000 0000 0000 0000 0100  sc..............
-00000c10: 0000 0400 0000 4300 0000 73b4 0000 007c  ......C...s....|
-00000c20: 006a 00a0 017c 006a 02a1 0101 007c 006a  .j...|.j.....|.j
-00000c30: 00a0 0374 046a 056a 0664 01a1 0201 007c  ...t.j.j.d.....|
-00000c40: 006a 00a0 0374 046a 076a 0664 02a1 0201  .j...t.j.j.d....
-00000c50: 007c 006a 00a0 0374 046a 086a 0664 02a1  .|.j...t.j.j.d..
-00000c60: 0201 007c 006a 00a0 0374 046a 096a 0664  ...|.j...t.j.j.d
-00000c70: 02a1 0201 007c 006a 00a0 0374 046a 0a6a  .....|.j...t.j.j
-00000c80: 0664 01a1 0201 0074 0b83 007c 005f 0c74  .d.....t...|._.t
-00000c90: 0b83 007c 005f 0d74 0b83 007c 005f 0e7c  ...|._.t...|._.|
-00000ca0: 006a 0fa0 1074 116a 05a1 0101 007c 006a  .j...t.j.....|.j
-00000cb0: 0fa0 12a1 0001 007c 006a 13a0 1464 02a1  .......|.j...d..
-00000cc0: 0101 007c 006a 15a0 1464 01a1 0101 0064  ...|.j...d.....d
-00000cd0: 0053 0029 034e 5446 2916 724a 0000 00da  .S.).NTF).rJ....
-00000ce0: 1073 6574 4375 7272 656e 7457 6964 6765  .setCurrentWidge
-00000cf0: 74da 0e63 6861 7275 636f 5f77 6964 6765  t..charuco_widge
-00000d00: 74da 0d73 6574 5461 6245 6e61 626c 6564  t..setTabEnabled
-00000d10: 7221 0000 0072 2900 0000 da05 7661 6c75  r!...r).....valu
-00000d20: 6572 2a00 0000 722b 0000 0072 2c00 0000  er*...r+...r,...
-00000d30: 722d 0000 0072 0800 0000 da0d 6361 6d65  r-...r......came
-00000d40: 7261 5f77 6964 6765 74da 1f63 616c 6962  ra_widget..calib
-00000d50: 7261 7465 5f63 6170 7475 7265 5f76 6f6c  rate_capture_vol
-00000d60: 756d 655f 7769 6467 6574 da10 7265 636f  ume_widget..reco
-00000d70: 7264 696e 675f 7769 6467 6574 da07 7365  rding_widget..se
-00000d80: 7373 696f 6eda 0873 6574 5f6d 6f64 6572  ssion..set_moder
-00000d90: 1800 0000 7258 0000 0072 4800 0000 7247  ....rX...rH...rG
-00000da0: 0000 0072 4600 0000 7259 0000 0072 2e00  ...rF...rY...r..
-00000db0: 0000 722e 0000 0072 2f00 0000 7258 0000  ..r....r/...rX..
-00000dc0: 0070 0000 0073 1a00 0000 0e01 1201 1201  .p...s..........
-00000dd0: 1201 1201 1201 0802 0801 0801 0e02 0a01  ................
-00000de0: 0c01 1001 7a1d 4d61 696e 5769 6e64 6f77  ....z.MainWindow
-00000df0: 2e64 6973 636f 6e6e 6563 745f 6361 6d65  .disconnect_came
-00000e00: 7261 7363 0100 0000 0000 0000 0000 0000  rasc............
-00000e10: 0100 0000 0300 0000 4300 0000 7322 0000  ........C...s"..
-00000e20: 0074 00a0 0164 01a1 0101 007c 006a 02a0  .t...d.....|.j..
-00000e30: 03a1 0001 007c 006a 02a0 04a1 0001 0064  .....|.j.......d
-00000e40: 0053 0029 024e 7a55 5061 7573 696e 6720  .S.).NzUPausing 
-00000e50: 616c 6c20 6672 616d 6520 7265 6164 696e  all frame readin
-00000e60: 6720 6174 206c 6f61 6420 6f66 2073 7472  g at load of str
-00000e70: 6561 6d20 746f 6f6c 733b 2073 686f 756c  eam tools; shoul
-00000e80: 6420 6265 206f 6e20 6368 6172 7563 6f20  d be on charuco 
-00000e90: 7461 6220 7269 6768 7420 6e6f 7729 05da  tab right now)..
-00000ea0: 066c 6f67 6765 72da 0469 6e66 6f72 6100  .logger..infora.
-00000eb0: 0000 da19 7061 7573 655f 616c 6c5f 6d6f  ....pause_all_mo
-00000ec0: 6e6f 6361 6c69 6272 6174 6f72 73da 1270  nocalibrators..p
-00000ed0: 6175 7365 5f73 796e 6368 726f 6e69 7a65  ause_synchronize
-00000ee0: 7272 5900 0000 722e 0000 0072 2e00 0000  rrY...r....r....
-00000ef0: 722f 0000 00da 1770 6175 7365 5f61 6c6c  r/.....pause_all
-00000f00: 5f66 7261 6d65 5f72 6561 6469 6e67 8100  _frame_reading..
-00000f10: 0000 7306 0000 000a 010a 010e 017a 224d  ..s..........z"M
-00000f20: 6169 6e57 696e 646f 772e 7061 7573 655f  ainWindow.pause_
-00000f30: 616c 6c5f 6672 616d 655f 7265 6164 696e  all_frame_readin
-00000f40: 6763 0100 0000 0000 0000 0000 0000 0100  gc..............
-00000f50: 0000 0500 0000 4300 0000 734a 0000 007c  ......C...sJ...|
-00000f60: 006a 00a0 0164 01a1 0101 007c 006a 02a0  .j...d.....|.j..
-00000f70: 0164 02a1 0101 007c 006a 036a 04a0 057c  .d.....|.j.j...|
-00000f80: 006a 06a1 0101 0074 077c 006a 036a 0864  .j.....t.|.j.j.d
-00000f90: 0364 0264 048d 037c 005f 097c 006a 09a0  .d.d...|._.|.j..
-00000fa0: 0aa1 0001 0064 0053 0029 054e 4654 722e  .....d.S.).NFTr.
-00000fb0: 0000 0029 03da 0674 6172 6765 74da 0461  ...)...target..a
-00000fc0: 7267 73da 0664 6165 6d6f 6e29 0b72 4600  rgs..daemon).rF.
-00000fd0: 0000 7247 0000 0072 4800 0000 7261 0000  ..rG...rH...ra..
-00000fe0: 00da 1a73 7472 6561 6d5f 746f 6f6c 735f  ...stream_tools_
-00000ff0: 6c6f 6164 6564 5f73 6967 6e61 6c72 3f00  loaded_signalr?.
-00001000: 0000 7267 0000 0072 0600 0000 7255 0000  ..rg...r....rU..
-00001010: 00da 0674 6872 6561 64da 0573 7461 7274  ...thread..start
-00001020: 7259 0000 0072 2e00 0000 722e 0000 0072  rY...r....r....r
-00001030: 2f00 0000 7255 0000 0086 0000 0073 0e00  /...rU.......s..
-00001040: 0000 0c01 0c01 1001 0201 0a01 08ff 0e03  ................
-00001050: 7a1c 4d61 696e 5769 6e64 6f77 2e6c 6f61  z.MainWindow.loa
-00001060: 645f 7374 7265 616d 5f74 6f6f 6c73 6302  d_stream_toolsc.
-00001070: 0000 0000 0000 0000 0000 0002 0000 0006  ................
-00001080: 0000 0043 0000 0073 4401 0000 7400 a001  ...C...sD...t...
-00001090: 6401 7c01 9b00 9d02 a101 0100 7c01 0400  d.|.........|...
-000010a0: 7402 6a03 6a04 6b02 721e 0100 7400 a001  t.j.j.k.r...t...
-000010b0: 6402 a101 0100 7c00 6a05 a006 7407 6a03  d.....|.j...t.j.
-000010c0: a101 0100 6400 5300 0400 7402 6a08 6a04  ....d.S...t.j.j.
-000010d0: 6b02 7233 0100 7400 a001 6403 a101 0100  k.r3..t...d.....
-000010e0: 7c00 6a05 a006 7407 6a09 a101 0100 6400  |.j...t.j.....d.
-000010f0: 5300 0400 7402 6a0a 6a04 6b02 725c 0100  S...t.j.j.k.r\..
-00001100: 7400 a001 6404 a101 0100 7c00 6a05 a00b  t...d.....|.j...
-00001110: a100 7250 7400 a001 6405 a101 0100 7c00  ..rPt...d.....|.
-00001120: 6a0c a00d a100 0100 6400 5300 7400 a001  j.......d.S.t...
-00001130: 6406 a101 0100 7c00 6a0c a00e a100 0100  d.....|.j.......
-00001140: 6400 5300 0400 7402 6a0f 6a04 6b02 7288  d.S...t.j.j.k.r.
-00001150: 0100 7400 a001 6407 a101 0100 7a0d 7400  ..t...d.....z.t.
-00001160: a001 6408 a101 0100 7c00 6a0c 6a10 a011  ..d.....|.j.j...
-00001170: a100 0100 5700 6e09 0100 0100 0100 7400  ....W.n.......t.
-00001180: a001 6409 a101 0100 5900 7c00 6a05 a006  ..d.....Y.|.j...
-00001190: 7407 6a0f a101 0100 6400 5300 7402 6a12  t.j.....d.S.t.j.
-000011a0: 6a04 6b02 72a0 7400 a001 640a a101 0100  j.k.r.t...d.....
-000011b0: 7c00 6a05 a006 7407 6a13 a101 0100 7c00  |.j...t.j.....|.
-000011c0: 6a14 a015 a100 0100 6400 5300 6400 5300  j.......d.S.d.S.
-000011d0: 290b 4e7a 1d53 7769 7463 6869 6e67 206d  ).Nz.Switching m
-000011e0: 6169 6e20 7769 6e64 6f77 2074 6f20 7461  ain window to ta
-000011f0: 6220 7a19 4163 7469 7661 7469 6e67 2043  b z.Activating C
-00001200: 6861 7275 636f 2057 6964 6765 747a 1e41  haruco Widgetz.A
-00001210: 6374 6976 6174 696e 6720 4361 6d65 7261  ctivating Camera
-00001220: 2053 6574 7570 2057 6964 6765 747a 2a41   Setup Widgetz*A
-00001230: 6374 6976 6174 696e 6720 4361 6c69 6272  ctivating Calibr
-00001240: 6174 6520 4361 7074 7572 6520 566f 6c75  ate Capture Volu
-00001250: 6d65 2057 6964 6765 747a 5353 6573 7369  me WidgetzSSessi
-00001260: 6f6e 2069 7320 656c 6967 6962 6c65 2066  on is eligible f
-00001270: 6f72 2073 6574 7469 6e67 206f 6620 6f72  or setting of or
-00001280: 6967 696e 2e2e 2e61 6374 6976 6174 696e  igin...activatin
-00001290: 6720 6361 7074 7572 6520 766f 6c75 6d65  g capture volume
-000012a0: 206f 7269 6769 6e20 7769 6467 6574 7a57   origin widgetzW
-000012b0: 5365 7373 696f 6e20 6973 206e 6f74 2065  Session is not e
-000012c0: 6c69 6769 626c 6520 666f 7220 7365 7474  ligible for sett
-000012d0: 696e 6720 6f66 206f 7269 6769 6e2e 2e2e  ing of origin...
-000012e0: 6163 7469 7661 7469 6e67 2065 7874 7269  activating extri
-000012f0: 6e73 6963 2063 616c 6962 7261 7469 6f6e  nsic calibration
-00001300: 2077 6964 6765 747a 1741 6374 6976 6174   widgetz.Activat
-00001310: 6520 5265 636f 7264 696e 6720 4d6f 6465  e Recording Mode
-00001320: 7a38 4174 7465 6d70 7469 6e67 2074 6f20  z8Attempting to 
-00001330: 7370 696e 2064 6f77 6e20 7468 6520 6578  spin down the ex
-00001340: 7472 696e 7369 6320 6361 6c69 6272 6174  trinsic calibrat
-00001350: 696f 6e20 7769 6467 6574 7a32 4e6f 2065  ion widgetz2No e
-00001360: 7874 7269 6e73 6963 2063 616c 6962 7261  xtrinsic calibra
-00001370: 7469 6f6e 2063 616c 6962 7261 7469 6f6e  tion calibration
-00001380: 2077 6964 6765 7420 6578 6973 7473 7a18   widget existsz.
-00001390: 4163 7469 7661 7465 2050 726f 6365 7373  Activate Process
-000013a0: 696e 6720 4d6f 6465 2916 7263 0000 0072  ing Mode).rc...r
-000013b0: 6400 0000 7221 0000 0072 2900 0000 725d  d...r!...r)...r]
-000013c0: 0000 0072 6100 0000 7262 0000 0072 1800  ...ra...rb...r..
-000013d0: 0000 722a 0000 00da 1449 6e74 7269 6e73  ..r*.....Intrins
-000013e0: 6963 4361 6c69 6272 6174 696f 6e72 2b00  icCalibrationr+.
-000013f0: 0000 da1a 6973 5f63 6170 7475 7265 5f76  ....is_capture_v
-00001400: 6f6c 756d 655f 656c 6967 6962 6c65 725f  olume_eligibler_
-00001410: 0000 005a 1e61 6374 6976 6174 655f 6361  ...Z.activate_ca
-00001420: 7074 7572 655f 766f 6c75 6d65 5f77 6964  pture_volume_wid
-00001430: 6765 745a 2561 6374 6976 6174 655f 6578  getZ%activate_ex
-00001440: 7472 696e 7369 635f 6361 6c69 6272 6174  trinsic_calibrat
-00001450: 696f 6e5f 7769 6467 6574 722c 0000 00da  ion_widgetr,....
-00001460: 1c65 7874 7269 6e73 6963 5f63 616c 6962  .extrinsic_calib
-00001470: 7261 7469 6f6e 5f77 6964 6765 74da 1073  ration_widget..s
-00001480: 6875 7464 6f77 6e5f 7468 7265 6164 7372  hutdown_threadsr
-00001490: 2d00 0000 da0e 506f 7374 5072 6f63 6573  -.....PostProces
-000014a0: 7369 6e67 da11 7072 6f63 6573 7369 6e67  sing..processing
-000014b0: 5f77 6964 6765 745a 1875 7064 6174 655f  _widgetZ.update_
-000014c0: 7265 636f 7264 696e 675f 666f 6c64 6572  recording_folder
-000014d0: 73a9 0272 5000 0000 da05 696e 6465 7872  s..rP.....indexr
-000014e0: 2e00 0000 722e 0000 0072 2f00 0000 da0e  ....r....r/.....
-000014f0: 6f6e 5f74 6162 5f63 6861 6e67 6564 9100  on_tab_changed..
-00001500: 0000 7338 0000 0010 0102 010e 010a 0112  ..s8............
-00001510: 020e 010a 0112 020e 010a 010a 020a 010e  ................
-00001520: 010a 020e 010e 020a 0102 020a 0110 0106  ................
-00001530: 010c 0112 020a 010a 010e 020e 0204 fb7a  ...............z
-00001540: 194d 6169 6e57 696e 646f 772e 6f6e 5f74  .MainWindow.on_t
-00001550: 6162 5f63 6861 6e67 6564 da0e 7061 7468  ab_changed..path
-00001560: 5f74 6f5f 666f 6c64 6572 6302 0000 0000  _to_folderc.....
-00001570: 0000 0000 0000 0004 0000 0004 0000 0043  ...............C
-00001580: 0000 0073 f000 0000 7400 7c01 8301 7d02  ...s....t.|...}.
-00001590: 7401 7c02 8301 7c00 5f02 7403 a004 6401  t.|...|._.t...d.
-000015a0: 7c02 9b00 9d02 a101 0100 7405 7c00 6a02  |.........t.|.j.
-000015b0: 8301 7c00 5f06 7407 7c00 6a06 8301 7c00  ..|._.t.|.j...|.
-000015c0: 5f08 7409 8300 7c00 5f0a 7409 8300 7c00  _.t...|._.t...|.
-000015d0: 5f0b 7409 8300 7c00 5f0c 7409 8300 7c00  _.t...|._.t...|.
-000015e0: 5f0d 7c00 6a0e a00f 7c00 6a08 6402 a102  _.|.j...|.j.d...
-000015f0: 0100 7c00 6a0e a00f 7c00 6a0a 6403 a102  ..|.j...|.j.d...
-00001600: 0100 7c00 6a0e a00f 7c00 6a0d 6404 a102  ..|.j...|.j.d...
-00001610: 0100 7c00 6a0e a00f 7c00 6a0b 6405 a102  ..|.j...|.j.d...
-00001620: 0100 7c00 6a0e a00f 7c00 6a0c 6406 a102  ..|.j...|.j.d...
-00001630: 0100 7c00 6a0e 6a10 a011 7c00 6a12 a101  ..|.j.j...|.j...
-00001640: 0100 7c00 6a13 a014 6407 a101 0100 7c00  ..|.j...d.....|.
-00001650: a015 a100 0100 7c00 6a0e a016 a100 7d03  ......|.j.....}.
-00001660: 7c00 6a0e a017 7c03 a101 0100 7c00 a018  |.j...|.....|...
-00001670: a100 0100 6400 5300 2908 4e7a 2d4c 6175  ....d.S.).Nz-Lau
-00001680: 6e63 6869 6e67 2073 6573 7369 6f6e 2077  nching session w
-00001690: 6974 6820 636f 6e66 6967 2066 696c 6520  ith config file 
-000016a0: 7374 6f72 6564 2069 6e20 7229 0000 0072  stored in r)...r
-000016b0: 2a00 0000 722b 0000 0072 2c00 0000 722d  *...r+...r,...r-
-000016c0: 0000 0054 2919 7205 0000 0072 1a00 0000  ...T).r....r....
-000016d0: da06 636f 6e66 6967 7263 0000 0072 6400  ..configrc...rd.
-000016e0: 0000 7217 0000 0072 6100 0000 721c 0000  ..r....ra...r...
-000016f0: 0072 5b00 0000 7208 0000 0072 5e00 0000  .r[...r....r^...
-00001700: 7260 0000 0072 7300 0000 725f 0000 0072  r`...rs...r_...r
-00001710: 4a00 0000 da06 6164 6454 6162 da0e 6375  J.....addTab..cu
-00001720: 7272 656e 7443 6861 6e67 6564 723f 0000  rrentChangedr?..
-00001730: 0072 7600 0000 7246 0000 0072 4700 0000  .rv...rF...rG...
-00001740: da0b 7570 6461 7465 5f74 6162 73da 0c63  ..update_tabs..c
-00001750: 7572 7265 6e74 496e 6465 78da 0f73 6574  urrentIndex..set
-00001760: 4375 7272 656e 7449 6e64 6578 da17 636f  CurrentIndex..co
-00001770: 6e6e 6563 745f 7365 7373 696f 6e5f 7369  nnect_session_si
-00001780: 676e 616c 7329 0472 5000 0000 7277 0000  gnals).rP...rw..
-00001790: 00da 0c73 6573 7369 6f6e 5f70 6174 685a  ...session_pathZ
-000017a0: 096f 6c64 5f69 6e64 6578 722e 0000 0072  .old_indexr....r
-000017b0: 2e00 0000 722f 0000 00da 0e6c 6175 6e63  ....r/.....launc
-000017c0: 685f 7365 7373 696f 6eb7 0000 0073 2800  h_session....s(.
-000017d0: 0000 0801 0a01 1001 0c01 0c03 0803 0801  ................
-000017e0: 0801 0801 1002 1001 1001 1001 1001 1003  ................
-000017f0: 0c03 0804 0a03 0c02 0c01 7a19 4d61 696e  ..........z.Main
-00001800: 5769 6e64 6f77 2e6c 6175 6e63 685f 7365  Window.launch_se
-00001810: 7373 696f 6e63 0100 0000 0000 0000 0000  ssionc..........
-00001820: 0000 0100 0000 0400 0000 4300 0000 7308  ..........C...s.
-00001830: 0100 007c 006a 00a0 0174 026a 036a 0464  ...|.j...t.j.j.d
-00001840: 01a1 0201 007c 006a 056a 0672 4a74 077c  .....|.j.j.rJt.|
-00001850: 006a 0883 0174 096b 0372 187c 00a0 0aa1  .j...t.k.r.|....
-00001860: 0001 0074 077c 006a 0b83 0174 0c6b 0372  ...t.|.j...t.k.r
-00001870: 237c 00a0 0da1 0001 0074 077c 006a 0e83  #|.......t.|.j..
-00001880: 0174 0f6b 0372 2e7c 00a0 10a1 0001 007c  .t.k.r.|.......|
-00001890: 006a 00a0 0174 026a 116a 0464 01a1 0201  .j...t.j.j.d....
-000018a0: 007c 006a 00a0 0174 026a 126a 0464 01a1  .|.j...t.j.j.d..
-000018b0: 0201 007c 006a 00a0 0174 026a 136a 0464  ...|.j...t.j.j.d
-000018c0: 01a1 0201 006e 1b7c 006a 00a0 0174 026a  .....n.|.j...t.j
-000018d0: 116a 0464 02a1 0201 007c 006a 00a0 0174  .j.d.....|.j...t
-000018e0: 026a 126a 0464 02a1 0201 007c 006a 00a0  .j.j.d.....|.j..
-000018f0: 0174 026a 136a 0464 02a1 0201 007c 006a  .t.j.j.d.....|.j
-00001900: 05a0 14a1 0072 797c 00a0 15a1 0001 007c  .....ry|.......|
-00001910: 006a 00a0 0174 026a 166a 0464 01a1 0201  .j...t.j.j.d....
-00001920: 0064 0353 007c 006a 00a0 0174 026a 166a  .d.S.|.j...t.j.j
-00001930: 0464 02a1 0201 0064 0353 0029 0461 0b01  .d.....d.S.).a..
-00001940: 0000 0a20 2020 2020 2020 2054 6162 2075  ...        Tab u
-00001950: 7064 6174 6573 206f 6363 7572 2070 7269  pdates occur pri
-00001960: 6d61 7269 6c79 2061 7420 3220 7469 6d65  marily at 2 time
-00001970: 733a 0a20 2020 2020 2020 2031 2e20 7570  s:.        1. up
-00001980: 6f6e 206d 6169 6e20 7769 6e64 6f77 2069  on main window i
-00001990: 6e69 7469 6174 696f 6e20 7768 656e 206f  nitiation when o
-000019a0: 6666 6c69 6e65 2063 6170 6163 6974 6965  ffline capacitie
-000019b0: 7320 0a20 2020 2020 2020 2028 6361 7074  s .        (capt
-000019c0: 7572 6520 766f 6c75 6d65 2061 6e64 2070  ure volume and p
-000019d0: 6f73 742d 7072 6f63 6573 7369 6e67 2920  ost-processing) 
-000019e0: 6d61 7920 6265 2061 7661 696c 6162 6c65  may be available
-000019f0: 2e0a 0a20 2020 2020 2020 2032 2e20 7570  ...        2. up
-00001a00: 6f6e 206c 6f61 6469 6e67 206f 6620 7374  on loading of st
-00001a10: 7265 616d 2074 6f6f 6c73 2077 6865 6e20  ream tools when 
-00001a20: 6361 6d65 7261 732f 7265 636f 7264 696e  cameras/recordin
-00001a30: 6720 776f 756c 6420 6265 2061 7661 696c  g would be avail
-00001a40: 6162 6c65 0a20 2020 2020 2020 2054 464e  able.        TFN
-00001a50: 2917 724a 0000 0072 5c00 0000 7221 0000  ).rJ...r\...r!..
-00001a60: 0072 2900 0000 725d 0000 0072 6100 0000  .r)...r]...ra...
-00001a70: da13 7374 7265 616d 5f74 6f6f 6c73 5f6c  ..stream_tools_l
-00001a80: 6f61 6465 64da 0474 7970 6572 5e00 0000  oaded..typer^...
-00001a90: 721d 0000 00da 126c 6f61 645f 6361 6d65  r......load_came
-00001aa0: 7261 5f77 6964 6765 7472 6000 0000 721f  ra_widgetr`...r.
-00001ab0: 0000 00da 156c 6f61 645f 7265 636f 7264  .....load_record
-00001ac0: 696e 675f 7769 6467 6574 725f 0000 0072  ing_widgetr_...r
-00001ad0: 1e00 0000 da1a 6c6f 6164 5f63 6170 7475  ......load_captu
-00001ae0: 7265 5f76 6f6c 756d 655f 7769 6467 6574  re_volume_widget
-00001af0: 722a 0000 0072 2c00 0000 722b 0000 00da  r*...r,...r+....
-00001b00: 1b69 735f 706f 7374 5f70 726f 6365 7373  .is_post_process
-00001b10: 696e 675f 656c 6967 6962 6c65 da1b 6c6f  ing_eligible..lo
-00001b20: 6164 5f70 6f73 745f 7072 6f63 6573 7369  ad_post_processi
-00001b30: 6e67 5f77 6964 6765 7472 2d00 0000 7259  ng_widgetr-...rY
-00001b40: 0000 0072 2e00 0000 722e 0000 0072 2f00  ...r....r....r/.
-00001b50: 0000 727b 0000 00dc 0000 0073 2400 0000  ..r{.......s$...
-00001b60: 120a 0803 0e02 0801 0e02 0801 0e02 0801  ................
-00001b70: 1202 1201 1401 1205 1201 1201 0a03 0801  ................
-00001b80: 1601 1602 7a16 4d61 696e 5769 6e64 6f77  ....z.MainWindow
-00001b90: 2e75 7064 6174 655f 7461 6273 6301 0000  .update_tabsc...
-00001ba0: 0000 0000 0000 0000 0001 0000 0003 0000  ................
-00001bb0: 0043 0000 0073 2400 0000 7c00 6a00 6a01  .C...s$...|.j.j.
-00001bc0: a002 7c00 6a03 a101 0100 7c00 6a00 6a04  ..|.j.....|.j.j.
-00001bd0: a002 7c00 6a05 a101 0100 6401 5300 2902  ..|.j.....d.S.).
-00001be0: 7a90 0a20 2020 2020 2020 2041 6674 6572  z..        After
-00001bf0: 206c 6175 6e63 6869 6e67 2061 2073 6573   launching a ses
-00001c00: 7369 6f6e 2c20 636f 6e6e 6563 7420 7369  sion, connect si
-00001c10: 676e 616c 7320 616e 6420 736c 6f74 732e  gnals and slots.
-00001c20: 0a20 2020 2020 2020 204d 7563 6820 6f66  .        Much of
-00001c30: 2074 6865 7365 2077 696c 6c20 6265 2066   these will be f
-00001c40: 726f 6d20 7468 6520 4755 4920 746f 2074  rom the GUI to t
-00001c50: 6865 2073 6573 7369 6f6e 2061 6e64 2076  he session and v
-00001c60: 6963 652d 7665 7273 610a 2020 2020 2020  ice-versa.      
-00001c70: 2020 4e29 0672 6100 0000 da15 756e 6c6f    N).ra.....unlo
-00001c80: 636b 5f70 6f73 7470 726f 6365 7373 696e  ck_postprocessin
-00001c90: 6772 3f00 0000 7287 0000 0072 6b00 0000  gr?...r....rk...
-00001ca0: 727b 0000 0072 5900 0000 722e 0000 0072  r{...rY...r....r
-00001cb0: 2e00 0000 722f 0000 0072 7e00 0000 0801  ....r/...r~.....
-00001cc0: 0000 7304 0000 0010 0514 017a 224d 6169  ..s........z"Mai
-00001cd0: 6e57 696e 646f 772e 636f 6e6e 6563 745f  nWindow.connect_
-00001ce0: 7365 7373 696f 6e5f 7369 676e 616c 7363  session_signalsc
-00001cf0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00001d00: 0500 0000 4300 0000 f346 0000 007c 006a  ....C....F...|.j
-00001d10: 00a0 0174 026a 036a 04a1 0101 007c 006a  ...t.j.j.....|.j
-00001d20: 05a0 06a1 0001 0074 077c 006a 0883 017d  .......t.|.j...}
-00001d30: 017c 006a 00a0 0974 026a 036a 047c 0174  .|.j...t.j.j.|.t
-00001d40: 026a 036a 0aa1 0301 007c 017c 005f 0564  .j.j.....|.|._.d
-00001d50: 0053 0072 5400 0000 290b 724a 0000 00da  .S.rT...).rJ....
-00001d60: 0972 656d 6f76 6554 6162 7221 0000 0072  .removeTabr!...r
-00001d70: 2c00 0000 725d 0000 0072 6000 0000 da0b  ,...r]...r`.....
-00001d80: 6465 6c65 7465 4c61 7465 7272 1f00 0000  deleteLaterr....
-00001d90: 7261 0000 00da 0969 6e73 6572 7454 6162  ra.....insertTab
-00001da0: da04 6e61 6d65 2902 7250 0000 005a 146e  ..name).rP...Z.n
-00001db0: 6577 5f72 6563 6f72 6469 6e67 5f77 6964  ew_recording_wid
-00001dc0: 6765 7472 2e00 0000 722e 0000 0072 2f00  getr....r....r/.
-00001dd0: 0000 7284 0000 0010 0100 0073 0e00 0000  ..r........s....
-00001de0: 1002 0a01 0a01 0601 0e01 04ff 0a03 7a20  ..............z 
-00001df0: 4d61 696e 5769 6e64 6f77 2e6c 6f61 645f  MainWindow.load_
-00001e00: 7265 636f 7264 696e 675f 7769 6467 6574  recording_widget
-00001e10: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00001e20: 0005 0000 0043 0000 0072 8900 0000 7254  .....C...r....rT
-00001e30: 0000 0029 0b72 4a00 0000 728a 0000 0072  ...).rJ...r....r
-00001e40: 2100 0000 722d 0000 0072 5d00 0000 7273  !...r-...r]...rs
-00001e50: 0000 0072 8b00 0000 7220 0000 0072 6100  ...r....r ...ra.
-00001e60: 0000 728c 0000 0072 8d00 0000 2902 7250  ..r....r....).rP
-00001e70: 0000 005a 156e 6577 5f70 726f 6365 7373  ...Z.new_process
-00001e80: 696e 675f 7769 6467 6574 722e 0000 0072  ing_widgetr....r
-00001e90: 2e00 0000 722f 0000 0072 8700 0000 1a01  ....r/...r......
-00001ea0: 0000 f30e 0000 0010 010a 010a 0106 010e  ................
-00001eb0: 0104 ff0a 037a 264d 6169 6e57 696e 646f  .....z&MainWindo
-00001ec0: 772e 6c6f 6164 5f70 6f73 745f 7072 6f63  w.load_post_proc
-00001ed0: 6573 7369 6e67 5f77 6964 6765 7463 0100  essing_widgetc..
-00001ee0: 0000 0000 0000 0000 0000 0200 0000 0500  ................
-00001ef0: 0000 4300 0000 7289 0000 0072 5400 0000  ..C...r....rT...
-00001f00: 290b 724a 0000 0072 8a00 0000 7221 0000  ).rJ...r....r!..
-00001f10: 0072 2b00 0000 725d 0000 0072 5f00 0000  .r+...r]...r_...
-00001f20: 728b 0000 0072 1e00 0000 7261 0000 0072  r....r....ra...r
-00001f30: 8c00 0000 728d 0000 0029 0272 5000 0000  ....r....).rP...
-00001f40: 5a19 6e65 775f 6361 7074 7572 655f 766f  Z.new_capture_vo
-00001f50: 6c75 6d65 5f77 6964 6765 7472 2e00 0000  lume_widgetr....
-00001f60: 722e 0000 0072 2f00 0000 7285 0000 0023  r....r/...r....#
-00001f70: 0100 0073 1200 0000 1001 0a01 0a01 0601  ...s............
-00001f80: 0601 0201 0601 04fd 0a05 7a25 4d61 696e  ..........z%Main
-00001f90: 5769 6e64 6f77 2e6c 6f61 645f 6361 7074  Window.load_capt
-00001fa0: 7572 655f 766f 6c75 6d65 5f77 6964 6765  ure_volume_widge
-00001fb0: 7463 0100 0000 0000 0000 0000 0000 0200  tc..............
-00001fc0: 0000 0500 0000 4300 0000 7289 0000 0072  ......C...r....r
-00001fd0: 5400 0000 290b 724a 0000 0072 8a00 0000  T...).rJ...r....
-00001fe0: 7221 0000 0072 2a00 0000 725d 0000 0072  r!...r*...r]...r
-00001ff0: 5e00 0000 728b 0000 0072 1d00 0000 7261  ^...r....r....ra
-00002000: 0000 0072 8c00 0000 728d 0000 0029 0272  ...r....r....).r
-00002010: 5000 0000 5a11 6e65 775f 6361 6d65 7261  P...Z.new_camera
-00002020: 5f77 6964 6765 7472 2e00 0000 722e 0000  _widgetr....r...
-00002030: 0072 2f00 0000 7283 0000 002e 0100 0072  .r/...r........r
-00002040: 8e00 0000 7a1d 4d61 696e 5769 6e64 6f77  ....z.MainWindow
-00002050: 2e6c 6f61 645f 6361 6d65 7261 5f77 6964  .load_camera_wid
-00002060: 6765 7472 5100 0000 6302 0000 0000 0000  getrQ...c.......
-00002070: 0000 0000 0003 0000 0003 0000 0043 0000  .............C..
-00002080: 0073 2800 0000 7400 7c01 7c00 8302 7d02  .s(...t.|.|...}.
-00002090: 7c02 6a01 a002 7c00 6a03 a101 0100 7c00  |.j...|.j.....|.
-000020a0: 6a04 a005 7c02 a101 0100 6400 5300 7254  j...|.....d.S.rT
-000020b0: 0000 0029 0672 1000 0000 723e 0000 0072  ...).r....r>...r
-000020c0: 3f00 0000 da13 6f70 656e 5f72 6563 656e  ?.....open_recen
-000020d0: 745f 7072 6f6a 6563 7472 4200 0000 7241  t_projectrB...rA
-000020e0: 0000 0029 0372 5000 0000 7251 0000 005a  ...).rP...rQ...Z
-000020f0: 1572 6563 656e 745f 7072 6f6a 6563 745f  .recent_project_
-00002100: 6163 7469 6f6e 722e 0000 0072 2e00 0000  actionr....r....
-00002110: 722f 0000 0072 4400 0000 3a01 0000 7306  r/...rD...:...s.
-00002120: 0000 000a 010e 0110 017a 204d 6169 6e57  .........z MainW
-00002130: 696e 646f 772e 6164 645f 746f 5f72 6563  indow.add_to_rec
-00002140: 656e 745f 7072 6f6a 6563 7463 0100 0000  ent_projectc....
-00002150: 0000 0000 0000 0000 0300 0000 0400 0000  ................
-00002160: 4300 0000 732e 0000 007c 00a0 00a1 007d  C...s....|.....}
-00002170: 017c 01a0 01a1 007d 0274 02a0 0364 017c  .|.....}.t...d.|
-00002180: 029b 009d 02a1 0101 007c 00a0 047c 02a1  .........|...|..
-00002190: 0101 0064 0053 0029 024e 7a21 4f70 656e  ...d.S.).Nz!Open
-000021a0: 696e 6720 7265 6365 6e74 2073 6573 7369  ing recent sessi
-000021b0: 6f6e 2073 746f 7265 6420 6174 2029 05da  on stored at )..
-000021c0: 0673 656e 6465 72da 0474 6578 7472 6300  .sender..textrc.
-000021d0: 0000 7264 0000 0072 8000 0000 2903 7250  ..rd...r....).rP
-000021e0: 0000 00da 0661 6374 696f 6e72 5100 0000  .....actionrQ...
-000021f0: 722e 0000 0072 2e00 0000 722f 0000 0072  r....r....r/...r
-00002200: 8f00 0000 3f01 0000 7308 0000 0008 0108  ....?...s.......
-00002210: 0110 010e 017a 1e4d 6169 6e57 696e 646f  .....z.MainWindo
-00002220: 772e 6f70 656e 5f72 6563 656e 745f 7072  w.open_recent_pr
-00002230: 6f6a 6563 7463 0100 0000 0000 0000 0000  ojectc..........
-00002240: 0000 0400 0000 0600 0000 4300 0000 735c  ..........C...s\
-00002250: 0000 0074 007c 006a 0164 0119 0083 017d  ...t.|.j.d.....}
-00002260: 0174 0283 007d 027c 026a 0364 0064 0274  .t...}.|.j.d.d.t
-00002270: 047c 0183 0174 026a 056a 0664 038d 047d  .|...t.j.j.d...}
-00002280: 037c 0372 2c74 07a0 0864 047c 0366 02a1  .|.r,t...d.|.f..
-00002290: 0101 007c 00a0 097c 03a1 0101 007c 00a0  ...|...|.....|..
-000022a0: 0a7c 03a1 0101 0064 0053 0064 0053 0029  .|.....d.S.d.S.)
-000022b0: 054e da13 6c61 7374 5f70 726f 6a65 6374  .N..last_project
-000022c0: 5f70 6172 656e 747a 2d4f 7065 6e20 5072  _parentz-Open Pr
-000022d0: 6576 696f 7573 206f 7220 4372 6561 7465  evious or Create
-000022e0: 204e 6577 2050 726f 6a65 6374 2044 6972   New Project Dir
-000022f0: 6563 746f 7279 2904 da06 7061 7265 6e74  ectory)...parent
-00002300: da07 6361 7074 696f 6eda 0964 6972 6563  ..caption..direc
-00002310: 746f 7279 da07 6f70 7469 6f6e 737a 1943  tory..optionsz.C
-00002320: 7265 6174 696e 6720 6e65 7720 7072 6f6a  reating new proj
-00002330: 6563 7420 696e 203a 290b 7205 0000 0072  ect in :).r....r
-00002340: 3700 0000 7204 0000 005a 1467 6574 4578  7...r....Z.getEx
-00002350: 6973 7469 6e67 4469 7265 6374 6f72 7972  istingDirectoryr
-00002360: 3a00 0000 da06 4f70 7469 6f6e 5a0c 5368  :.....OptionZ.Sh
-00002370: 6f77 4469 7273 4f6e 6c79 7263 0000 0072  owDirsOnlyrc...r
-00002380: 6400 0000 da15 6164 645f 7072 6f6a 6563  d.....add_projec
-00002390: 745f 746f 5f72 6563 656e 7472 8000 0000  t_to_recentr....
-000023a0: 2904 7250 0000 005a 0e64 6566 6175 6c74  ).rP...Z.default
-000023b0: 5f66 6f6c 6465 725a 0664 6961 6c6f 6772  _folderZ.dialogr
-000023c0: 7700 0000 722e 0000 0072 2e00 0000 722f  w...r....r....r/
-000023d0: 0000 0072 4000 0000 4501 0000 731a 0000  ...r@...E...s...
-000023e0: 000e 0106 0104 0102 0102 0106 0106 0106  ................
-000023f0: fc04 070e 010a 010e 0104 fd7a 244d 6169  ...........z$Mai
-00002400: 6e57 696e 646f 772e 6372 6561 7465 5f6e  nWindow.create_n
-00002410: 6577 5f70 726f 6a65 6374 5f66 6f6c 6465  ew_project_folde
-00002420: 7263 0200 0000 0000 0000 0000 0000 0200  rc..............
-00002430: 0000 0400 0000 4300 0000 7354 0000 0074  ......C...sT...t
-00002440: 007c 0183 017c 006a 0164 0119 0076 0072  .|...|.j.d...v.r
-00002450: 0b64 0053 007c 006a 0164 0119 00a0 0274  .d.S.|.j.d.....t
-00002460: 007c 0183 01a1 0101 0074 0074 037c 0183  .|.......t.t.|..
-00002470: 016a 0483 017c 006a 0164 023c 007c 00a0  .j...|.j.d.<.|..
-00002480: 05a1 0001 007c 00a0 067c 01a1 0101 0064  .....|...|.....d
-00002490: 0053 0029 034e 7232 0000 0072 9300 0000  .S.).Nr2...r....
-000024a0: 2907 723a 0000 0072 3700 0000 da06 6170  ).r:...r7.....ap
-000024b0: 7065 6e64 7205 0000 0072 9400 0000 da13  pendr....r......
-000024c0: 7570 6461 7465 5f61 7070 5f73 6574 7469  update_app_setti
-000024d0: 6e67 7372 4400 0000 2902 7250 0000 005a  ngsrD...).rP...Z
-000024e0: 0b66 6f6c 6465 725f 7061 7468 722e 0000  .folder_pathr...
-000024f0: 0072 2e00 0000 722f 0000 0072 9900 0000  .r....r/...r....
-00002500: 5401 0000 730c 0000 0012 0104 0114 0214  T...s...........
-00002510: 0108 010e 017a 204d 6169 6e57 696e 646f  .....z MainWindo
-00002520: 772e 6164 645f 7072 6f6a 6563 745f 746f  w.add_project_to
-00002530: 5f72 6563 656e 7463 0100 0000 0000 0000  _recentc........
-00002540: 0000 0000 0200 0000 0800 0000 4300 0000  ............C...
-00002550: 733e 0000 0074 0074 0164 0183 028f 107d  s>...t.t.d.....}
-00002560: 0174 02a0 037c 006a 047c 01a1 0201 0057  .t...|.j.|.....W
-00002570: 0064 0004 0004 0083 0301 0064 0053 0031  .d.........d.S.1
-00002580: 0073 1877 0101 0001 0001 0059 0001 0064  .s.w.......Y...d
-00002590: 0053 0029 024e da01 7729 05da 046f 7065  .S.).N..w)...ope
-000025a0: 6e72 1500 0000 7235 0000 00da 0464 756d  nr....r5.....dum
-000025b0: 7072 3700 0000 2902 7250 0000 00da 0166  pr7...).rP.....f
-000025c0: 722e 0000 0072 2e00 0000 722f 0000 0072  r....r....r/...r
-000025d0: 9b00 0000 5d01 0000 7306 0000 000c 0110  ....]...s.......
-000025e0: 0122 ff7a 1e4d 6169 6e57 696e 646f 772e  .".z.MainWindow.
-000025f0: 7570 6461 7465 5f61 7070 5f73 6574 7469  update_app_setti
-00002600: 6e67 7329 1772 2600 0000 7227 0000 0072  ngs).r&...r'...r
-00002610: 2800 0000 7234 0000 0072 4900 0000 7258  (...r4...rI...rX
-00002620: 0000 0072 6700 0000 7255 0000 0072 7600  ...rg...rU...rv.
-00002630: 0000 723a 0000 0072 8000 0000 727b 0000  ..r:...r....r{..
-00002640: 0072 7e00 0000 7284 0000 0072 8700 0000  .r~...r....r....
-00002650: 7285 0000 0072 8300 0000 7244 0000 0072  r....r....rD...r
-00002660: 8f00 0000 7240 0000 0072 9900 0000 729b  ....r@...r....r.
-00002670: 0000 00da 0d5f 5f63 6c61 7373 6365 6c6c  .....__classcell
-00002680: 5f5f 722e 0000 0072 2e00 0000 7252 0000  __r....r....rR..
-00002690: 0072 2f00 0000 7230 0000 0031 0000 0073  .r/...r0...1...s
-000026a0: 2600 0000 0800 0c01 0839 0805 0811 0805  &........9......
-000026b0: 080b 0e26 0825 082c 0808 080a 0809 080b  ...&.%.,........
-000026c0: 0e0c 0805 0806 080f 1009 7230 0000 0063  ..........r0...c
-000026d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000026e0: 0300 0000 0000 0000 732c 0000 0065 005a  ........s,...e.Z
-000026f0: 0164 005a 0264 015a 0387 0066 0164 0264  .d.Z.d.Z...f.d.d
-00002700: 0384 085a 0487 0066 0164 0464 0584 085a  ...Z...f.d.d...Z
-00002710: 0587 0004 005a 0653 0029 06da 1043 656e  .....Z.S.)...Cen
-00002720: 7472 616c 5461 6257 6964 6765 7461 8901  tralTabWidgeta..
-00002730: 0000 0a20 2020 2053 7769 7463 6869 6e67  ...    Switching
-00002740: 2062 6574 7765 656e 2074 6162 732c 2070   between tabs, p
-00002750: 6172 7469 6375 6c61 726c 7920 7768 656e  articularly when
-00002760: 2073 7973 7465 6d20 7265 736f 7572 6365   system resource
-00002770: 2075 7469 6c69 7a61 7469 6f6e 2069 7320   utilization is 
-00002780: 6869 6768 2c0a 2020 2020 6973 2070 726f  high,.    is pro
-00002790: 6e65 2074 6f20 7265 7375 6c74 2069 6e20  ne to result in 
-000027a0: 7365 6766 6175 6c74 2063 7261 7368 6573  segfault crashes
-000027b0: 2e20 576f 726b 696e 6720 6879 706f 7468  . Working hypoth
-000027c0: 6573 6973 2069 7320 7468 6174 2074 6869  esis is that thi
-000027d0: 7320 6973 2064 7565 2074 6f20 6d6f 6465  s is due to mode
-000027e0: 0a20 2020 2063 6861 6e67 6573 2068 6170  .    changes hap
-000027f0: 7065 6e69 6e67 2077 6865 6e20 7468 6520  pening when the 
-00002800: 7461 6220 6973 2063 6861 6e67 6564 2061  tab is changed a
-00002810: 6e64 2074 6865 2047 5549 2074 7269 6573  nd the GUI tries
-00002820: 2074 6f20 7265 6e64 6572 2073 6f6d 6574   to render somet
-00002830: 6869 6e67 2069 7420 646f 6573 6e27 7420  hing it doesn't 
-00002840: 6861 7665 0a20 2020 200a 2020 2020 5468  have.    .    Th
-00002850: 6973 206f 7665 7272 6964 6520 736c 6970  is override slip
-00002860: 7320 7468 6520 6d6f 6465 2063 6861 6e67  s the mode chang
-00002870: 6520 6265 7477 6565 6e20 636c 6963 6b20  e between click 
-00002880: 616e 6420 6368 616e 6765 2074 6f20 7472  and change to tr
-00002890: 7920 746f 2073 7461 6269 6c69 7a65 2074  y to stabilize t
-000028a0: 6865 206d 6f64 6520 7377 6974 6368 6573  he mode switches
-000028b0: 2e0a 2020 2020 0a20 2020 2063 0100 0000  ..    .    c....
-000028c0: 0000 0000 0000 0000 0100 0000 0300 0000  ................
-000028d0: 0300 0000 7312 0000 0074 0074 017c 0083  ....s....t.t.|..
-000028e0: 02a0 02a1 0001 0064 0053 0072 5400 0000  .......d.S.rT...
-000028f0: 2903 7233 0000 0072 a100 0000 7234 0000  ).r3...r....r4..
-00002900: 0072 5900 0000 7252 0000 0072 2e00 0000  .rY...rR...r....
-00002910: 722f 0000 0072 3400 0000 6c01 0000 7302  r/...r4...l...s.
-00002920: 0000 0012 017a 1943 656e 7472 616c 5461  .....z.CentralTa
-00002930: 6257 6964 6765 742e 5f5f 696e 6974 5f5f  bWidget.__init__
-00002940: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-00002950: 0005 0000 0003 0000 0073 2600 0000 7400  .........s&...t.
-00002960: a001 6401 7c01 9b00 6402 9d03 a101 0100  ..d.|...d.......
-00002970: 7402 7403 7c00 8302 a004 7c01 a101 0100  t.t.|.....|.....
-00002980: 6400 5300 2903 4e7a 0454 6162 207a 0820  d.S.).Nz.Tab z. 
-00002990: 636c 6963 6b65 6429 0572 6300 0000 7264  clicked).rc...rd
-000029a0: 0000 0072 3300 0000 72a1 0000 00da 0d74  ...r3...r......t
-000029b0: 6162 4261 7243 6c69 636b 6564 7274 0000  abBarClickedrt..
-000029c0: 0072 5200 0000 722e 0000 0072 2f00 0000  .rR...r....r/...
-000029d0: 72a2 0000 006f 0100 0073 0400 0000 1202  r....o...s......
-000029e0: 1403 7a1e 4365 6e74 7261 6c54 6162 5769  ..z.CentralTabWi
-000029f0: 6467 6574 2e74 6162 4261 7243 6c69 636b  dget.tabBarClick
-00002a00: 6564 2907 7226 0000 0072 2700 0000 7228  ed).r&...r'...r(
-00002a10: 0000 00da 075f 5f64 6f63 5f5f 7234 0000  .....__doc__r4..
-00002a20: 0072 a200 0000 72a0 0000 0072 2e00 0000  .r....r....r....
-00002a30: 722e 0000 0072 5200 0000 722f 0000 0072  r....rR...r/...r
-00002a40: a100 0000 6201 0000 7308 0000 0008 0004  ....b...s.......
-00002a50: 010c 0914 0372 a100 0000 6300 0000 0000  .....r....c.....
-00002a60: 0000 0000 0000 0002 0000 0002 0000 0043  ...............C
-00002a70: 0000 0073 2400 0000 7400 7401 6a02 8301  ...s$...t.t.j...
-00002a80: 7d00 7403 8300 7d01 7c01 a004 a100 0100  }.t...}.|.......
-00002a90: 7c00 a005 a100 0100 6400 5300 7254 0000  |.......d.S.rT..
-00002aa0: 0029 0672 0700 0000 da03 7379 73da 0461  .).r......sys..a
-00002ab0: 7267 7672 3000 0000 da04 7368 6f77 da04  rgvr0.....show..
-00002ac0: 6578 6563 2902 da03 6170 70da 0677 696e  exec)...app..win
-00002ad0: 646f 7772 2e00 0000 722e 0000 0072 2f00  dowr....r....r/.
-00002ae0: 0000 da0b 6c61 756e 6368 5f6d 6169 6e76  ....launch_mainv
-00002af0: 0100 0073 0800 0000 0a01 0601 0801 0c02  ...s............
-00002b00: 72aa 0000 00da 085f 5f6d 6169 6e5f 5f29  r......__main__)
-00002b10: 39da 0d70 7978 7933 642e 6c6f 6767 6572  9..pyxy3d.logger
-00002b20: da06 7079 7879 3364 7263 0000 00da 0367  ..pyxy3drc.....g
-00002b30: 6574 7226 0000 00da 0f50 7951 7436 2e51  etr&.....PyQt6.Q
-00002b40: 7457 6964 6765 7473 7202 0000 0072 0300  tWidgetsr....r..
-00002b50: 0000 7204 0000 00da 0770 6174 686c 6962  ..r......pathlib
-00002b60: 7205 0000 00da 0974 6872 6561 6469 6e67  r......threading
-00002b70: 7206 0000 0072 a400 0000 7207 0000 0072  r....r....r....r
-00002b80: 0800 0000 7209 0000 0072 0a00 0000 720b  ....r....r....r.
-00002b90: 0000 0072 0c00 0000 720d 0000 0072 3500  ...r....r....r5.
-00002ba0: 0000 da04 656e 756d 720e 0000 005a 0b50  ....enumr....Z.P
-00002bb0: 7951 7436 2e51 7447 7569 720f 0000 0072  yQt6.QtGuir....r
-00002bc0: 1000 0000 7211 0000 0072 1200 0000 da0c  ....r....r......
-00002bd0: 5079 5174 362e 5174 436f 7265 7213 0000  PyQt6.QtCorer...
-00002be0: 0072 1400 0000 7215 0000 0072 1600 0000  .r....r....r....
-00002bf0: da16 7079 7879 3364 2e73 6573 7369 6f6e  ..pyxy3d.session
-00002c00: 2e73 6573 7369 6f6e 7217 0000 0072 1800  .sessionr....r..
-00002c10: 0000 5a15 7079 7879 3364 2e67 7569 2e6c  ..Z.pyxy3d.gui.l
-00002c20: 6f67 5f77 6964 6765 7472 1900 0000 da13  og_widgetr......
-00002c30: 7079 7879 3364 2e63 6f6e 6669 6775 7261  pyxy3d.configura
-00002c40: 746f 7272 1a00 0000 da1d 7079 7879 3364  torr......pyxy3d
-00002c50: 2e67 7569 2e63 616c 6962 7261 7469 6f6e  .gui.calibration
-00002c60: 5f77 6964 6765 7472 1b00 0000 da19 7079  _widgetr......py
-00002c70: 7879 3364 2e67 7569 2e63 6861 7275 636f  xy3d.gui.charuco
-00002c80: 5f77 6964 6765 7472 1c00 0000 da35 7079  _widgetr.....5py
-00002c90: 7879 3364 2e67 7569 2e63 616d 6572 615f  xy3d.gui.camera_
-00002ca0: 636f 6e66 6967 2e69 6e74 7269 6e73 6963  config.intrinsic
-00002cb0: 5f63 616c 6962 7261 7469 6f6e 5f77 6964  _calibration_wid
-00002cc0: 6765 7472 1d00 0000 5a2a 7079 7879 3364  getr....Z*pyxy3d
-00002cd0: 2e67 7569 2e63 616c 6962 7261 7465 5f63  .gui.calibrate_c
-00002ce0: 6170 7475 7265 5f76 6f6c 756d 655f 7769  apture_volume_wi
-00002cf0: 6467 6574 721e 0000 00da 1b70 7978 7933  dgetr......pyxy3
-00002d00: 642e 6775 692e 7265 636f 7264 696e 675f  d.gui.recording_
-00002d10: 7769 6467 6574 721f 0000 005a 2170 7978  widgetr....Z!pyx
-00002d20: 7933 642e 6775 692e 706f 7374 5f70 726f  y3d.gui.post_pro
-00002d30: 6365 7373 696e 675f 7769 6467 6574 7220  cessing_widgetr 
-00002d40: 0000 0072 2100 0000 7230 0000 0072 a100  ...r!...r0...r..
-00002d50: 0000 72aa 0000 0072 2e00 0000 722e 0000  ..r....r....r...
-00002d60: 0072 2e00 0000 722f 0000 00da 083c 6d6f  .r....r/.....<mo
-00002d70: 6475 6c65 3e01 0000 0073 4000 0000 0800  dule>....s@.....
-00002d80: 0801 0c02 1402 0c02 0c01 0c01 0801 2c01  ..............,.
-00002d90: 080b 0c01 1801 0c01 1401 1001 0c01 0c01  ................
-00002da0: 0c01 0c01 0c01 0c03 0c01 0c01 1003 1008  ................
-00002db0: 007f 007f 1033 0814 0808 0a01 04ff       .....3........
+00000160: 6d32 5a32 0100 4700 6412 6413 8400 6413  m2Z2..G.d.d...d.
+00000170: 6517 8303 5a33 4700 6414 6415 8400 6415  e...Z3G.d.d...d.
+00000180: 6506 8303 5a34 4700 6416 6417 8400 6417  e...Z4G.d.d...d.
+00000190: 6514 8303 5a35 6418 6419 8400 5a36 6504  e...Z5d.d...Z6e.
+000001a0: 641a 6b02 72c1 6536 8300 0100 6401 5300  d.k.r.e6....d.S.
+000001b0: 6401 5300 291b e900 0000 004e 2903 da0b  d.S.)......N)...
+000001c0: 514d 6169 6e57 696e 646f 77da 0e51 5374  QMainWindow..QSt
+000001d0: 6163 6b65 644c 6179 6f75 74da 0b51 4669  ackedLayout..QFi
+000001e0: 6c65 4469 616c 6f67 2901 da04 5061 7468  leDialog)...Path
+000001f0: 2901 da06 5468 7265 6164 2909 da0c 5141  )...Thread)...QA
+00000200: 7070 6c69 6361 7469 6f6e 7202 0000 0072  pplicationr....r
+00000210: 0300 0000 da07 5157 6964 6765 74da 0b51  ......QWidget..Q
+00000220: 446f 636b 5769 6467 6574 da0b 5156 426f  DockWidget..QVBo
+00000230: 784c 6179 6f75 74da 0551 4d65 6e75 da08  xLayout..QMenu..
+00000240: 514d 656e 7542 6172 da0a 5154 6162 5769  QMenuBar..QTabWi
+00000250: 6467 6574 2901 da04 456e 756d 2904 da05  dget)...Enum)...
+00000260: 5149 636f 6eda 0751 4163 7469 6f6e da0c  QIcon..QAction..
+00000270: 514b 6579 5365 7175 656e 6365 da09 5153  QKeySequence..QS
+00000280: 686f 7274 6375 7429 01da 0251 7429 03da  hortcut)...Qt)..
+00000290: 085f 5f72 6f6f 745f 5fda 115f 5f73 6574  .__root__..__set
+000002a0: 7469 6e67 735f 7061 7468 5f5f da0c 5f5f  tings_path__..__
+000002b0: 7573 6572 5f64 6972 5f5f 2902 da07 5365  user_dir__)...Se
+000002c0: 7373 696f 6eda 0b53 6573 7369 6f6e 4d6f  ssion..SessionMo
+000002d0: 6465 2901 da09 4c6f 6757 6964 6765 7429  de)...LogWidget)
+000002e0: 01da 0c43 6f6e 6669 6775 7261 746f 7229  ...Configurator)
+000002f0: 01da 0d43 6861 7275 636f 5769 6467 6574  ...CharucoWidget
+00000300: 2901 da1a 496e 7472 696e 7369 6343 616c  )...IntrinsicCal
+00000310: 6962 7261 7469 6f6e 5769 6467 6574 2901  ibrationWidget).
+00000320: da1c 4361 6c69 6272 6174 6543 6170 7475  ..CalibrateCaptu
+00000330: 7265 566f 6c75 6d65 5769 6467 6574 2901  reVolumeWidget).
+00000340: da0f 5265 636f 7264 696e 6757 6964 6765  ..RecordingWidge
+00000350: 7429 01da 1450 6f73 7450 726f 6365 7373  t)...PostProcess
+00000360: 696e 6757 6964 6765 7463 0000 0000 0000  ingWidgetc......
+00000370: 0000 0000 0000 0000 0000 0100 0000 4000  ..............@.
+00000380: 0000 7320 0000 0065 005a 0164 005a 0264  ..s ...e.Z.d.Z.d
+00000390: 015a 0364 025a 0464 035a 0564 045a 0664  .Z.d.Z.d.Z.d.Z.d
+000003a0: 055a 0764 0653 0029 07da 0854 6162 496e  .Z.d.S.)...TabIn
+000003b0: 6465 7872 0100 0000 e901 0000 00e9 0200  dexr............
+000003c0: 0000 e903 0000 00e9 0400 0000 4e29 08da  ............N)..
+000003d0: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
+000003e0: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
+000003f0: 655f 5fda 0743 6861 7275 636f da07 4361  e__..Charuco..Ca
+00000400: 6d65 7261 73da 0d43 6170 7475 7265 566f  meras..CaptureVo
+00000410: 6c75 6d65 da09 5265 636f 7264 696e 67da  lume..Recording.
+00000420: 0a50 726f 6365 7373 696e 67a9 0072 2d00  .Processing..r-.
+00000430: 0000 722d 0000 00fa 3a43 3a5c 5573 6572  ..r-....:C:\User
+00000440: 735c 4d61 6320 5072 6962 6c65 5c72 6570  s\Mac Prible\rep
+00000450: 6f73 5c70 7978 7933 645c 7079 7879 3364  os\pyxy3d\pyxy3d
+00000460: 5c67 7569 5c6d 6169 6e5f 7769 6467 6574  \gui\main_widget
+00000470: 2e70 7972 2000 0000 2800 0000 730c 0000  .pyr ...(...s...
+00000480: 0008 0004 0104 0104 0104 0108 0172 2000  .............r .
+00000490: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+000004a0: 0000 0003 0000 0000 0000 0073 b000 0000  ...........s....
+000004b0: 6500 5a01 6400 5a02 8700 6601 6401 6402  e.Z.d.Z...f.d.d.
+000004c0: 8408 5a03 6403 6404 8400 5a04 6405 6406  ..Z.d.d...Z.d.d.
+000004d0: 8400 5a05 6407 6408 8400 5a06 6409 640a  ..Z.d.d...Z.d.d.
+000004e0: 8400 5a07 640b 640c 8400 5a08 640d 6509  ..Z.d.d...Z.d.e.
+000004f0: 6602 640e 640f 8404 5a0a 6410 6411 8400  f.d.d...Z.d.d...
+00000500: 5a0b 6412 6413 8400 5a0c 6414 6415 8400  Z.d.d...Z.d.d...
+00000510: 5a0d 6416 6417 8400 5a0e 6418 6419 8400  Z.d.d...Z.d.d...
+00000520: 5a0f 641a 641b 8400 5a10 641c 6509 6602  Z.d.d...Z.d.e.f.
+00000530: 641d 641e 8404 5a11 641f 6420 8400 5a12  d.d...Z.d.d ..Z.
+00000540: 6421 6422 8400 5a13 6423 6424 8400 5a14  d!d"..Z.d#d$..Z.
+00000550: 6425 6426 8400 5a15 8700 0400 5a16 5300  d%d&..Z.....Z.S.
+00000560: 2927 da0a 4d61 696e 5769 6e64 6f77 6301  )'..MainWindowc.
+00000570: 0000 0000 0000 0000 0000 0002 0000 0007  ................
+00000580: 0000 0003 0000 0073 aa01 0000 7400 7401  .......s....t.t.
+00000590: 7c00 8302 a002 a100 0100 7403 a004 7405  |.........t...t.
+000005a0: a101 7c00 5f06 7c00 a007 6401 a101 0100  ..|._.|...d.....
+000005b0: 7c00 a008 7409 740a 740b 740c 6402 8302  |...t.t.t.t.d...
+000005c0: 8301 8301 a101 0100 7c00 a00d 6403 6403  ........|...d.d.
+000005d0: a102 0100 7c00 a00e a100 7c00 5f0f 7c00  ....|.....|._.|.
+000005e0: 6a0f a010 6404 a101 7c00 5f11 7412 6405  j...d...|._.t.d.
+000005f0: 7c00 8302 7c00 5f13 7c00 6a13 6a14 a015  |...|._.|.j.j...
+00000600: 7c00 6a16 a101 0100 7c00 6a11 a017 7c00  |.j.....|.j...|.
+00000610: 6a13 a101 0100 7418 6406 7c00 8302 7c00  j.....t.d.|...|.
+00000620: 5f19 741a 7c00 6a06 6407 1900 8301 4400  _.t.|.j.d.....D.
+00000630: 5d07 7d01 7c00 a01b 7c01 a101 0100 7152  ].}.|...|.....qR
+00000640: 7c00 6a11 a010 7c00 6a19 a101 0100 7412  |.j...|.j.....t.
+00000650: 6408 7c00 8302 7c00 5f1c 7c00 6a11 a017  d.|...|._.|.j...
+00000660: 7c00 6a1c a101 0100 7c00 6a0f a010 6409  |.j.....|.j...d.
+00000670: a101 7c00 5f1d 7412 640a 7c00 8302 7c00  ..|._.t.d.|...|.
+00000680: 5f1e 7c00 6a1d a017 7c00 6a1e a101 0100  _.|.j...|.j.....
+00000690: 7c00 6a1e a01f 640b a101 0100 7412 640c  |.j...d.....t.d.
+000006a0: 7c00 8302 7c00 5f20 7c00 6a1d a017 7c00  |...|._ |.j...|.
+000006b0: 6a20 a101 0100 7c00 6a20 a01f 640b a101  j ....|.j ..d...
+000006c0: 0100 7c00 a021 a100 0100 7422 8300 7c00  ..|..!....t"..|.
+000006d0: 5f23 7c00 a024 7c00 6a23 a101 0100 7425  _#|..$|.j#....t%
+000006e0: 640d 7c00 8302 7c00 5f26 7c00 6a26 a027  d.|...|._&|.j&.'
+000006f0: 7425 6a28 6a29 a101 0100 7c00 6a26 a02a  t%j(j)....|.j&.*
+00000700: 742b 6a2c 6a2d a101 0100 742e 8300 7c00  t+j,j-....t...|.
+00000710: 5f2f 7c00 6a26 a030 7c00 6a2f a101 0100  _/|.j&.0|.j/....
+00000720: 7c00 a031 742b 6a2c 6a2d 7c00 6a26 a102  |..1t+j,j-|.j&..
+00000730: 0100 6400 5300 290e 4e5a 0650 7978 7933  ..d.S.).NZ.Pyxy3
+00000740: 447a 1e70 7978 7933 642f 6775 692f 6963  Dz.pyxy3d/gui/ic
+00000750: 6f6e 732f 7079 7879 5f6c 6f67 6f2e 7376  ons/pyxy_logo.sv
+00000760: 6769 f401 0000 5a04 4669 6c65 7a10 4e65  gi....Z.Filez.Ne
+00000770: 772f 4f70 656e 2050 726f 6a65 6374 7a12  w/Open Projectz.
+00000780: 5265 6365 6e74 2050 726f 6a65 6374 732e  Recent Projects.
+00000790: 2e2e da0f 7265 6365 6e74 5f70 726f 6a65  ....recent_proje
+000007a0: 6374 735a 0445 7869 7472 2900 0000 7a0f  ctsZ.Exitr)...z.
+000007b0: 436f 6e6e 6563 7420 4361 6d65 7261 7346  Connect CamerasF
+000007c0: 7a12 4469 7363 6f6e 6e65 6374 2043 616d  z.Disconnect Cam
+000007d0: 6572 6173 5a03 4c6f 6729 32da 0573 7570  erasZ.Log)2..sup
+000007e0: 6572 722f 0000 00da 085f 5f69 6e69 745f  err/.....__init_
+000007f0: 5fda 0474 6f6d 6cda 046c 6f61 6472 1500  _..toml..loadr..
+00000800: 0000 da0c 6170 705f 7365 7474 696e 6773  ....app_settings
+00000810: da0e 7365 7457 696e 646f 7754 6974 6c65  ..setWindowTitle
+00000820: 5a0d 7365 7457 696e 646f 7749 636f 6e72  Z.setWindowIconr
+00000830: 0f00 0000 da03 7374 7272 0500 0000 7214  ......strr....r.
+00000840: 0000 005a 0e73 6574 4d69 6e69 6d75 6d53  ...Z.setMinimumS
+00000850: 697a 655a 076d 656e 7542 6172 5a04 6d65  izeZ.menuBarZ.me
+00000860: 6e75 5a07 6164 644d 656e 755a 0966 696c  nuZ.addMenuZ.fil
+00000870: 655f 6d65 6e75 7210 0000 005a 136f 7065  e_menur....Z.ope
+00000880: 6e5f 7072 6f6a 6563 745f 6163 7469 6f6e  n_project_action
+00000890: da09 7472 6967 6765 7265 64da 0763 6f6e  ..triggered..con
+000008a0: 6e65 6374 da19 6372 6561 7465 5f6e 6577  nect..create_new
+000008b0: 5f70 726f 6a65 6374 5f66 6f6c 6465 72da  _project_folder.
+000008c0: 0961 6464 4163 7469 6f6e 720b 0000 00da  .addActionr.....
+000008d0: 1b6f 7065 6e5f 7265 6365 6e74 5f70 726f  .open_recent_pro
+000008e0: 6a65 6374 5f73 7562 6d65 6e75 da08 7265  ject_submenu..re
+000008f0: 7665 7273 6564 da15 6164 645f 746f 5f72  versed..add_to_r
+00000900: 6563 656e 745f 7072 6f6a 6563 74da 1265  ecent_project..e
+00000910: 7869 745f 7079 7879 3364 5f61 6374 696f  xit_pyxy3d_actio
+00000920: 6e5a 0c63 616d 6572 6173 5f6d 656e 75da  nZ.cameras_menu.
+00000930: 1663 6f6e 6e65 6374 5f63 616d 6572 6173  .connect_cameras
+00000940: 5f61 6374 696f 6eda 0a73 6574 456e 6162  _action..setEnab
+00000950: 6c65 64da 1964 6973 636f 6e6e 6563 745f  led..disconnect_
+00000960: 6361 6d65 7261 735f 6163 7469 6f6e da14  cameras_action..
+00000970: 636f 6e6e 6563 745f 6d65 6e75 5f61 6374  connect_menu_act
+00000980: 696f 6e73 720d 0000 00da 0a74 6162 5f77  ionsr......tab_w
+00000990: 6964 6765 745a 1073 6574 4365 6e74 7261  idgetZ.setCentra
+000009a0: 6c57 6964 6765 7472 0900 0000 5a0d 646f  lWidgetr....Z.do
+000009b0: 636b 6564 5f6c 6f67 6765 725a 0b73 6574  cked_loggerZ.set
+000009c0: 4665 6174 7572 6573 5a11 446f 636b 5769  FeaturesZ.DockWi
+000009d0: 6467 6574 4665 6174 7572 655a 1144 6f63  dgetFeatureZ.Doc
+000009e0: 6b57 6964 6765 744d 6f76 6162 6c65 5a0f  kWidgetMovableZ.
+000009f0: 7365 7441 6c6c 6f77 6564 4172 6561 7372  setAllowedAreasr
+00000a00: 1300 0000 5a0e 446f 636b 5769 6467 6574  ....Z.DockWidget
+00000a10: 4172 6561 5a14 426f 7474 6f6d 446f 636b  AreaZ.BottomDock
+00000a20: 5769 6467 6574 4172 6561 7219 0000 005a  WidgetArear....Z
+00000a30: 0a6c 6f67 5f77 6964 6765 745a 0973 6574  .log_widgetZ.set
+00000a40: 5769 6467 6574 5a0d 6164 6444 6f63 6b57  WidgetZ.addDockW
+00000a50: 6964 6765 7429 02da 0473 656c 66da 0c70  idget)...self..p
+00000a60: 726f 6a65 6374 5f70 6174 68a9 01da 095f  roject_path...._
+00000a70: 5f63 6c61 7373 5f5f 722d 0000 0072 2e00  _class__r-...r..
+00000a80: 0000 7232 0000 0031 0000 0073 4000 0000  ..r2...1...s@...
+00000a90: 0e01 0c02 0a02 1801 0c01 0a03 0e01 0c03  ................
+00000aa0: 1001 0e01 0c03 1203 0c01 0e02 0c02 0e01  ................
+00000ab0: 0e02 0c01 0e01 0c01 0c02 0e01 0c01 0802  ................
+00000ac0: 0803 0c02 0c03 1001 1001 0801 0e01 1602  ................
+00000ad0: 7a13 4d61 696e 5769 6e64 6f77 2e5f 5f69  z.MainWindow.__i
+00000ae0: 6e69 745f 5f63 0100 0000 0000 0000 0000  nit__c..........
+00000af0: 0000 0100 0000 0400 0000 4300 0000 7338  ..........C...s8
+00000b00: 0000 007c 006a 006a 01a0 027c 006a 03a1  ...|.j.j...|.j..
+00000b10: 0101 007c 006a 046a 01a0 0274 05a0 06a1  ...|.j.j...t....
+00000b20: 006a 07a1 0101 007c 006a 086a 01a0 027c  .j.....|.j.j...|
+00000b30: 006a 09a1 0101 0064 0053 00a9 014e 290a  .j.....d.S...N).
+00000b40: 7240 0000 0072 3800 0000 7239 0000 00da  r@...r8...r9....
+00000b50: 116c 6f61 645f 7374 7265 616d 5f74 6f6f  .load_stream_too
+00000b60: 6c73 723f 0000 0072 0700 0000 da08 696e  lsr?...r......in
+00000b70: 7374 616e 6365 da04 7175 6974 7242 0000  stance..quitrB..
+00000b80: 00da 1264 6973 636f 6e6e 6563 745f 6361  ...disconnect_ca
+00000b90: 6d65 7261 73a9 0172 4500 0000 722d 0000  meras..rE...r-..
+00000ba0: 0072 2d00 0000 722e 0000 0072 4300 0000  .r-...r....rC...
+00000bb0: 6a00 0000 7306 0000 0010 0114 0114 017a  j...s..........z
+00000bc0: 1f4d 6169 6e57 696e 646f 772e 636f 6e6e  .MainWindow.conn
+00000bd0: 6563 745f 6d65 6e75 5f61 6374 696f 6e73  ect_menu_actions
+00000be0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00000bf0: 0004 0000 0043 0000 0073 b400 0000 7c00  .....C...s....|.
+00000c00: 6a00 a001 7c00 6a02 a101 0100 7c00 6a00  j...|.j.....|.j.
+00000c10: a003 7404 6a05 6a06 6401 a102 0100 7c00  ..t.j.j.d.....|.
+00000c20: 6a00 a003 7404 6a07 6a06 6402 a102 0100  j...t.j.j.d.....
+00000c30: 7c00 6a00 a003 7404 6a08 6a06 6402 a102  |.j...t.j.j.d...
+00000c40: 0100 7c00 6a00 a003 7404 6a09 6a06 6402  ..|.j...t.j.j.d.
+00000c50: a102 0100 7c00 6a00 a003 7404 6a0a 6a06  ....|.j...t.j.j.
+00000c60: 6401 a102 0100 740b 8300 7c00 5f0c 740b  d.....t...|._.t.
+00000c70: 8300 7c00 5f0d 740b 8300 7c00 5f0e 7c00  ..|._.t...|._.|.
+00000c80: 6a0f a010 7411 6a05 a101 0100 7c00 6a0f  j...t.j.....|.j.
+00000c90: a012 a100 0100 7c00 6a13 a014 6402 a101  ......|.j...d...
+00000ca0: 0100 7c00 6a15 a014 6401 a101 0100 6400  ..|.j...d.....d.
+00000cb0: 5300 2903 4e54 4629 1672 4400 0000 5a10  S.).NTF).rD...Z.
+00000cc0: 7365 7443 7572 7265 6e74 5769 6467 6574  setCurrentWidget
+00000cd0: da0e 6368 6172 7563 6f5f 7769 6467 6574  ..charuco_widget
+00000ce0: da0d 7365 7454 6162 456e 6162 6c65 6472  ..setTabEnabledr
+00000cf0: 2000 0000 7228 0000 00da 0576 616c 7565   ...r(.....value
+00000d00: 7229 0000 0072 2a00 0000 722b 0000 0072  r)...r*...r+...r
+00000d10: 2c00 0000 7208 0000 00da 0d63 616d 6572  ,...r......camer
+00000d20: 615f 7769 6467 6574 da1f 6361 6c69 6272  a_widget..calibr
+00000d30: 6174 655f 6361 7074 7572 655f 766f 6c75  ate_capture_volu
+00000d40: 6d65 5f77 6964 6765 74da 1072 6563 6f72  me_widget..recor
+00000d50: 6469 6e67 5f77 6964 6765 74da 0773 6573  ding_widget..ses
+00000d60: 7369 6f6e da08 7365 745f 6d6f 6465 7218  sion..set_moder.
+00000d70: 0000 0072 4d00 0000 7242 0000 0072 4100  ...rM...rB...rA.
+00000d80: 0000 7240 0000 0072 4e00 0000 722d 0000  ..r@...rN...r-..
+00000d90: 0072 2d00 0000 722e 0000 0072 4d00 0000  .r-...r....rM...
+00000da0: 6f00 0000 731a 0000 000e 0112 0112 0112  o...s...........
+00000db0: 0112 0112 0108 0208 0108 010e 020a 010c  ................
+00000dc0: 0110 017a 1d4d 6169 6e57 696e 646f 772e  ...z.MainWindow.
+00000dd0: 6469 7363 6f6e 6e65 6374 5f63 616d 6572  disconnect_camer
+00000de0: 6173 6301 0000 0000 0000 0000 0000 0001  asc.............
+00000df0: 0000 0003 0000 0043 0000 0073 2200 0000  .......C...s"...
+00000e00: 7400 a001 6401 a101 0100 7c00 6a02 a003  t...d.....|.j...
+00000e10: a100 0100 7c00 6a02 a004 a100 0100 6400  ....|.j.......d.
+00000e20: 5300 2902 4e7a 5550 6175 7369 6e67 2061  S.).NzUPausing a
+00000e30: 6c6c 2066 7261 6d65 2072 6561 6469 6e67  ll frame reading
+00000e40: 2061 7420 6c6f 6164 206f 6620 7374 7265   at load of stre
+00000e50: 616d 2074 6f6f 6c73 3b20 7368 6f75 6c64  am tools; should
+00000e60: 2062 6520 6f6e 2063 6861 7275 636f 2074   be on charuco t
+00000e70: 6162 2072 6967 6874 206e 6f77 2905 da06  ab right now)...
+00000e80: 6c6f 6767 6572 da04 696e 666f 7255 0000  logger..inforU..
+00000e90: 00da 1970 6175 7365 5f61 6c6c 5f6d 6f6e  ...pause_all_mon
+00000ea0: 6f63 616c 6962 7261 746f 7273 da12 7061  ocalibrators..pa
+00000eb0: 7573 655f 7379 6e63 6872 6f6e 697a 6572  use_synchronizer
+00000ec0: 724e 0000 0072 2d00 0000 722d 0000 0072  rN...r-...r-...r
+00000ed0: 2e00 0000 da17 7061 7573 655f 616c 6c5f  ......pause_all_
+00000ee0: 6672 616d 655f 7265 6164 696e 6780 0000  frame_reading...
+00000ef0: 0073 0600 0000 0a01 0a01 0e01 7a22 4d61  .s..........z"Ma
+00000f00: 696e 5769 6e64 6f77 2e70 6175 7365 5f61  inWindow.pause_a
+00000f10: 6c6c 5f66 7261 6d65 5f72 6561 6469 6e67  ll_frame_reading
+00000f20: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00000f30: 0005 0000 0043 0000 0073 4c00 0000 7c00  .....C...sL...|.
+00000f40: 6a00 a001 6401 a101 0100 7c00 6a02 a001  j...d.....|.j...
+00000f50: 6402 a101 0100 7c00 6a03 6a04 6a05 a006  d.....|.j.j.j...
+00000f60: 7c00 6a07 a101 0100 7408 7c00 6a03 6a09  |.j.....t.|.j.j.
+00000f70: 6403 6402 6404 8d03 7c00 5f0a 7c00 6a0a  d.d.d...|._.|.j.
+00000f80: a00b a100 0100 6400 5300 2905 4e46 5472  ......d.S.).NFTr
+00000f90: 2d00 0000 2903 da06 7461 7267 6574 da04  -...)...target..
+00000fa0: 6172 6773 da06 6461 656d 6f6e 290c 7240  args..daemon).r@
+00000fb0: 0000 0072 4100 0000 7242 0000 0072 5500  ...rA...rB...rU.
+00000fc0: 0000 da0b 7174 5f73 6967 6e61 6c65 72da  ....qt_signaler.
+00000fd0: 1a73 7472 6561 6d5f 746f 6f6c 735f 6c6f  .stream_tools_lo
+00000fe0: 6164 6564 5f73 6967 6e61 6c72 3900 0000  aded_signalr9...
+00000ff0: 725b 0000 0072 0600 0000 724a 0000 00da  r[...r....rJ....
+00001000: 0674 6872 6561 64da 0573 7461 7274 724e  .thread..startrN
+00001010: 0000 0072 2d00 0000 722d 0000 0072 2e00  ...r-...r-...r..
+00001020: 0000 724a 0000 0085 0000 0073 0e00 0000  ..rJ.......s....
+00001030: 0c01 0c01 1201 0201 0a01 08ff 0e03 7a1c  ..............z.
+00001040: 4d61 696e 5769 6e64 6f77 2e6c 6f61 645f  MainWindow.load_
+00001050: 7374 7265 616d 5f74 6f6f 6c73 6302 0000  stream_toolsc...
+00001060: 0000 0000 0000 0000 0002 0000 0006 0000  ................
+00001070: 0043 0000 0073 4401 0000 7400 a001 6401  .C...sD...t...d.
+00001080: 7c01 9b00 9d02 a101 0100 7c01 0400 7402  |.........|...t.
+00001090: 6a03 6a04 6b02 721e 0100 7400 a001 6402  j.j.k.r...t...d.
+000010a0: a101 0100 7c00 6a05 a006 7407 6a03 a101  ....|.j...t.j...
+000010b0: 0100 6400 5300 0400 7402 6a08 6a04 6b02  ..d.S...t.j.j.k.
+000010c0: 7233 0100 7400 a001 6403 a101 0100 7c00  r3..t...d.....|.
+000010d0: 6a05 a006 7407 6a09 a101 0100 6400 5300  j...t.j.....d.S.
+000010e0: 0400 7402 6a0a 6a04 6b02 725c 0100 7400  ..t.j.j.k.r\..t.
+000010f0: a001 6404 a101 0100 7c00 6a05 a00b a100  ..d.....|.j.....
+00001100: 7250 7400 a001 6405 a101 0100 7c00 6a0c  rPt...d.....|.j.
+00001110: a00d a100 0100 6400 5300 7400 a001 6406  ......d.S.t...d.
+00001120: a101 0100 7c00 6a0c a00e a100 0100 6400  ....|.j.......d.
+00001130: 5300 0400 7402 6a0f 6a04 6b02 7288 0100  S...t.j.j.k.r...
+00001140: 7400 a001 6407 a101 0100 7a0d 7400 a001  t...d.....z.t...
+00001150: 6408 a101 0100 7c00 6a0c 6a10 a011 a100  d.....|.j.j.....
+00001160: 0100 5700 6e09 0100 0100 0100 7400 a001  ..W.n.......t...
+00001170: 6409 a101 0100 5900 7c00 6a05 a006 7407  d.....Y.|.j...t.
+00001180: 6a0f a101 0100 6400 5300 7402 6a12 6a04  j.....d.S.t.j.j.
+00001190: 6b02 72a0 7400 a001 640a a101 0100 7c00  k.r.t...d.....|.
+000011a0: 6a05 a006 7407 6a13 a101 0100 7c00 6a14  j...t.j.....|.j.
+000011b0: a015 a100 0100 6400 5300 6400 5300 290b  ......d.S.d.S.).
+000011c0: 4e7a 1d53 7769 7463 6869 6e67 206d 6169  Nz.Switching mai
+000011d0: 6e20 7769 6e64 6f77 2074 6f20 7461 6220  n window to tab 
+000011e0: 7a19 4163 7469 7661 7469 6e67 2043 6861  z.Activating Cha
+000011f0: 7275 636f 2057 6964 6765 747a 1e41 6374  ruco Widgetz.Act
+00001200: 6976 6174 696e 6720 4361 6d65 7261 2053  ivating Camera S
+00001210: 6574 7570 2057 6964 6765 747a 2a41 6374  etup Widgetz*Act
+00001220: 6976 6174 696e 6720 4361 6c69 6272 6174  ivating Calibrat
+00001230: 6520 4361 7074 7572 6520 566f 6c75 6d65  e Capture Volume
+00001240: 2057 6964 6765 747a 5353 6573 7369 6f6e   WidgetzSSession
+00001250: 2069 7320 656c 6967 6962 6c65 2066 6f72   is eligible for
+00001260: 2073 6574 7469 6e67 206f 6620 6f72 6967   setting of orig
+00001270: 696e 2e2e 2e61 6374 6976 6174 696e 6720  in...activating 
+00001280: 6361 7074 7572 6520 766f 6c75 6d65 206f  capture volume o
+00001290: 7269 6769 6e20 7769 6467 6574 7a57 5365  rigin widgetzWSe
+000012a0: 7373 696f 6e20 6973 206e 6f74 2065 6c69  ssion is not eli
+000012b0: 6769 626c 6520 666f 7220 7365 7474 696e  gible for settin
+000012c0: 6720 6f66 206f 7269 6769 6e2e 2e2e 6163  g of origin...ac
+000012d0: 7469 7661 7469 6e67 2065 7874 7269 6e73  tivating extrins
+000012e0: 6963 2063 616c 6962 7261 7469 6f6e 2077  ic calibration w
+000012f0: 6964 6765 747a 1741 6374 6976 6174 6520  idgetz.Activate 
+00001300: 5265 636f 7264 696e 6720 4d6f 6465 7a38  Recording Modez8
+00001310: 4174 7465 6d70 7469 6e67 2074 6f20 7370  Attempting to sp
+00001320: 696e 2064 6f77 6e20 7468 6520 6578 7472  in down the extr
+00001330: 696e 7369 6320 6361 6c69 6272 6174 696f  insic calibratio
+00001340: 6e20 7769 6467 6574 7a32 4e6f 2065 7874  n widgetz2No ext
+00001350: 7269 6e73 6963 2063 616c 6962 7261 7469  rinsic calibrati
+00001360: 6f6e 2063 616c 6962 7261 7469 6f6e 2077  on calibration w
+00001370: 6964 6765 7420 6578 6973 7473 7a18 4163  idget existsz.Ac
+00001380: 7469 7661 7465 2050 726f 6365 7373 696e  tivate Processin
+00001390: 6720 4d6f 6465 2916 7257 0000 0072 5800  g Mode).rW...rX.
+000013a0: 0000 7220 0000 0072 2800 0000 7251 0000  ..r ...r(...rQ..
+000013b0: 0072 5500 0000 7256 0000 0072 1800 0000  .rU...rV...r....
+000013c0: 7229 0000 00da 1449 6e74 7269 6e73 6963  r).....Intrinsic
+000013d0: 4361 6c69 6272 6174 696f 6e72 2a00 0000  Calibrationr*...
+000013e0: da1a 6973 5f63 6170 7475 7265 5f76 6f6c  ..is_capture_vol
+000013f0: 756d 655f 656c 6967 6962 6c65 7253 0000  ume_eligiblerS..
+00001400: 005a 1e61 6374 6976 6174 655f 6361 7074  .Z.activate_capt
+00001410: 7572 655f 766f 6c75 6d65 5f77 6964 6765  ure_volume_widge
+00001420: 745a 2561 6374 6976 6174 655f 6578 7472  tZ%activate_extr
+00001430: 696e 7369 635f 6361 6c69 6272 6174 696f  insic_calibratio
+00001440: 6e5f 7769 6467 6574 722b 0000 005a 1c65  n_widgetr+...Z.e
+00001450: 7874 7269 6e73 6963 5f63 616c 6962 7261  xtrinsic_calibra
+00001460: 7469 6f6e 5f77 6964 6765 745a 1073 6875  tion_widgetZ.shu
+00001470: 7464 6f77 6e5f 7468 7265 6164 7372 2c00  tdown_threadsr,.
+00001480: 0000 da0e 506f 7374 5072 6f63 6573 7369  ....PostProcessi
+00001490: 6e67 da11 7072 6f63 6573 7369 6e67 5f77  ng..processing_w
+000014a0: 6964 6765 745a 1875 7064 6174 655f 7265  idgetZ.update_re
+000014b0: 636f 7264 696e 675f 666f 6c64 6572 73a9  cording_folders.
+000014c0: 0272 4500 0000 da05 696e 6465 7872 2d00  .rE.....indexr-.
+000014d0: 0000 722d 0000 0072 2e00 0000 da0e 6f6e  ..r-...r......on
+000014e0: 5f74 6162 5f63 6861 6e67 6564 9000 0000  _tab_changed....
+000014f0: 7338 0000 0010 0102 010e 010a 0112 020e  s8..............
+00001500: 010a 0112 020e 010a 010a 020a 010e 010a  ................
+00001510: 020e 010e 020a 0102 020a 0110 0106 010c  ................
+00001520: 0112 020a 010a 010e 020e 0204 fb7a 194d  .............z.M
+00001530: 6169 6e57 696e 646f 772e 6f6e 5f74 6162  ainWindow.on_tab
+00001540: 5f63 6861 6e67 6564 da0e 7061 7468 5f74  _changed..path_t
+00001550: 6f5f 666f 6c64 6572 6302 0000 0000 0000  o_folderc.......
+00001560: 0000 0000 0004 0000 0004 0000 0043 0000  .............C..
+00001570: 0073 f000 0000 7400 7c01 8301 7d02 7401  .s....t.|...}.t.
+00001580: 7c02 8301 7c00 5f02 7403 a004 6401 7c02  |...|._.t...d.|.
+00001590: 9b00 9d02 a101 0100 7405 7c00 6a02 8301  ........t.|.j...
+000015a0: 7c00 5f06 7407 7c00 6a06 8301 7c00 5f08  |._.t.|.j...|._.
+000015b0: 7409 8300 7c00 5f0a 7409 8300 7c00 5f0b  t...|._.t...|._.
+000015c0: 7409 8300 7c00 5f0c 7409 8300 7c00 5f0d  t...|._.t...|._.
+000015d0: 7c00 6a0e a00f 7c00 6a08 6402 a102 0100  |.j...|.j.d.....
+000015e0: 7c00 6a0e a00f 7c00 6a0a 6403 a102 0100  |.j...|.j.d.....
+000015f0: 7c00 6a0e a00f 7c00 6a0d 6404 a102 0100  |.j...|.j.d.....
+00001600: 7c00 6a0e a00f 7c00 6a0b 6405 a102 0100  |.j...|.j.d.....
+00001610: 7c00 6a0e a00f 7c00 6a0c 6406 a102 0100  |.j...|.j.d.....
+00001620: 7c00 6a0e 6a10 a011 7c00 6a12 a101 0100  |.j.j...|.j.....
+00001630: 7c00 6a13 a014 6407 a101 0100 7c00 a015  |.j...d.....|...
+00001640: a100 0100 7c00 6a0e a016 a100 7d03 7c00  ....|.j.....}.|.
+00001650: 6a0e a017 7c03 a101 0100 7c00 a018 a100  j...|.....|.....
+00001660: 0100 6400 5300 2908 4e7a 2d4c 6175 6e63  ..d.S.).Nz-Launc
+00001670: 6869 6e67 2073 6573 7369 6f6e 2077 6974  hing session wit
+00001680: 6820 636f 6e66 6967 2066 696c 6520 7374  h config file st
+00001690: 6f72 6564 2069 6e20 7228 0000 0072 2900  ored in r(...r).
+000016a0: 0000 722a 0000 0072 2b00 0000 722c 0000  ..r*...r+...r,..
+000016b0: 0054 2919 7205 0000 0072 1a00 0000 da06  .T).r....r......
+000016c0: 636f 6e66 6967 7257 0000 0072 5800 0000  configrW...rX...
+000016d0: 7217 0000 0072 5500 0000 721b 0000 0072  r....rU...r....r
+000016e0: 4f00 0000 7208 0000 0072 5200 0000 7254  O...r....rR...rT
+000016f0: 0000 0072 6600 0000 7253 0000 0072 4400  ...rf...rS...rD.
+00001700: 0000 5a06 6164 6454 6162 5a0e 6375 7272  ..Z.addTabZ.curr
+00001710: 656e 7443 6861 6e67 6564 7239 0000 0072  entChangedr9...r
+00001720: 6900 0000 7240 0000 0072 4100 0000 da0b  i...r@...rA.....
+00001730: 7570 6461 7465 5f74 6162 735a 0c63 7572  update_tabsZ.cur
+00001740: 7265 6e74 496e 6465 785a 0f73 6574 4375  rentIndexZ.setCu
+00001750: 7272 656e 7449 6e64 6578 da17 636f 6e6e  rrentIndex..conn
+00001760: 6563 745f 7365 7373 696f 6e5f 7369 676e  ect_session_sign
+00001770: 616c 7329 0472 4500 0000 726a 0000 00da  als).rE...rj....
+00001780: 0c73 6573 7369 6f6e 5f70 6174 685a 096f  .session_pathZ.o
+00001790: 6c64 5f69 6e64 6578 722d 0000 0072 2d00  ld_indexr-...r-.
+000017a0: 0000 722e 0000 00da 0e6c 6175 6e63 685f  ..r......launch_
+000017b0: 7365 7373 696f 6eb6 0000 0073 2800 0000  session....s(...
+000017c0: 0801 0a01 1001 0c01 0c03 0803 0801 0801  ................
+000017d0: 0801 1002 1001 1001 1001 1001 1003 0c03  ................
+000017e0: 0804 0a03 0c02 0c01 7a19 4d61 696e 5769  ........z.MainWi
+000017f0: 6e64 6f77 2e6c 6175 6e63 685f 7365 7373  ndow.launch_sess
+00001800: 696f 6e63 0100 0000 0000 0000 0000 0000  ionc............
+00001810: 0100 0000 0400 0000 4300 0000 7308 0100  ........C...s...
+00001820: 007c 006a 00a0 0174 026a 036a 0464 01a1  .|.j...t.j.j.d..
+00001830: 0201 007c 006a 056a 0672 4a74 077c 006a  ...|.j.j.rJt.|.j
+00001840: 0883 0174 096b 0372 187c 00a0 0aa1 0001  ...t.k.r.|......
+00001850: 0074 077c 006a 0b83 0174 0c6b 0372 237c  .t.|.j...t.k.r#|
+00001860: 00a0 0da1 0001 0074 077c 006a 0e83 0174  .......t.|.j...t
+00001870: 0f6b 0372 2e7c 00a0 10a1 0001 007c 006a  .k.r.|.......|.j
+00001880: 00a0 0174 026a 116a 0464 01a1 0201 007c  ...t.j.j.d.....|
+00001890: 006a 00a0 0174 026a 126a 0464 01a1 0201  .j...t.j.j.d....
+000018a0: 007c 006a 00a0 0174 026a 136a 0464 01a1  .|.j...t.j.j.d..
+000018b0: 0201 006e 1b7c 006a 00a0 0174 026a 116a  ...n.|.j...t.j.j
+000018c0: 0464 02a1 0201 007c 006a 00a0 0174 026a  .d.....|.j...t.j
+000018d0: 126a 0464 02a1 0201 007c 006a 00a0 0174  .j.d.....|.j...t
+000018e0: 026a 136a 0464 02a1 0201 007c 006a 05a0  .j.j.d.....|.j..
+000018f0: 14a1 0072 797c 00a0 15a1 0001 007c 006a  ...ry|.......|.j
+00001900: 00a0 0174 026a 166a 0464 01a1 0201 0064  ...t.j.j.d.....d
+00001910: 0353 007c 006a 00a0 0174 026a 166a 0464  .S.|.j...t.j.j.d
+00001920: 02a1 0201 0064 0353 0029 0461 0b01 0000  .....d.S.).a....
+00001930: 0a20 2020 2020 2020 2054 6162 2075 7064  .        Tab upd
+00001940: 6174 6573 206f 6363 7572 2070 7269 6d61  ates occur prima
+00001950: 7269 6c79 2061 7420 3220 7469 6d65 733a  rily at 2 times:
+00001960: 0a20 2020 2020 2020 2031 2e20 7570 6f6e  .        1. upon
+00001970: 206d 6169 6e20 7769 6e64 6f77 2069 6e69   main window ini
+00001980: 7469 6174 696f 6e20 7768 656e 206f 6666  tiation when off
+00001990: 6c69 6e65 2063 6170 6163 6974 6965 7320  line capacities 
+000019a0: 0a20 2020 2020 2020 2028 6361 7074 7572  .        (captur
+000019b0: 6520 766f 6c75 6d65 2061 6e64 2070 6f73  e volume and pos
+000019c0: 742d 7072 6f63 6573 7369 6e67 2920 6d61  t-processing) ma
+000019d0: 7920 6265 2061 7661 696c 6162 6c65 2e0a  y be available..
+000019e0: 0a20 2020 2020 2020 2032 2e20 7570 6f6e  .        2. upon
+000019f0: 206c 6f61 6469 6e67 206f 6620 7374 7265   loading of stre
+00001a00: 616d 2074 6f6f 6c73 2077 6865 6e20 6361  am tools when ca
+00001a10: 6d65 7261 732f 7265 636f 7264 696e 6720  meras/recording 
+00001a20: 776f 756c 6420 6265 2061 7661 696c 6162  would be availab
+00001a30: 6c65 0a20 2020 2020 2020 2054 464e 2917  le.        TFN).
+00001a40: 7244 0000 0072 5000 0000 7220 0000 0072  rD...rP...r ...r
+00001a50: 2800 0000 7251 0000 0072 5500 0000 da13  (...rQ...rU.....
+00001a60: 7374 7265 616d 5f74 6f6f 6c73 5f6c 6f61  stream_tools_loa
+00001a70: 6465 64da 0474 7970 6572 5200 0000 721c  ded..typerR...r.
+00001a80: 0000 00da 126c 6f61 645f 6361 6d65 7261  .....load_camera
+00001a90: 5f77 6964 6765 7472 5400 0000 721e 0000  _widgetrT...r...
+00001aa0: 00da 156c 6f61 645f 7265 636f 7264 696e  ...load_recordin
+00001ab0: 675f 7769 6467 6574 7253 0000 0072 1d00  g_widgetrS...r..
+00001ac0: 0000 da1a 6c6f 6164 5f63 6170 7475 7265  ....load_capture
+00001ad0: 5f76 6f6c 756d 655f 7769 6467 6574 7229  _volume_widgetr)
+00001ae0: 0000 0072 2b00 0000 722a 0000 00da 1b69  ...r+...r*.....i
+00001af0: 735f 706f 7374 5f70 726f 6365 7373 696e  s_post_processin
+00001b00: 675f 656c 6967 6962 6c65 da1b 6c6f 6164  g_eligible..load
+00001b10: 5f70 6f73 745f 7072 6f63 6573 7369 6e67  _post_processing
+00001b20: 5f77 6964 6765 7472 2c00 0000 724e 0000  _widgetr,...rN..
+00001b30: 0072 2d00 0000 722d 0000 0072 2e00 0000  .r-...r-...r....
+00001b40: 726c 0000 00db 0000 0073 2400 0000 120a  rl.......s$.....
+00001b50: 0803 0e02 0801 0e02 0801 0e02 0801 1202  ................
+00001b60: 1201 1401 1205 1201 1201 0a03 0801 1601  ................
+00001b70: 1602 7a16 4d61 696e 5769 6e64 6f77 2e75  ..z.MainWindow.u
+00001b80: 7064 6174 655f 7461 6273 6301 0000 0000  pdate_tabsc.....
+00001b90: 0000 0000 0000 0001 0000 0003 0000 0043  ...............C
+00001ba0: 0000 0073 2800 0000 7c00 6a00 6a01 6a02  ...s(...|.j.j.j.
+00001bb0: a003 7c00 6a04 a101 0100 7c00 6a00 6a01  ..|.j.....|.j.j.
+00001bc0: 6a05 a003 7c00 6a06 a101 0100 6401 5300  j...|.j.....d.S.
+00001bd0: 2902 7a90 0a20 2020 2020 2020 2041 6674  ).z..        Aft
+00001be0: 6572 206c 6175 6e63 6869 6e67 2061 2073  er launching a s
+00001bf0: 6573 7369 6f6e 2c20 636f 6e6e 6563 7420  ession, connect 
+00001c00: 7369 676e 616c 7320 616e 6420 736c 6f74  signals and slot
+00001c10: 732e 0a20 2020 2020 2020 204d 7563 6820  s..        Much 
+00001c20: 6f66 2074 6865 7365 2077 696c 6c20 6265  of these will be
+00001c30: 2066 726f 6d20 7468 6520 4755 4920 746f   from the GUI to
+00001c40: 2074 6865 2073 6573 7369 6f6e 2061 6e64   the session and
+00001c50: 2076 6963 652d 7665 7273 610a 2020 2020   vice-versa.    
+00001c60: 2020 2020 4e29 0772 5500 0000 725f 0000      N).rU...r_..
+00001c70: 00da 1575 6e6c 6f63 6b5f 706f 7374 7072  ...unlock_postpr
+00001c80: 6f63 6573 7369 6e67 7239 0000 0072 7600  ocessingr9...rv.
+00001c90: 0000 7260 0000 0072 6c00 0000 724e 0000  ..r`...rl...rN..
+00001ca0: 0072 2d00 0000 722d 0000 0072 2e00 0000  .r-...r-...r....
+00001cb0: 726d 0000 0007 0100 0073 0400 0000 1205  rm.......s......
+00001cc0: 1601 7a22 4d61 696e 5769 6e64 6f77 2e63  ..z"MainWindow.c
+00001cd0: 6f6e 6e65 6374 5f73 6573 7369 6f6e 5f73  onnect_session_s
+00001ce0: 6967 6e61 6c73 6301 0000 0000 0000 0000  ignalsc.........
+00001cf0: 0000 0002 0000 0005 0000 0043 0000 00f3  ...........C....
+00001d00: 4600 0000 7c00 6a00 a001 7402 6a03 6a04  F...|.j...t.j.j.
+00001d10: a101 0100 7c00 6a05 a006 a100 0100 7407  ....|.j.......t.
+00001d20: 7c00 6a08 8301 7d01 7c00 6a00 a009 7402  |.j...}.|.j...t.
+00001d30: 6a03 6a04 7c01 7402 6a03 6a0a a103 0100  j.j.|.t.j.j.....
+00001d40: 7c01 7c00 5f05 6400 5300 7249 0000 0029  |.|._.d.S.rI...)
+00001d50: 0b72 4400 0000 da09 7265 6d6f 7665 5461  .rD.....removeTa
+00001d60: 6272 2000 0000 722b 0000 0072 5100 0000  br ...r+...rQ...
+00001d70: 7254 0000 00da 0b64 656c 6574 654c 6174  rT.....deleteLat
+00001d80: 6572 721e 0000 0072 5500 0000 da09 696e  err....rU.....in
+00001d90: 7365 7274 5461 62da 046e 616d 6529 0272  sertTab..name).r
+00001da0: 4500 0000 5a14 6e65 775f 7265 636f 7264  E...Z.new_record
+00001db0: 696e 675f 7769 6467 6574 722d 0000 0072  ing_widgetr-...r
+00001dc0: 2d00 0000 722e 0000 0072 7300 0000 0f01  -...r....rs.....
+00001dd0: 0000 730e 0000 0010 020a 010a 0106 010e  ..s.............
+00001de0: 0104 ff0a 037a 204d 6169 6e57 696e 646f  .....z MainWindo
+00001df0: 772e 6c6f 6164 5f72 6563 6f72 6469 6e67  w.load_recording
+00001e00: 5f77 6964 6765 7463 0100 0000 0000 0000  _widgetc........
+00001e10: 0000 0000 0200 0000 0500 0000 4300 0000  ............C...
+00001e20: 7278 0000 0072 4900 0000 290b 7244 0000  rx...rI...).rD..
+00001e30: 0072 7900 0000 7220 0000 0072 2c00 0000  .ry...r ...r,...
+00001e40: 7251 0000 0072 6600 0000 727a 0000 0072  rQ...rf...rz...r
+00001e50: 1f00 0000 7255 0000 0072 7b00 0000 727c  ....rU...r{...r|
+00001e60: 0000 0029 0272 4500 0000 5a15 6e65 775f  ...).rE...Z.new_
+00001e70: 7072 6f63 6573 7369 6e67 5f77 6964 6765  processing_widge
+00001e80: 7472 2d00 0000 722d 0000 0072 2e00 0000  tr-...r-...r....
+00001e90: 7276 0000 0019 0100 00f3 0e00 0000 1001  rv..............
+00001ea0: 0a01 0a01 0601 0e01 04ff 0a03 7a26 4d61  ............z&Ma
+00001eb0: 696e 5769 6e64 6f77 2e6c 6f61 645f 706f  inWindow.load_po
+00001ec0: 7374 5f70 726f 6365 7373 696e 675f 7769  st_processing_wi
+00001ed0: 6467 6574 6301 0000 0000 0000 0000 0000  dgetc...........
+00001ee0: 0002 0000 0005 0000 0043 0000 0072 7800  .........C...rx.
+00001ef0: 0000 7249 0000 0029 0b72 4400 0000 7279  ..rI...).rD...ry
+00001f00: 0000 0072 2000 0000 722a 0000 0072 5100  ...r ...r*...rQ.
+00001f10: 0000 7253 0000 0072 7a00 0000 721d 0000  ..rS...rz...r...
+00001f20: 0072 5500 0000 727b 0000 0072 7c00 0000  .rU...r{...r|...
+00001f30: 2902 7245 0000 005a 196e 6577 5f63 6170  ).rE...Z.new_cap
+00001f40: 7475 7265 5f76 6f6c 756d 655f 7769 6467  ture_volume_widg
+00001f50: 6574 722d 0000 0072 2d00 0000 722e 0000  etr-...r-...r...
+00001f60: 0072 7400 0000 2201 0000 7312 0000 0010  .rt..."...s.....
+00001f70: 010a 010a 0106 0106 0102 0106 0104 fd0a  ................
+00001f80: 057a 254d 6169 6e57 696e 646f 772e 6c6f  .z%MainWindow.lo
+00001f90: 6164 5f63 6170 7475 7265 5f76 6f6c 756d  ad_capture_volum
+00001fa0: 655f 7769 6467 6574 6301 0000 0000 0000  e_widgetc.......
+00001fb0: 0000 0000 0002 0000 0005 0000 0043 0000  .............C..
+00001fc0: 0072 7800 0000 7249 0000 0029 0b72 4400  .rx...rI...).rD.
+00001fd0: 0000 7279 0000 0072 2000 0000 7229 0000  ..ry...r ...r)..
+00001fe0: 0072 5100 0000 7252 0000 0072 7a00 0000  .rQ...rR...rz...
+00001ff0: 721c 0000 0072 5500 0000 727b 0000 0072  r....rU...r{...r
+00002000: 7c00 0000 2902 7245 0000 005a 116e 6577  |...).rE...Z.new
+00002010: 5f63 616d 6572 615f 7769 6467 6574 722d  _camera_widgetr-
+00002020: 0000 0072 2d00 0000 722e 0000 0072 7200  ...r-...r....rr.
+00002030: 0000 2d01 0000 727d 0000 007a 1d4d 6169  ..-...r}...z.Mai
+00002040: 6e57 696e 646f 772e 6c6f 6164 5f63 616d  nWindow.load_cam
+00002050: 6572 615f 7769 6467 6574 7246 0000 0063  era_widgetrF...c
+00002060: 0200 0000 0000 0000 0000 0000 0300 0000  ................
+00002070: 0300 0000 4300 0000 7328 0000 0074 007c  ....C...s(...t.|
+00002080: 017c 0083 027d 027c 026a 01a0 027c 006a  .|...}.|.j...|.j
+00002090: 03a1 0101 007c 006a 04a0 057c 02a1 0101  .....|.j...|....
+000020a0: 0064 0053 0072 4900 0000 2906 7210 0000  .d.S.rI...).r...
+000020b0: 0072 3800 0000 7239 0000 00da 136f 7065  .r8...r9.....ope
+000020c0: 6e5f 7265 6365 6e74 5f70 726f 6a65 6374  n_recent_project
+000020d0: 723c 0000 0072 3b00 0000 2903 7245 0000  r<...r;...).rE..
+000020e0: 0072 4600 0000 5a15 7265 6365 6e74 5f70  .rF...Z.recent_p
+000020f0: 726f 6a65 6374 5f61 6374 696f 6e72 2d00  roject_actionr-.
+00002100: 0000 722d 0000 0072 2e00 0000 723e 0000  ..r-...r....r>..
+00002110: 0039 0100 0073 0600 0000 0a01 0e01 1001  .9...s..........
+00002120: 7a20 4d61 696e 5769 6e64 6f77 2e61 6464  z MainWindow.add
+00002130: 5f74 6f5f 7265 6365 6e74 5f70 726f 6a65  _to_recent_proje
+00002140: 6374 6301 0000 0000 0000 0000 0000 0003  ctc.............
+00002150: 0000 0004 0000 0043 0000 0073 2e00 0000  .......C...s....
+00002160: 7c00 a000 a100 7d01 7c01 a001 a100 7d02  |.....}.|.....}.
+00002170: 7402 a003 6401 7c02 9b00 9d02 a101 0100  t...d.|.........
+00002180: 7c00 a004 7c02 a101 0100 6400 5300 2902  |...|.....d.S.).
+00002190: 4e7a 214f 7065 6e69 6e67 2072 6563 656e  Nz!Opening recen
+000021a0: 7420 7365 7373 696f 6e20 7374 6f72 6564  t session stored
+000021b0: 2061 7420 2905 5a06 7365 6e64 6572 da04   at ).Z.sender..
+000021c0: 7465 7874 7257 0000 0072 5800 0000 726f  textrW...rX...ro
+000021d0: 0000 0029 0372 4500 0000 da06 6163 7469  ...).rE.....acti
+000021e0: 6f6e 7246 0000 0072 2d00 0000 722d 0000  onrF...r-...r-..
+000021f0: 0072 2e00 0000 727e 0000 003e 0100 0073  .r....r~...>...s
+00002200: 0800 0000 0801 0801 1001 0e01 7a1e 4d61  ............z.Ma
+00002210: 696e 5769 6e64 6f77 2e6f 7065 6e5f 7265  inWindow.open_re
+00002220: 6365 6e74 5f70 726f 6a65 6374 6301 0000  cent_projectc...
+00002230: 0000 0000 0000 0000 0004 0000 0006 0000  ................
+00002240: 0043 0000 0073 5c00 0000 7400 7c00 6a01  .C...s\...t.|.j.
+00002250: 6401 1900 8301 7d01 7402 8300 7d02 7c02  d.....}.t...}.|.
+00002260: 6a03 6400 6402 7404 7c01 8301 7402 6a05  j.d.d.t.|...t.j.
+00002270: 6a06 6403 8d04 7d03 7c03 722c 7407 a008  j.d...}.|.r,t...
+00002280: 6404 7c03 6602 a101 0100 7c00 a009 7c03  d.|.f.....|...|.
+00002290: a101 0100 7c00 a00a 7c03 a101 0100 6400  ....|...|.....d.
+000022a0: 5300 6400 5300 2905 4eda 136c 6173 745f  S.d.S.).N..last_
+000022b0: 7072 6f6a 6563 745f 7061 7265 6e74 7a2d  project_parentz-
+000022c0: 4f70 656e 2050 7265 7669 6f75 7320 6f72  Open Previous or
+000022d0: 2043 7265 6174 6520 4e65 7720 5072 6f6a   Create New Proj
+000022e0: 6563 7420 4469 7265 6374 6f72 7929 04da  ect Directory)..
+000022f0: 0670 6172 656e 74da 0763 6170 7469 6f6e  .parent..caption
+00002300: da09 6469 7265 6374 6f72 79da 076f 7074  ..directory..opt
+00002310: 696f 6e73 7a19 4372 6561 7469 6e67 206e  ionsz.Creating n
+00002320: 6577 2070 726f 6a65 6374 2069 6e20 3a29  ew project in :)
+00002330: 0b72 0500 0000 7235 0000 0072 0400 0000  .r....r5...r....
+00002340: 5a14 6765 7445 7869 7374 696e 6744 6972  Z.getExistingDir
+00002350: 6563 746f 7279 7237 0000 00da 064f 7074  ectoryr7.....Opt
+00002360: 696f 6e5a 0c53 686f 7744 6972 734f 6e6c  ionZ.ShowDirsOnl
+00002370: 7972 5700 0000 7258 0000 00da 1561 6464  yrW...rX.....add
+00002380: 5f70 726f 6a65 6374 5f74 6f5f 7265 6365  _project_to_rece
+00002390: 6e74 726f 0000 0029 0472 4500 0000 5a0e  ntro...).rE...Z.
+000023a0: 6465 6661 756c 745f 666f 6c64 6572 5a06  default_folderZ.
+000023b0: 6469 616c 6f67 726a 0000 0072 2d00 0000  dialogrj...r-...
+000023c0: 722d 0000 0072 2e00 0000 723a 0000 0044  r-...r....r:...D
+000023d0: 0100 0073 1a00 0000 0e01 0601 0401 0201  ...s............
+000023e0: 0201 0601 0601 06fc 0407 0e01 0a01 0e01  ................
+000023f0: 04fd 7a24 4d61 696e 5769 6e64 6f77 2e63  ..z$MainWindow.c
+00002400: 7265 6174 655f 6e65 775f 7072 6f6a 6563  reate_new_projec
+00002410: 745f 666f 6c64 6572 6302 0000 0000 0000  t_folderc.......
+00002420: 0000 0000 0002 0000 0004 0000 0043 0000  .............C..
+00002430: 0073 5400 0000 7400 7c01 8301 7c00 6a01  .sT...t.|...|.j.
+00002440: 6401 1900 7600 720b 6400 5300 7c00 6a01  d...v.r.d.S.|.j.
+00002450: 6401 1900 a002 7400 7c01 8301 a101 0100  d.....t.|.......
+00002460: 7400 7403 7c01 8301 6a04 8301 7c00 6a01  t.t.|...j...|.j.
+00002470: 6402 3c00 7c00 a005 a100 0100 7c00 a006  d.<.|.......|...
+00002480: 7c01 a101 0100 6400 5300 2903 4e72 3000  |.....d.S.).Nr0.
+00002490: 0000 7281 0000 0029 0772 3700 0000 7235  ..r....).r7...r5
+000024a0: 0000 00da 0661 7070 656e 6472 0500 0000  .....appendr....
+000024b0: 7282 0000 00da 1375 7064 6174 655f 6170  r......update_ap
+000024c0: 705f 7365 7474 696e 6773 723e 0000 0029  p_settingsr>...)
+000024d0: 0272 4500 0000 5a0b 666f 6c64 6572 5f70  .rE...Z.folder_p
+000024e0: 6174 6872 2d00 0000 722d 0000 0072 2e00  athr-...r-...r..
+000024f0: 0000 7287 0000 0053 0100 0073 0c00 0000  ..r....S...s....
+00002500: 1201 0401 1402 1401 0801 0e01 7a20 4d61  ............z Ma
+00002510: 696e 5769 6e64 6f77 2e61 6464 5f70 726f  inWindow.add_pro
+00002520: 6a65 6374 5f74 6f5f 7265 6365 6e74 6301  ject_to_recentc.
+00002530: 0000 0000 0000 0000 0000 0002 0000 0008  ................
+00002540: 0000 0043 0000 0073 3e00 0000 7400 7401  ...C...s>...t.t.
+00002550: 6401 8302 8f10 7d01 7402 a003 7c00 6a04  d.....}.t...|.j.
+00002560: 7c01 a102 0100 5700 6400 0400 0400 8303  |.....W.d.......
+00002570: 0100 6400 5300 3100 7318 7701 0100 0100  ..d.S.1.s.w.....
+00002580: 0100 5900 0100 6400 5300 2902 4eda 0177  ..Y...d.S.).N..w
+00002590: 2905 da04 6f70 656e 7215 0000 0072 3300  )...openr....r3.
+000025a0: 0000 da04 6475 6d70 7235 0000 0029 0272  ....dumpr5...).r
+000025b0: 4500 0000 da01 6672 2d00 0000 722d 0000  E.....fr-...r-..
+000025c0: 0072 2e00 0000 7289 0000 005c 0100 0073  .r....r....\...s
+000025d0: 0600 0000 0c01 1001 22ff 7a1e 4d61 696e  ........".z.Main
+000025e0: 5769 6e64 6f77 2e75 7064 6174 655f 6170  Window.update_ap
+000025f0: 705f 7365 7474 696e 6773 2917 7225 0000  p_settings).r%..
+00002600: 0072 2600 0000 7227 0000 0072 3200 0000  .r&...r'...r2...
+00002610: 7243 0000 0072 4d00 0000 725b 0000 0072  rC...rM...r[...r
+00002620: 4a00 0000 7269 0000 0072 3700 0000 726f  J...ri...r7...ro
+00002630: 0000 0072 6c00 0000 726d 0000 0072 7300  ...rl...rm...rs.
+00002640: 0000 7276 0000 0072 7400 0000 7272 0000  ..rv...rt...rr..
+00002650: 0072 3e00 0000 727e 0000 0072 3a00 0000  .r>...r~...r:...
+00002660: 7287 0000 0072 8900 0000 da0d 5f5f 636c  r....r......__cl
+00002670: 6173 7363 656c 6c5f 5f72 2d00 0000 722d  asscell__r-...r-
+00002680: 0000 0072 4700 0000 722e 0000 0072 2f00  ...rG...r....r/.
+00002690: 0000 3000 0000 7326 0000 0008 000c 0108  ..0...s&........
+000026a0: 3908 0508 1108 0508 0b0e 2608 2508 2c08  9.........&.%.,.
+000026b0: 0808 0a08 0908 0b0e 0c08 0508 0608 0f10  ................
+000026c0: 0972 2f00 0000 6300 0000 0000 0000 0000  .r/...c.........
+000026d0: 0000 0000 0000 0003 0000 0000 0000 0073  ...............s
+000026e0: 2c00 0000 6500 5a01 6400 5a02 6401 5a03  ,...e.Z.d.Z.d.Z.
+000026f0: 8700 6601 6402 6403 8408 5a04 8700 6601  ..f.d.d...Z...f.
+00002700: 6404 6405 8408 5a05 8700 0400 5a06 5300  d.d...Z.....Z.S.
+00002710: 2906 da10 4365 6e74 7261 6c54 6162 5769  )...CentralTabWi
+00002720: 6467 6574 6189 0100 000a 2020 2020 5377  dgeta.....    Sw
+00002730: 6974 6368 696e 6720 6265 7477 6565 6e20  itching between 
+00002740: 7461 6273 2c20 7061 7274 6963 756c 6172  tabs, particular
+00002750: 6c79 2077 6865 6e20 7379 7374 656d 2072  ly when system r
+00002760: 6573 6f75 7263 6520 7574 696c 697a 6174  esource utilizat
+00002770: 696f 6e20 6973 2068 6967 682c 0a20 2020  ion is high,.   
+00002780: 2069 7320 7072 6f6e 6520 746f 2072 6573   is prone to res
+00002790: 756c 7420 696e 2073 6567 6661 756c 7420  ult in segfault 
+000027a0: 6372 6173 6865 732e 2057 6f72 6b69 6e67  crashes. Working
+000027b0: 2068 7970 6f74 6865 7369 7320 6973 2074   hypothesis is t
+000027c0: 6861 7420 7468 6973 2069 7320 6475 6520  hat this is due 
+000027d0: 746f 206d 6f64 650a 2020 2020 6368 616e  to mode.    chan
+000027e0: 6765 7320 6861 7070 656e 696e 6720 7768  ges happening wh
+000027f0: 656e 2074 6865 2074 6162 2069 7320 6368  en the tab is ch
+00002800: 616e 6765 6420 616e 6420 7468 6520 4755  anged and the GU
+00002810: 4920 7472 6965 7320 746f 2072 656e 6465  I tries to rende
+00002820: 7220 736f 6d65 7468 696e 6720 6974 2064  r something it d
+00002830: 6f65 736e 2774 2068 6176 650a 2020 2020  oesn't have.    
+00002840: 0a20 2020 2054 6869 7320 6f76 6572 7269  .    This overri
+00002850: 6465 2073 6c69 7073 2074 6865 206d 6f64  de slips the mod
+00002860: 6520 6368 616e 6765 2062 6574 7765 656e  e change between
+00002870: 2063 6c69 636b 2061 6e64 2063 6861 6e67   click and chang
+00002880: 6520 746f 2074 7279 2074 6f20 7374 6162  e to try to stab
+00002890: 696c 697a 6520 7468 6520 6d6f 6465 2073  ilize the mode s
+000028a0: 7769 7463 6865 732e 0a20 2020 200a 2020  witches..    .  
+000028b0: 2020 6301 0000 0000 0000 0000 0000 0001    c.............
+000028c0: 0000 0003 0000 0003 0000 0073 1200 0000  ...........s....
+000028d0: 7400 7401 7c00 8302 a002 a100 0100 6400  t.t.|.........d.
+000028e0: 5300 7249 0000 0029 0372 3100 0000 728f  S.rI...).r1...r.
+000028f0: 0000 0072 3200 0000 724e 0000 0072 4700  ...r2...rN...rG.
+00002900: 0000 722d 0000 0072 2e00 0000 7232 0000  ..r-...r....r2..
+00002910: 006b 0100 0073 0200 0000 1201 7a19 4365  .k...s......z.Ce
+00002920: 6e74 7261 6c54 6162 5769 6467 6574 2e5f  ntralTabWidget._
+00002930: 5f69 6e69 745f 5f63 0200 0000 0000 0000  _init__c........
+00002940: 0000 0000 0200 0000 0500 0000 0300 0000  ................
+00002950: 7326 0000 0074 00a0 0164 017c 019b 0064  s&...t...d.|...d
+00002960: 029d 03a1 0101 0074 0274 037c 0083 02a0  .......t.t.|....
+00002970: 047c 01a1 0101 0064 0053 0029 034e 7a04  .|.....d.S.).Nz.
+00002980: 5461 6220 7a08 2063 6c69 636b 6564 2905  Tab z. clicked).
+00002990: 7257 0000 0072 5800 0000 7231 0000 0072  rW...rX...r1...r
+000029a0: 8f00 0000 da0d 7461 6242 6172 436c 6963  ......tabBarClic
+000029b0: 6b65 6472 6700 0000 7247 0000 0072 2d00  kedrg...rG...r-.
+000029c0: 0000 722e 0000 0072 9000 0000 6e01 0000  ..r....r....n...
+000029d0: 7304 0000 0012 0214 037a 1e43 656e 7472  s........z.Centr
+000029e0: 616c 5461 6257 6964 6765 742e 7461 6242  alTabWidget.tabB
+000029f0: 6172 436c 6963 6b65 6429 0772 2500 0000  arClicked).r%...
+00002a00: 7226 0000 0072 2700 0000 da07 5f5f 646f  r&...r'.....__do
+00002a10: 635f 5f72 3200 0000 7290 0000 0072 8e00  c__r2...r....r..
+00002a20: 0000 722d 0000 0072 2d00 0000 7247 0000  ..r-...r-...rG..
+00002a30: 0072 2e00 0000 728f 0000 0061 0100 0073  .r....r....a...s
+00002a40: 0800 0000 0800 0401 0c09 1403 728f 0000  ............r...
+00002a50: 0063 0000 0000 0000 0000 0000 0000 0200  .c..............
+00002a60: 0000 0200 0000 4300 0000 7324 0000 0074  ......C...s$...t
+00002a70: 0074 016a 0283 017d 0074 0383 007d 017c  .t.j...}.t...}.|
+00002a80: 01a0 04a1 0001 007c 00a0 05a1 0001 0064  .......|.......d
+00002a90: 0053 0072 4900 0000 2906 7207 0000 00da  .S.rI...).r.....
+00002aa0: 0373 7973 da04 6172 6776 722f 0000 00da  .sys..argvr/....
+00002ab0: 0473 686f 77da 0465 7865 6329 02da 0361  .show..exec)...a
+00002ac0: 7070 da06 7769 6e64 6f77 722d 0000 0072  pp..windowr-...r
+00002ad0: 2d00 0000 722e 0000 00da 0b6c 6175 6e63  -...r......launc
+00002ae0: 685f 6d61 696e 7501 0000 7308 0000 000a  h_mainu...s.....
+00002af0: 0106 0108 010c 0272 9800 0000 da08 5f5f  .......r......__
+00002b00: 6d61 696e 5f5f 2937 da0d 7079 7879 3364  main__)7..pyxy3d
+00002b10: 2e6c 6f67 6765 72da 0670 7978 7933 6472  .logger..pyxy3dr
+00002b20: 5700 0000 da03 6765 7472 2500 0000 da0f  W.....getr%.....
+00002b30: 5079 5174 362e 5174 5769 6467 6574 7372  PyQt6.QtWidgetsr
+00002b40: 0200 0000 7203 0000 0072 0400 0000 da07  ....r....r......
+00002b50: 7061 7468 6c69 6272 0500 0000 da09 7468  pathlibr......th
+00002b60: 7265 6164 696e 6772 0600 0000 7292 0000  readingr....r...
+00002b70: 0072 0700 0000 7208 0000 0072 0900 0000  .r....r....r....
+00002b80: 720a 0000 0072 0b00 0000 720c 0000 0072  r....r....r....r
+00002b90: 0d00 0000 7233 0000 00da 0465 6e75 6d72  ....r3.....enumr
+00002ba0: 0e00 0000 5a0b 5079 5174 362e 5174 4775  ....Z.PyQt6.QtGu
+00002bb0: 6972 0f00 0000 7210 0000 0072 1100 0000  ir....r....r....
+00002bc0: 7212 0000 005a 0c50 7951 7436 2e51 7443  r....Z.PyQt6.QtC
+00002bd0: 6f72 6572 1300 0000 7214 0000 0072 1500  orer....r....r..
+00002be0: 0000 7216 0000 00da 1670 7978 7933 642e  ..r......pyxy3d.
+00002bf0: 7365 7373 696f 6e2e 7365 7373 696f 6e72  session.sessionr
+00002c00: 1700 0000 7218 0000 005a 1570 7978 7933  ....r....Z.pyxy3
+00002c10: 642e 6775 692e 6c6f 675f 7769 6467 6574  d.gui.log_widget
+00002c20: 7219 0000 00da 1370 7978 7933 642e 636f  r......pyxy3d.co
+00002c30: 6e66 6967 7572 6174 6f72 721a 0000 005a  nfiguratorr....Z
+00002c40: 1970 7978 7933 642e 6775 692e 6368 6172  .pyxy3d.gui.char
+00002c50: 7563 6f5f 7769 6467 6574 721b 0000 005a  uco_widgetr....Z
+00002c60: 3570 7978 7933 642e 6775 692e 6361 6d65  5pyxy3d.gui.came
+00002c70: 7261 5f63 6f6e 6669 672e 696e 7472 696e  ra_config.intrin
+00002c80: 7369 635f 6361 6c69 6272 6174 696f 6e5f  sic_calibration_
+00002c90: 7769 6467 6574 721c 0000 005a 2a70 7978  widgetr....Z*pyx
+00002ca0: 7933 642e 6775 692e 6361 6c69 6272 6174  y3d.gui.calibrat
+00002cb0: 655f 6361 7074 7572 655f 766f 6c75 6d65  e_capture_volume
+00002cc0: 5f77 6964 6765 7472 1d00 0000 da1b 7079  _widgetr......py
+00002cd0: 7879 3364 2e67 7569 2e72 6563 6f72 6469  xy3d.gui.recordi
+00002ce0: 6e67 5f77 6964 6765 7472 1e00 0000 5a21  ng_widgetr....Z!
+00002cf0: 7079 7879 3364 2e67 7569 2e70 6f73 745f  pyxy3d.gui.post_
+00002d00: 7072 6f63 6573 7369 6e67 5f77 6964 6765  processing_widge
+00002d10: 7472 1f00 0000 7220 0000 0072 2f00 0000  tr....r ...r/...
+00002d20: 728f 0000 0072 9800 0000 722d 0000 0072  r....r....r-...r
+00002d30: 2d00 0000 722d 0000 0072 2e00 0000 da08  -...r-...r......
+00002d40: 3c6d 6f64 756c 653e 0100 0000 733e 0000  <module>....s>..
+00002d50: 0008 0008 010c 0214 020c 020c 010c 0108  ................
+00002d60: 012c 0108 0b0c 0118 010c 0114 0110 010c  .,..............
+00002d70: 010c 010c 010c 010c 030c 010c 0110 0310  ................
+00002d80: 0800 7f00 7f10 3308 1408 080a 0104 ff    ......3........
```

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/__pycache__/navigation_bars.cpython-310.pyc` & `pyxy3d-0.1.4/pyxy3d/gui/__pycache__/navigation_bars.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/__pycache__/playback_widget.cpython-310.pyc` & `pyxy3d-0.1.4/pyxy3d/gui/__pycache__/playback_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/__pycache__/post_processing_widget.cpython-310.pyc` & `pyxy3d-0.1.4/pyxy3d/gui/__pycache__/post_processing_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/__pycache__/progress_dialog.cpython-310.pyc` & `pyxy3d-0.1.4/pyxy3d/gui/__pycache__/progress_dialog.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/__pycache__/qt_logger.cpython-310.pyc` & `pyxy3d-0.1.4/pyxy3d/gui/__pycache__/qt_logger.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/__pycache__/qt_logger.cpython-38.pyc` & `pyxy3d-0.1.4/pyxy3d/gui/__pycache__/qt_logger.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/__pycache__/recording_widget.cpython-310.pyc` & `pyxy3d-0.1.4/pyxy3d/gui/__pycache__/recording_widget.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jun 15 18:45:15 2023 UTC, .py size: 14740 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3b5c 8b64 9439 0000  o.......;\.d.9..
+00000000: 6f0d 0d0a 0000 0000 3fe7 9564 6a3b 0000  o.......?..dj;..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7e01 0000 6400  .....@...s~...d.
 00000030: 6401 6c00 5a01 6501 6a02 a003 6504 a101  d.l.Z.e.j...e...
 00000040: 5a02 6400 6401 6c05 5a05 6400 6401 6c06  Z.d.d.l.Z.d.d.l.
 00000050: 5a06 6400 6402 6c07 6d08 5a08 0100 6400  Z.d.d.l.m.Z...d.
 00000060: 6403 6c09 6d0a 5a0a 6d0b 5a0b 0100 6400  d.l.m.Z.m.Z...d.
 00000070: 6401 6c0c 5a0d 6400 6404 6c0e 6d0f 5a0f  d.l.Z.d.d.l.m.Z.
@@ -99,18 +99,18 @@
 00000620: 7379 6e63 6872 6f6e 697a 6572 da14 556e  synchronizer..Un
 00000630: 7061 6972 6564 4672 616d 6542 7569 6c64  pairedFrameBuild
 00000640: 6572 da16 756e 7061 6972 6564 5f66 7261  er..unpaired_fra
 00000650: 6d65 5f62 7569 6c64 6572 da14 556e 7061  me_builder..Unpa
 00000660: 6972 6564 4672 616d 6545 6d69 7474 6572  iredFrameEmitter
 00000670: da16 756e 7061 6972 6564 5f66 7261 6d65  ..unpaired_frame
 00000680: 5f65 6d69 7474 6572 da05 7374 6172 7472  _emitter..startr
-00000690: 2200 0000 da0e 7669 6465 6f5f 7265 636f  ".....video_reco
+00000690: 2200 0000 5a0e 7669 6465 6f5f 7265 636f  "...Z.video_reco
 000006a0: 7264 6572 7210 0000 00da 0f66 7261 6d65  rderr......frame
-000006b0: 5f72 6174 655f 7370 696e da08 7365 7456  _rate_spin..setV
-000006c0: 616c 7565 da0d 6670 735f 7265 636f 7264  alue..fps_record
+000006b0: 5f72 6174 655f 7370 696e 5a08 7365 7456  _rate_spinZ.setV
+000006c0: 616c 7565 5a0d 6670 735f 7265 636f 7264  alueZ.fps_record
 000006d0: 696e 6772 2400 0000 7228 0000 00da 0b6e  ingr$...r(.....n
 000006e0: 6578 745f 6163 7469 6f6e 721b 0000 00da  ext_actionr.....
 000006f0: 0576 616c 7565 da0a 7374 6172 745f 7374  .value..start_st
 00000700: 6f70 721a 0000 00da 1164 6573 7469 6e61  opr......destina
 00000710: 7469 6f6e 5f6c 6162 656c 7215 0000 00da  tion_labelr.....
 00000720: 1c67 6574 5f6e 6578 745f 7265 636f 7264  .get_next_record
 00000730: 696e 675f 6469 7265 6374 6f72 79da 1372  ing_directory..r
@@ -129,19 +129,19 @@
 00000800: 0e01 0802 0802 0802 0801 0c01 7a18 5265  ............z.Re
 00000810: 636f 7264 696e 6757 6964 6765 742e 5f5f  cordingWidget.__
 00000820: 696e 6974 5f5f 6301 0000 0000 0000 0000  init__c.........
 00000830: 0000 0001 0000 0003 0000 0043 0000 0073  ...........C...s
 00000840: 2a00 0000 7c00 6a00 a001 a100 720d 7c00  *...|.j.....r.|.
 00000850: 6a02 a003 6401 a101 0100 6400 5300 7c00  j...d.....d.S.|.
 00000860: 6a02 a003 6402 a101 0100 6400 5300 2903  j...d.....d.S.).
-00000870: 4e54 4629 0472 2e00 0000 da15 6973 5f72  NTF).r......is_r
+00000870: 4e54 4629 0472 2e00 0000 5a15 6973 5f72  NTF).r....Z.is_r
 00000880: 6563 6f72 6469 6e67 5f65 6c69 6769 626c  ecording_eligibl
-00000890: 6572 3d00 0000 da0a 7365 7445 6e61 626c  er=.....setEnabl
-000008a0: 6564 a901 7246 0000 0072 2b00 0000 722b  ed..rF...r+...r+
-000008b0: 0000 0072 2c00 0000 7245 0000 0053 0000  ...r,...rE...S..
+00000890: 6572 3a00 0000 da0a 7365 7445 6e61 626c  er:.....setEnabl
+000008a0: 6564 a901 7243 0000 0072 2b00 0000 722b  ed..rC...r+...r+
+000008b0: 0000 0072 2c00 0000 7242 0000 0053 0000  ...r,...rB...S..
 000008c0: 0073 0600 0000 0a01 1001 1002 7a26 5265  .s..........z&Re
 000008d0: 636f 7264 696e 6757 6964 6765 742e 7570  cordingWidget.up
 000008e0: 6461 7465 5f62 746e 5f65 6c69 6769 6269  date_btn_eligibi
 000008f0: 6c69 7479 6301 0000 0000 0000 0000 0000  lityc...........
 00000900: 0005 0000 0004 0000 0043 0000 0073 6c00  .........C...sl.
 00000910: 0000 6401 6402 8400 7c00 6a00 6a01 a002  ..d.d...|.j.j...
 00000920: a100 4400 8301 7d01 6403 6402 8400 7c01  ..D...}.d.d...|.
@@ -163,42 +163,42 @@
 00000a20: 6469 6e67 5f64 6972 6563 746f 7279 2e3c  ding_directory.<
 00000a30: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
 00000a40: 703e 6301 0000 0000 0000 0000 0000 0002  p>c.............
 00000a50: 0000 0005 0000 0053 0000 0073 1a00 0000  .......S...s....
 00000a60: 6700 7c00 5d09 7d01 7c01 a000 6400 a101  g.|.].}.|...d...
 00000a70: 7202 7c01 9102 7102 5300 2901 da0a 7265  r.|...q.S.)...re
 00000a80: 636f 7264 696e 675f 2901 da0a 7374 6172  cording_)...star
-00000a90: 7473 7769 7468 a902 724e 0000 00da 0666  tswith..rN.....f
+00000a90: 7473 7769 7468 a902 724a 0000 005a 0666  tswith..rJ...Z.f
 00000aa0: 6f6c 6465 7272 2b00 0000 722b 0000 0072  olderr+...r+...r
-00000ab0: 2c00 0000 7250 0000 005d 0000 0072 5100  ,...rP...]...rQ.
+00000ab0: 2c00 0000 724c 0000 005d 0000 0072 4d00  ,...rL...]...rM.
 00000ac0: 0000 6301 0000 0000 0000 0000 0000 0002  ..c.............
 00000ad0: 0000 0005 0000 0053 0000 0073 1a00 0000  .......S...s....
 00000ae0: 6700 7c00 5d09 7d01 7c01 a000 6400 a101  g.|.].}.|...d...
 00000af0: 6401 1900 9102 7102 5300 2902 da01 5fe9  d.....q.S.)..._.
-00000b00: 0100 0000 2901 da05 7370 6c69 7472 5400  ....)...splitrT.
+00000b00: 0100 0000 2901 da05 7370 6c69 7472 5000  ....)...splitrP.
 00000b10: 0000 722b 0000 0072 2b00 0000 722c 0000  ..r+...r+...r,..
-00000b20: 0072 5000 0000 5e00 0000 7251 0000 0063  .rP...^...rQ...c
+00000b20: 0072 4c00 0000 5e00 0000 724d 0000 0063  .rL...^...rM...c
 00000b30: 0100 0000 0000 0000 0000 0000 0200 0000  ................
 00000b40: 0400 0000 5300 0000 731c 0000 0067 007c  ....S...s....g.|
 00000b50: 005d 0a7d 017c 01a0 00a1 0072 0274 017c  .].}.|.....r.t.|
 00000b60: 0183 0191 0271 0253 0072 2b00 0000 2902  .....q.S.r+...).
 00000b70: da09 6973 6e75 6d65 7269 63da 0369 6e74  ..isnumeric..int
-00000b80: 2902 724e 0000 005a 0972 6563 5f63 6f75  ).rN...Z.rec_cou
+00000b80: 2902 724a 0000 005a 0972 6563 5f63 6f75  ).rJ...Z.rec_cou
 00000b90: 6e74 722b 0000 0072 2b00 0000 722c 0000  ntr+...r+...r,..
-00000ba0: 0072 5000 0000 5f00 0000 f302 0000 001c  .rP..._.........
+00000ba0: 0072 4c00 0000 5f00 0000 f302 0000 001c  .rL..._.........
 00000bb0: 0072 0100 0000 5a0b 7265 636f 7264 696e  .r....Z.recordin
-00000bc0: 675f 3172 5200 0000 7257 0000 0029 0672  g_1rR...rW...).r
+00000bc0: 675f 3172 4e00 0000 7252 0000 0029 0672  g_1rN...rR...).r
 00000bd0: 2e00 0000 da04 7061 7468 da07 6974 6572  ......path..iter
 00000be0: 6469 72da 036c 656e da03 7374 72da 036d  dir..len..str..m
-00000bf0: 6178 2905 7246 0000 005a 0766 6f6c 6465  ax).rF...Z.folde
+00000bf0: 6178 2905 7243 0000 005a 0766 6f6c 6465  ax).rC...Z.folde
 00000c00: 7273 5a11 7265 636f 7264 696e 675f 666f  rsZ.recording_fo
 00000c10: 6c64 6572 735a 1072 6563 6f72 6469 6e67  ldersZ.recording
 00000c20: 5f63 6f75 6e74 735a 0e6e 6578 745f 6469  _countsZ.next_di
 00000c30: 7265 6374 6f72 7972 2b00 0000 722b 0000  rectoryr+...r+..
-00000c40: 0072 2c00 0000 723f 0000 005a 0000 0073  .r,...r?...Z...s
+00000c40: 0072 2c00 0000 723c 0000 005a 0000 0073  .r,...r<...Z...s
 00000c50: 1200 0000 1602 0e01 0e01 0e01 0c02 0401  ................
 00000c60: 0405 14fe 0402 7a2c 5265 636f 7264 696e  ......z,Recordin
 00000c70: 6757 6964 6765 742e 6765 745f 6e65 7874  gWidget.get_next
 00000c80: 5f72 6563 6f72 6469 6e67 5f64 6972 6563  _recording_direc
 00000c90: 746f 7279 6301 0000 0000 0000 0000 0000  toryc...........
 00000ca0: 0001 0000 0004 0000 0043 0000 0073 da00  .........C...s..
 00000cb0: 0000 7c00 a000 7401 8300 a101 0100 7402  ..|...t.......t.
@@ -210,538 +210,557 @@
 00000d10: 7c00 5f09 7c00 6a09 a000 7404 8300 a101  |._.|.j...t.....
 00000d20: 0100 7c00 6a09 a005 a100 a006 7c00 6a0a  ..|.j.......|.j.
 00000d30: a101 0100 7c00 6a09 a005 a100 a006 7c00  ....|.j.......|.
 00000d40: 6a0b a101 0100 7c00 6a09 a005 a100 a006  j.....|.j.......
 00000d50: 7c00 6a0c a101 0100 7c00 a005 a100 a006  |.j.....|.......
 00000d60: 7c00 6a09 a101 0100 7c00 a005 a100 a006  |.j.....|.......
 00000d70: 7c00 6a0d a101 0100 7c00 a005 a100 a006  |.j.....|.......
-00000d80: 7c00 6a0e a101 0100 6400 5300 2903 4eda  |.j.....d.S.).N.
+00000d80: 7c00 6a0e a101 0100 6400 5300 2903 4e5a  |.j.....d.S.).NZ
 00000d90: 0853 6574 7469 6e67 737a 0b46 7261 6d65  .Settingsz.Frame
-00000da0: 2052 6174 653a 290f da09 7365 744c 6179   Rate:)...setLay
-00000db0: 6f75 7472 1d00 0000 7217 0000 00da 0e73  outr....r......s
+00000da0: 2052 6174 653a 290f 5a09 7365 744c 6179   Rate:).Z.setLay
+00000db0: 6f75 7472 1d00 0000 7217 0000 005a 0e73  outr....r....Z.s
 00000dc0: 6574 7469 6e67 735f 6772 6f75 7072 1900  ettings_groupr..
-00000dd0: 0000 da06 6c61 796f 7574 da09 6164 6457  ....layout..addW
-00000de0: 6964 6765 7472 1a00 0000 7238 0000 005a  idgetr....r8...Z
+00000dd0: 0000 5a06 6c61 796f 7574 5a09 6164 6457  ..Z.layoutZ.addW
+00000de0: 6964 6765 7472 1a00 0000 7237 0000 005a  idgetr....r7...Z
 00000df0: 0f72 6563 6f72 645f 636f 6e74 726f 6c73  .record_controls
-00000e00: 723d 0000 0072 3e00 0000 7240 0000 0072  r=...r>...r@...r
-00000e10: 4100 0000 7242 0000 0072 4b00 0000 722b  A...rB...rK...r+
-00000e20: 0000 0072 2b00 0000 722c 0000 0072 4300  ...r+...r,...rC.
+00000e00: 723a 0000 0072 3b00 0000 723d 0000 0072  r:...r;...r=...r
+00000e10: 3e00 0000 723f 0000 0072 4700 0000 722b  >...r?...rG...r+
+00000e20: 0000 0072 2b00 0000 722c 0000 0072 4000  ...r+...r,...r@.
 00000e30: 0000 6b00 0000 731c 0000 000c 010a 010e  ..k...s.........
 00000e40: 0114 0112 0110 0108 020e 0112 0112 0112  ................
 00000e50: 0110 0210 0114 027a 1d52 6563 6f72 6469  .......z.Recordi
 00000e60: 6e67 5769 6467 6574 2e70 6c61 6365 5f77  ngWidget.place_w
 00000e70: 6964 6765 7473 6301 0000 0000 0000 0000  idgetsc.........
 00000e80: 0000 0001 0000 0003 0000 0043 0000 0073  ...........C...s
-00000e90: 5600 0000 7c00 6a00 6a01 a002 7c00 6a03  V...|.j.j...|.j.
+00000e90: 5800 0000 7c00 6a00 6a01 a002 7c00 6a03  X...|.j.j...|.j.
 00000ea0: a101 0100 7c00 6a04 6a05 a002 7c00 6a06  ....|.j.j...|.j.
 00000eb0: 6a07 a101 0100 7c00 6a00 6a08 a002 7c00  j.....|.j.j...|.
 00000ec0: 6a09 a101 0100 7c00 6a0a 6a0b a002 7c00  j.....|.j.j...|.
-00000ed0: 6a0c a101 0100 7c00 6a06 6a0d a002 7c00  j.....|.j.j...|.
-00000ee0: 6a0e a101 0100 6400 5300 a901 4e29 0f72  j.....d.S...N).r
-00000ef0: 3500 0000 da0e 496d 6167 6542 726f 6164  5.....ImageBroad
-00000f00: 6361 7374 da07 636f 6e6e 6563 74da 0f49  cast..connect..I
-00000f10: 6d61 6765 5570 6461 7465 536c 6f74 7238  mageUpdateSlotr8
-00000f20: 0000 00da 0c76 616c 7565 4368 616e 6765  .....valueChange
-00000f30: 6472 2e00 0000 da13 7365 745f 6163 7469  dr......set_acti
-00000f40: 7665 5f6d 6f64 655f 6670 73da 0b64 726f  ve_mode_fps..dro
-00000f50: 7070 6564 5f66 7073 da12 7570 6461 7465  pped_fps..update
-00000f60: 5f64 726f 7070 6564 5f66 7073 723d 0000  _dropped_fpsr=..
-00000f70: 00da 0763 6c69 636b 6564 da11 746f 6767  ...clicked..togg
-00000f80: 6c65 5f73 7461 7274 5f73 746f 70da 1972  le_start_stop..r
-00000f90: 6563 6f72 6469 6e67 5f63 6f6d 706c 6574  ecording_complet
-00000fa0: 655f 7369 676e 616c da15 6f6e 5f72 6563  e_signal..on_rec
-00000fb0: 6f72 6469 6e67 5f63 6f6d 706c 6574 6572  ording_completer
-00000fc0: 4b00 0000 722b 0000 0072 2b00 0000 722c  K...r+...r+...r,
-00000fd0: 0000 0072 4400 0000 7f00 0000 730a 0000  ...rD.......s...
-00000fe0: 0010 0212 0110 0110 0114 017a 1f52 6563  ...........z.Rec
-00000ff0: 6f72 6469 6e67 5769 6467 6574 2e63 6f6e  ordingWidget.con
-00001000: 6e65 6374 5f77 6964 6765 7473 6301 0000  nect_widgetsc...
-00001010: 0000 0000 0000 0000 0002 0000 0004 0000  ................
-00001020: 0043 0000 0073 c600 0000 7c00 6a00 7401  .C...s....|.j.t.
-00001030: 6a02 6b02 722f 7401 6a03 7c00 5f00 7c00  j.k.r/t.j.|._.|.
-00001040: 6a04 a005 7c00 6a00 6a06 a101 0100 7c00  j...|.j.j.....|.
-00001050: 6a07 a008 6401 a101 0100 7409 a00a 6402  j...d.....t...d.
-00001060: a101 0100 740b 7c00 6a0c 6a0d 7c00 6a07  ....t.|.j.j.|.j.
-00001070: a00e a100 8302 7d01 7c00 6a0c a00f 7c01  ......}.|.j...|.
-00001080: a101 0100 6400 5300 7c00 6a00 7401 6a03  ....d.S.|.j.t.j.
-00001090: 6b02 7261 7c00 6a04 a008 6401 a101 0100  k.ra|.j...d.....
-000010a0: 7401 6a10 7c00 5f00 7c00 6a04 a005 7c00  t.j.|._.|.j...|.
-000010b0: 6a00 6a06 a101 0100 7c00 6a0c a011 a100  j.j.....|.j.....
-000010c0: 0100 7c00 6a07 a008 6403 a101 0100 7409  ..|.j...d.....t.
-000010d0: a00a 6404 a101 0100 7c00 6a07 a005 7c00  ..d.....|.j...|.
-000010e0: a012 a100 a101 0100 6400 5300 6400 5300  ........d.S.d.S.
-000010f0: 2905 4e46 7a12 496e 6974 6961 7465 2072  ).NFz.Initiate r
-00001100: 6563 6f72 6469 6e67 547a 2e53 746f 7020  ecordingTz.Stop 
-00001110: 7265 636f 7264 696e 6720 616e 6420 696e  recording and in
-00001120: 6974 6961 7465 2066 696e 616c 2073 6176  itiate final sav
-00001130: 6520 6f66 2066 696c 6529 1372 3b00 0000  e of file).r;...
-00001140: 7224 0000 0072 2800 0000 7229 0000 0072  r$...r(...r)...r
-00001150: 3d00 0000 da07 7365 7454 6578 7472 3c00  =.....setTextr<.
-00001160: 0000 7240 0000 0072 4a00 0000 da06 6c6f  ..r@...rJ.....lo
-00001170: 6767 6572 da04 696e 666f 7202 0000 0072  gger..infor....r
-00001180: 2e00 0000 725c 0000 00da 0474 6578 74da  ....r\.....text.
-00001190: 0f73 7461 7274 5f72 6563 6f72 6469 6e67  .start_recording
-000011a0: 722a 0000 00da 0e73 746f 705f 7265 636f  r*.....stop_reco
-000011b0: 7264 696e 6772 3f00 0000 2902 7246 0000  rdingr?...).rF..
-000011c0: 005a 0e72 6563 6f72 6469 6e67 5f70 6174  .Z.recording_pat
-000011d0: 6872 2b00 0000 722b 0000 0072 2c00 0000  hr+...r+...r,...
-000011e0: 726f 0000 0087 0000 0073 2000 0000 0c01  ro.......s .....
-000011f0: 0801 1001 0c01 0a02 1401 1001 0c02 0c01  ................
-00001200: 0802 1002 0a01 0c02 0a01 1401 04f6 7a21  ..............z!
-00001210: 5265 636f 7264 696e 6757 6964 6765 742e  RecordingWidget.
-00001220: 746f 6767 6c65 5f73 7461 7274 5f73 746f  toggle_start_sto
-00001230: 7063 0100 0000 0000 0000 0000 0000 0100  pc..............
-00001240: 0000 0300 0000 4300 0000 733c 0000 0074  ......C...s<...t
-00001250: 00a0 0164 01a1 0101 0074 026a 037c 005f  ...d.....t.j.|._
-00001260: 047c 006a 05a0 067c 006a 046a 07a1 0101  .|.j...|.j.j....
-00001270: 007c 006a 05a0 0864 02a1 0101 0074 00a0  .|.j...d.....t..
-00001280: 0164 03a1 0101 0064 0053 0029 044e 7a44  .d.....d.S.).NzD
-00001290: 5265 636f 7264 696e 6720 636f 6d70 6c65  Recording comple
-000012a0: 7465 2073 6967 6e61 6c20 7265 6365 6976  te signal receiv
-000012b0: 6564 2e2e 2e75 7064 6174 696e 6720 6e65  ed...updating ne
-000012c0: 7874 2061 6374 696f 6e20 616e 6420 6275  xt action and bu
-000012d0: 7474 6f6e 547a 2445 6e61 626c 696e 6720  ttonTz$Enabling 
-000012e0: 7374 6172 742f 7374 6f70 2072 6563 6f72  start/stop recor
-000012f0: 6469 6e67 2062 7574 746f 6e29 0972 7300  ding button).rs.
-00001300: 0000 7274 0000 0072 2400 0000 7228 0000  ..rt...r$...r(..
-00001310: 0072 3b00 0000 723d 0000 0072 7200 0000  .r;...r=...rr...
-00001320: 723c 0000 0072 4a00 0000 724b 0000 0072  r<...rJ...rK...r
-00001330: 2b00 0000 722b 0000 0072 2c00 0000 7271  +...r+...r,...rq
-00001340: 0000 009d 0000 0073 0a00 0000 0a01 0801  .......s........
-00001350: 1001 0c01 0e01 7a25 5265 636f 7264 696e  ......z%Recordin
-00001360: 6757 6964 6765 742e 6f6e 5f72 6563 6f72  gWidget.on_recor
-00001370: 6469 6e67 5f63 6f6d 706c 6574 6572 6c00  ding_completerl.
-00001380: 0000 6302 0000 0000 0000 0000 0000 0005  ..c.............
-00001390: 0000 0006 0000 0043 0000 0073 3c00 0000  .......C...s<...
-000013a0: 6401 7d02 7c01 a000 a100 4400 5d0f 5c02  d.}.|.....D.].\.
-000013b0: 7d03 7d04 7c02 7c03 9b00 6402 7c04 6403  }.}.|.|...d.|.d.
-000013c0: 9b04 6404 9d04 3700 7d02 7106 7c00 6a01  ..d...7.}.q.|.j.
-000013d0: a002 7c02 a101 0100 6405 5300 2906 7a38  ..|.....d.S.).z8
-000013e0: 556e 7261 7665 6c20 6472 6f70 7065 6420  Unravel dropped 
-000013f0: 6670 7320 6469 6374 696f 6e61 7279 2074  fps dictionary t
-00001400: 6f20 6120 6d6f 7265 2072 6561 6461 626c  o a more readabl
-00001410: 6520 7374 7269 6e67 7a23 5261 7465 206f  e stringz#Rate o
-00001420: 6620 4672 616d 6520 4472 6f70 7069 6e67  f Frame Dropping
-00001430: 2062 7920 506f 7274 3a20 2020 207a 023a   by Port:    z.:
-00001440: 207a 032e 3025 7a08 2020 2020 2020 2020   z..0%z.        
-00001450: 4e29 03da 0569 7465 6d73 7241 0000 0072  N)...itemsrA...r
-00001460: 7200 0000 2905 7246 0000 0072 6c00 0000  r...).rF...rl...
-00001470: 7275 0000 00da 0470 6f72 745a 0964 726f  ru.....portZ.dro
-00001480: 705f 7261 7465 722b 0000 0072 2b00 0000  p_rater+...r+...
-00001490: 722c 0000 0072 6d00 0000 a400 0000 7308  r,...rm.......s.
-000014a0: 0000 0004 0210 0118 0110 027a 2252 6563  ...........z"Rec
-000014b0: 6f72 6469 6e67 5769 6467 6574 2e75 7064  ordingWidget.upd
-000014c0: 6174 655f 6472 6f70 7065 645f 6670 7363  ate_dropped_fpsc
-000014d0: 0200 0000 0000 0000 0000 0000 0300 0000  ................
-000014e0: 0400 0000 4300 0000 732c 0000 007c 006a  ....C...s,...|.j
-000014f0: 00a0 017c 006a 00a0 02a1 00a1 0101 0074  ...|.j.........t
-00001500: 03a0 047c 01a1 017d 027c 006a 00a0 057c  ...|...}.|.j...|
-00001510: 02a1 0101 0064 0053 0072 6600 0000 2906  .....d.S.rf...).
-00001520: 7242 0000 00da 0672 6573 697a 65da 0873  rB.....resize..s
-00001530: 697a 6548 696e 7472 0b00 0000 da09 6672  izeHintr......fr
-00001540: 6f6d 496d 6167 65da 0973 6574 5069 786d  omImage..setPixm
-00001550: 6170 2903 7246 0000 00da 0771 5f69 6d61  ap).rF.....q_ima
-00001560: 6765 da07 7170 6978 6d61 7072 2b00 0000  ge..qpixmapr+...
-00001570: 722b 0000 0072 2c00 0000 7269 0000 00ad  r+...r,...ri....
-00001580: 0000 0073 0600 0000 1201 0a01 1001 7a1f  ...s..........z.
-00001590: 5265 636f 7264 696e 6757 6964 6765 742e  RecordingWidget.
-000015a0: 496d 6167 6555 7064 6174 6553 6c6f 7429  ImageUpdateSlot)
-000015b0: 0f72 2500 0000 7226 0000 0072 2700 0000  .r%...r&...r'...
-000015c0: 721e 0000 0072 3000 0000 7245 0000 0072  r....r0...rE...r
-000015d0: 3f00 0000 7243 0000 0072 4400 0000 726f  ?...rC...rD...ro
-000015e0: 0000 0072 7100 0000 da04 6469 6374 726d  ...rq.....dictrm
-000015f0: 0000 0072 6900 0000 da0d 5f5f 636c 6173  ...ri.....__clas
-00001600: 7363 656c 6c5f 5f72 2b00 0000 722b 0000  scell__r+...r+..
-00001610: 0072 4700 0000 722c 0000 0072 2d00 0000  .rG...r,...r-...
-00001620: 3100 0000 7314 0000 0008 0012 0208 2008  1...s......... .
-00001630: 0708 1108 1408 0808 160e 0710 0972 2d00  .............r-.
-00001640: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-00001650: 0000 0004 0000 0040 0000 0073 4400 0000  .......@...sD...
-00001660: 6500 5a01 6400 5a02 6410 6402 6503 6602  e.Z.d.Z.d.d.e.f.
-00001670: 6403 6404 8405 5a04 6405 6406 8400 5a05  d.d...Z.d.d...Z.
-00001680: 6407 6408 8400 5a06 6409 640a 8400 5a07  d.d...Z.d.d...Z.
-00001690: 640b 640c 8400 5a08 640d 640e 8400 5a09  d.d...Z.d.d...Z.
-000016a0: 640f 5300 2911 7232 0000 00e9 fa00 0000  d.S.).r2........
-000016b0: 7231 0000 0063 0300 0000 0000 0000 0000  r1...c..........
-000016c0: 0000 0600 0000 0500 0000 4300 0000 738c  ..........C...s.
-000016d0: 0000 007c 017c 005f 007c 027c 005f 0167  ...|.|._.|.|._.g
-000016e0: 007c 005f 027c 006a 006a 03a0 04a1 0044  .|._.|.j.j.....D
-000016f0: 005d 0a5c 027d 037d 047c 006a 02a0 057c  .].\.}.}.|.j...|
-00001700: 03a1 0101 0071 0f7c 006a 02a0 06a1 0001  .....q.|.j......
-00001710: 0074 077c 006a 0283 017d 0574 0874 09a0  .t.|.j...}.t.t..
-00001720: 0a7c 0564 0113 00a1 0183 017c 005f 0b74  .|.d.......|._.t
-00001730: 0874 09a0 0a7c 057c 006a 0b1b 00a1 0183  .t...|.|.j......
-00001740: 017c 005f 0c74 0d83 007c 005f 0e7c 006a  .|._.t...|._.|.j
-00001750: 00a0 0f7c 006a 0ea1 0101 0064 0053 0029  ...|.j.....d.S.)
-00001760: 024e 6700 0000 0000 00e0 3f29 1072 3100  .Ng.......?).r1.
-00001770: 0000 da13 7369 6e67 6c65 5f66 7261 6d65  ....single_frame
-00001780: 5f68 6569 6768 74da 0570 6f72 7473 da07  _height..ports..
-00001790: 7374 7265 616d 7372 7800 0000 da06 6170  streamsrx.....ap
-000017a0: 7065 6e64 da04 736f 7274 725e 0000 0072  pend..sortr^...r
-000017b0: 5a00 0000 da04 6d61 7468 da04 6365 696c  Z.....math..ceil
-000017c0: da0d 6672 616d 655f 636f 6c75 6d6e 73da  ..frame_columns.
-000017d0: 0a66 7261 6d65 5f72 6f77 7372 0500 0000  .frame_rowsr....
-000017e0: da16 6e65 775f 7379 6e63 5f70 6163 6b65  ..new_sync_packe
-000017f0: 745f 6e6f 7469 6365 da13 7375 6273 6372  t_notice..subscr
-00001800: 6962 655f 746f 5f6e 6f74 6963 6529 0672  ibe_to_notice).r
-00001810: 4600 0000 7231 0000 0072 8300 0000 7279  F...r1...r....ry
-00001820: 0000 00da 0673 7472 6561 6d5a 0c63 616d  .....streamZ.cam
-00001830: 6572 615f 636f 756e 7472 2b00 0000 722b  era_countr+...r+
-00001840: 0000 0072 2c00 0000 7230 0000 00b3 0000  ...r,...r0......
-00001850: 0073 1600 0000 0601 0601 0603 1401 0e03  .s..............
-00001860: 0a01 0a04 1401 1601 0802 1201 7a1d 556e  ............z.Un
-00001870: 7061 6972 6564 4672 616d 6542 7569 6c64  pairedFrameBuild
-00001880: 6572 2e5f 5f69 6e69 745f 5f63 0100 0000  er.__init__c....
-00001890: 0000 0000 0000 0000 0100 0000 0300 0000  ................
-000018a0: 4300 0000 731c 0000 0074 00a0 0164 01a1  C...s....t...d..
-000018b0: 0101 007c 006a 02a0 037c 006a 04a1 0101  ...|.j...|.j....
-000018c0: 0064 0053 0029 024e 7a2c 556e 7375 6273  .d.S.).Nz,Unsubs
-000018d0: 6372 6962 6520 6672 616d 6520 6275 696c  cribe frame buil
-000018e0: 6465 7220 6672 6f6d 2073 796e 6368 726f  der from synchro
-000018f0: 6e69 7a65 722e 2905 7273 0000 0072 7400  nizer.).rs...rt.
-00001900: 0000 7231 0000 00da 1575 6e73 7562 7363  ..r1.....unsubsc
-00001910: 7269 6265 5f74 6f5f 6e6f 7469 6365 728c  ribe_to_noticer.
-00001920: 0000 0072 4b00 0000 722b 0000 0072 2b00  ...rK...r+...r+.
-00001930: 0000 722c 0000 00da 1d75 6e73 7562 7363  ..r,.....unsubsc
-00001940: 7269 6265 5f66 726f 6d5f 7379 6e63 6872  ribe_from_synchr
-00001950: 6f6e 697a 6572 c800 0000 7304 0000 000a  onizer....s.....
-00001960: 0112 017a 3255 6e70 6169 7265 6446 7261  ...z2UnpairedFra
-00001970: 6d65 4275 696c 6465 722e 756e 7375 6273  meBuilder.unsubs
-00001980: 6372 6962 655f 6672 6f6d 5f73 796e 6368  cribe_from_synch
-00001990: 726f 6e69 7a65 7263 0200 0000 0000 0000  ronizerc........
-000019a0: 0000 0000 0400 0000 0400 0000 4300 0000  ............C...
-000019b0: 733c 0000 007c 006a 007d 027c 0164 0175  s<...|.j.}.|.d.u
-000019c0: 0072 1974 01a0 0264 02a1 0101 0074 036a  .r.t...d.....t.j
-000019d0: 047c 027c 0264 0366 0374 036a 0564 048d  .|.|.d.f.t.j.d..
-000019e0: 027d 037c 0353 007c 016a 067d 037c 0353  .}.|.S.|.j.}.|.S
-000019f0: 0029 057a 7b53 796e 6368 726f 6e69 7a61  .).z{Synchroniza
-00001a00: 7469 6f6e 2069 7373 7565 7320 6361 6e20  tion issues can 
-00001a10: 6c65 6164 2074 6f20 736f 6d65 2066 7261  lead to some fra
-00001a20: 6d65 7320 6265 696e 6720 4e6f 6e65 2061  mes being None a
-00001a30: 6d6f 6e67 0a20 2020 2020 2020 2074 6865  mong.        the
-00001a40: 2073 796e 6368 6564 2066 7261 6d65 732c   synched frames,
-00001a50: 2073 6f20 706c 7567 2074 6861 7420 7769   so plug that wi
-00001a60: 7468 2061 2062 6c61 6e6b 2066 7261 6d65  th a blank frame
-00001a70: 4e7a 1970 6c75 6767 696e 6720 626c 616e  Nz.plugging blan
-00001a80: 6b20 6672 616d 6520 6461 7461 e903 0000  k frame data....
-00001a90: 0029 01da 0564 7479 7065 2907 7283 0000  .)...dtype).r...
-00001aa0: 0072 7300 0000 da05 6465 6275 67da 026e  .rs.....debug..n
-00001ab0: 70da 057a 6572 6f73 da05 7569 6e74 38da  p..zeros..uint8.
-00001ac0: 0566 7261 6d65 2904 7246 0000 00da 0c66  .frame).rF.....f
-00001ad0: 7261 6d65 5f70 6163 6b65 74da 0465 6467  rame_packet..edg
-00001ae0: 6572 9700 0000 722b 0000 0072 2b00 0000  er....r+...r+...
-00001af0: 722c 0000 00da 1267 6574 5f66 7261 6d65  r,.....get_frame
-00001b00: 5f6f 725f 626c 616e 6bcd 0000 0073 0e00  _or_blank....s..
-00001b10: 0000 0604 0802 0a01 1601 0404 06fe 0402  ................
-00001b20: 7a27 556e 7061 6972 6564 4672 616d 6542  z'UnpairedFrameB
-00001b30: 7569 6c64 6572 2e67 6574 5f66 7261 6d65  uilder.get_frame
-00001b40: 5f6f 725f 626c 616e 6b63 0200 0000 0000  _or_blankc......
-00001b50: 0000 0000 0000 0800 0000 0900 0000 4300  ..............C.
-00001b60: 0000 7386 0000 0074 00a0 0164 01a1 0101  ..s....t...d....
-00001b70: 007c 016a 0264 0219 007d 027c 016a 0264  .|.j.d...}.|.j.d
-00001b80: 0319 007d 0374 037c 027c 0383 027d 0474  ...}.t.|.|...}.t
-00001b90: 047c 047c 0218 0064 041b 0083 017d 0574  .|.|...d.....}.t
-00001ba0: 047c 047c 0318 0064 041b 0083 017d 0667  .|.|...d.....}.g
-00001bb0: 0064 05a2 017d 0774 00a0 0164 06a1 0101  .d...}.t...d....
-00001bc0: 0074 056a 067c 017c 057c 057c 067c 0674  .t.j.|.|.|.|.|.t
-00001bd0: 056a 077c 0764 078d 077d 0174 087c 017c  .j.|.d...}.t.|.|
-00001be0: 006a 0964 088d 027d 017c 0153 0029 097a  .j.d...}.|.S.).z
-00001bf0: 6554 6f20 6d61 6b65 2073 7572 6520 7468  eTo make sure th
-00001c00: 6174 2066 7261 6d65 7320 616c 6967 6e20  at frames align 
-00001c10: 7765 6c6c 2c20 7363 616c 6520 7468 656d  well, scale them
-00001c20: 2061 6c6c 2074 6f20 7468 756d 626e 6169   all to thumbnai
-00001c30: 6c73 0a20 2020 2020 2020 2073 7175 6172  ls.        squar
-00001c40: 6573 2077 6974 6820 626c 6163 6b20 626f  es with black bo
-00001c50: 7264 6572 732e 7a0f 7265 7369 7a69 6e67  rders.z.resizing
-00001c60: 2073 7175 6172 6572 0100 0000 7257 0000   squarer....rW..
-00001c70: 00e9 0200 0000 2903 7201 0000 0072 0100  ......).r....r..
-00001c80: 0000 7201 0000 007a 1361 626f 7574 2074  ..r....z.about t
-00001c90: 6f20 7061 6420 626f 7264 6572 2901 723c  o pad border).r<
-00001ca0: 0000 0029 01da 0a6e 6577 5f68 6569 6768  ...)...new_heigh
-00001cb0: 7429 0a72 7300 0000 7293 0000 00da 0573  t).rs...r......s
-00001cc0: 6861 7065 7260 0000 0072 5a00 0000 da03  haper`...rZ.....
-00001cd0: 6376 32da 0e63 6f70 794d 616b 6542 6f72  cv2..copyMakeBor
-00001ce0: 6465 72da 0f42 4f52 4445 525f 434f 4e53  der..BORDER_CONS
-00001cf0: 5441 4e54 727a 0000 0072 8300 0000 2908  TANTrz...r....).
-00001d00: 7246 0000 0072 9700 0000 da06 6865 6967  rF...r......heig
-00001d10: 6874 da05 7769 6474 68da 0b70 6164 6465  ht..width..padde
-00001d20: 645f 7369 7a65 da0a 6865 6967 6874 5f70  d_size..height_p
-00001d30: 6164 da09 7769 6474 685f 7061 64da 0970  ad..width_pad..p
-00001d40: 6164 5f63 6f6c 6f72 722b 0000 0072 2b00  ad_colorr+...r+.
-00001d50: 0000 722c 0000 00da 1072 6573 697a 655f  ..r,.....resize_
-00001d60: 746f 5f73 7175 6172 65dc 0000 0073 2600  to_square....s&.
-00001d70: 0000 0a03 0a04 0a01 0a02 1002 1001 0801  ................
-00001d80: 0a02 0401 0201 0201 0201 0201 0201 0401  ................
-00001d90: 0201 06f9 0e0a 0401 7a25 556e 7061 6972  ........z%Unpair
-00001da0: 6564 4672 616d 6542 7569 6c64 6572 2e72  edFrameBuilder.r
-00001db0: 6573 697a 655f 746f 5f73 7175 6172 6563  esize_to_squarec
-00001dc0: 0300 0000 0000 0000 0000 0000 0400 0000  ................
-00001dd0: 0400 0000 4300 0000 736c 0000 007c 006a  ....C...sl...|.j
-00001de0: 006a 017c 0219 006a 026a 037d 037c 0364  .j.|...j.j.}.|.d
-00001df0: 016b 0272 0f09 007c 0153 007c 0364 0276  .k.r...|.S.|.d.v
-00001e00: 0072 1c74 04a0 057c 0174 046a 06a1 027d  .r.t...|.t.j...}
-00001e10: 017c 0153 007c 0364 0376 0072 2974 04a0  .|.S.|.d.v.r)t..
-00001e20: 057c 0174 046a 07a1 027d 017c 0153 007c  .|.t.j...}.|.S.|
-00001e30: 0364 0476 0072 3474 04a0 057c 0174 046a  .d.v.r4t...|.t.j
-00001e40: 08a1 027d 017c 0153 0029 054e 7201 0000  ...}.|.S.).Nr...
-00001e50: 0029 0272 5700 0000 e9fd ffff ff29 0272  .).rW........).r
-00001e60: 9b00 0000 e9fe ffff ff29 02e9 ffff ffff  .........)......
-00001e70: 7291 0000 0029 0972 3100 0000 7285 0000  r....).r1...r...
-00001e80: 00da 0663 616d 6572 61da 0e72 6f74 6174  ...camera..rotat
-00001e90: 696f 6e5f 636f 756e 7472 9e00 0000 da06  ion_countr......
-00001ea0: 726f 7461 7465 da13 524f 5441 5445 5f39  rotate..ROTATE_9
-00001eb0: 305f 434c 4f43 4b57 4953 45da 0a52 4f54  0_CLOCKWISE..ROT
-00001ec0: 4154 455f 3138 30da 1a52 4f54 4154 455f  ATE_180..ROTATE_
-00001ed0: 3930 5f43 4f55 4e54 4552 434c 4f43 4b57  90_COUNTERCLOCKW
-00001ee0: 4953 4529 0472 4600 0000 7297 0000 0072  ISE).rF...r....r
-00001ef0: 7900 0000 72ac 0000 0072 2b00 0000 722b  y...r....r+...r+
-00001f00: 0000 0072 2c00 0000 da0e 6170 706c 795f  ...r,.....apply_
-00001f10: 726f 7461 7469 6f6e fb00 0000 731a 0000  rotation....s...
-00001f20: 0010 0208 0102 0104 0808 f90e 0104 0608  ................
-00001f30: fb0e 0104 0408 fd0e 0104 027a 2355 6e70  ...........z#Unp
-00001f40: 6169 7265 6446 7261 6d65 4275 696c 6465  airedFrameBuilde
-00001f50: 722e 6170 706c 795f 726f 7461 7469 6f6e  r.apply_rotation
-00001f60: 6301 0000 0000 0000 0000 0000 0011 0000  c...............
-00001f70: 000a 0000 0043 0000 0073 7801 0000 7c00  .....C...sx...|.
-00001f80: 6a00 a001 a100 0100 7c00 6a02 6a03 7c00  j.......|.j.j.|.
-00001f90: 5f03 6900 7d01 7c00 6a04 4400 5d3f 7d02  _.i.}.|.j.D.]?}.
-00001fa0: 7c00 6a03 6a05 7c02 1900 7d03 7c00 a006  |.j.j.|...}.|...
-00001fb0: 7c03 a101 7d04 7c00 a007 7c04 a101 7d05  |...}.|...|...}.
-00001fc0: 7c00 a008 7c05 7c02 a102 7d06 7409 a00a  |...|.|...}.t...
-00001fd0: 7c06 6401 a102 7d07 7409 6a0b 7c07 740c  |.d...}.t.j.|.t.
-00001fe0: 7c02 8301 740d 7c07 6a0e 6401 1900 6402  |...t.|.j.d...d.
-00001ff0: 1b00 8301 740d 7c00 6a0f 6403 1b00 8301  ....t.|.j.d.....
-00002000: 6602 7409 6a10 6401 6404 6402 6405 8d07  f.t.j.d.d.d.d...
-00002010: 7d08 7c08 7c01 7c02 3c00 710f 6700 7d09  }.|.|.|.<.q.g.}.
-00002020: 6406 7d0a 6407 7d0b 6407 7d0c 7411 7c00  d.}.d.}.d.}.t.|.
-00002030: 6a04 8301 7d0d 7c01 a012 a100 4400 5d44  j...}.|.....D.]D
-00002040: 5c02 7d02 7d0e 7c0a 6406 7500 726b 7c0e  \.}.}.|.d.u.rk|.
-00002050: 7d0a 6e07 7413 a014 7c0a 7c0e 6702 a101  }.n.t...|.|.g...
-00002060: 7d0a 7c0b 6401 3700 7d0b 7c0d 6401 3800  }.|.d.7.}.|.d.8.
-00002070: 7d0d 7c0d 6407 6b02 7296 7c0b 7c00 6a15  }.|.d.k.r.|.|.j.
-00002080: 6b00 7296 7413 a014 7c0a 7c00 a006 6406  k.r.t...|.|...d.
-00002090: a101 6702 a101 7d0a 7c0b 6401 3700 7d0b  ..g...}.|.d.7.}.
-000020a0: 7c0b 7c00 6a15 6b00 7383 7c0b 7c00 6a15  |.|.j.k.s.|.|.j.
-000020b0: 6b02 72a4 7c09 a016 7c0a a101 0100 6406  k.r.|...|.....d.
-000020c0: 7d0a 6407 7d0b 7160 6406 7d0f 7c09 4400  }.d.}.q`d.}.|.D.
-000020d0: 5d10 7d10 7c0f 6406 7500 72b2 7c10 7d0f  ].}.|.d.u.r.|.}.
-000020e0: 71a9 7413 a017 7c0f 7c10 6702 a101 7d0f  q.t...|.|.g...}.
-000020f0: 71a9 7c0f 5300 2908 7afb 0a20 2020 2020  q.|.S.).z..     
-00002100: 2020 2054 6869 7320 676c 7565 7320 746f     This glues to
-00002110: 6765 7468 6572 2074 6865 2069 6e64 6976  gether the indiv
-00002120: 6964 7561 6c20 6672 616d 6573 2069 6e20  idual frames in 
-00002130: 7468 6520 7379 6e63 2070 6163 6b65 7420  the sync packet 
-00002140: 696e 746f 206f 6e65 206c 6172 6765 2062  into one large b
-00002150: 6c6f 636b 0a0a 2020 2020 2020 2020 4375  lock..        Cu
-00002160: 7272 656e 746c 7920 6a75 7374 2073 7461  rrently just sta
-00002170: 636b 696e 6720 616c 6c20 6672 616d 6573  cking all frames
-00002180: 2076 6572 7469 6361 6c6c 792c 2062 7574   vertically, but
-00002190: 2074 6869 7320 7368 6f75 6c64 2062 6520   this should be 
-000021a0: 6578 7061 6e64 6564 206f 6e20 7468 6520  expanded on the 
-000021b0: 0a20 2020 2020 2020 2074 6865 2066 7574  .        the fut
-000021c0: 7572 6520 746f 2061 6c6c 6f77 2077 7261  ure to allow wra
-000021d0: 7070 696e 6720 746f 2061 206d 6f72 6520  pping to a more 
-000021e0: 7371 7561 7265 2073 6861 7065 0a20 2020  square shape.   
-000021f0: 2020 2020 2072 5700 0000 729b 0000 00e9       rW...r.....
-00002200: 0400 0000 2903 7201 0000 0072 0100 0000  ....).r....r....
-00002210: e9ff 0000 0029 04da 0866 6f6e 7446 6163  .....)...fontFac
-00002220: 65da 0966 6f6e 7453 6361 6c65 da05 636f  e..fontScale..co
-00002230: 6c6f 72da 0974 6869 636b 6e65 7373 4e72  lor..thicknessNr
-00002240: 0100 0000 2918 728c 0000 00da 0367 6574  ....).r......get
-00002250: 7231 0000 00da 1363 7572 7265 6e74 5f73  r1.....current_s
-00002260: 796e 635f 7061 636b 6574 7284 0000 00da  ync_packetr.....
-00002270: 0d66 7261 6d65 5f70 6163 6b65 7473 729a  .frame_packetsr.
-00002280: 0000 0072 a700 0000 72b1 0000 0072 9e00  ...r....r....r..
-00002290: 0000 da04 666c 6970 da07 7075 7454 6578  ....flip..putTex
-000022a0: 7472 5f00 0000 725a 0000 0072 9d00 0000  tr_...rZ...r....
-000022b0: 7283 0000 00da 1446 4f4e 545f 4845 5253  r......FONT_HERS
-000022c0: 4845 595f 5349 4d50 4c45 5872 5e00 0000  HEY_SIMPLEXr^...
-000022d0: 7278 0000 0072 9400 0000 da06 6873 7461  rx...r......hsta
-000022e0: 636b 728a 0000 0072 8600 0000 da06 7673  ckr....r......vs
-000022f0: 7461 636b 2911 7246 0000 005a 1074 6875  tack).rF...Z.thu
-00002300: 6d62 6e61 696c 5f66 7261 6d65 7372 7900  mbnail_framesry.
-00002310: 0000 7298 0000 005a 0972 6177 5f66 7261  ..r....Z.raw_fra
-00002320: 6d65 5a0c 7371 7561 7265 5f66 7261 6d65  meZ.square_frame
-00002330: 5a0d 726f 7461 7465 645f 6672 616d 655a  Z.rotated_frameZ
-00002340: 0d66 6c69 7070 6564 5f66 7261 6d65 5a0a  .flipped_frameZ.
-00002350: 7465 7874 5f66 7261 6d65 728b 0000 005a  text_framer....Z
-00002360: 0b63 7572 7265 6e74 5f72 6f77 5a12 6375  .current_rowZ.cu
-00002370: 7272 656e 745f 726f 775f 6c65 6e67 7468  rrent_row_length
-00002380: 5a0c 6672 616d 6573 5f61 6464 6564 5a10  Z.frames_addedZ.
-00002390: 6672 616d 6573 5f72 656d 6169 6e69 6e67  frames_remaining
-000023a0: 7297 0000 005a 0a6d 6567 615f 6672 616d  r....Z.mega_fram
-000023b0: 65da 0372 6f77 722b 0000 0072 2b00 0000  e..rowr+...r+...
-000023c0: 722c 0000 00da 1367 6574 5f72 6563 6f72  r,.....get_recor
-000023d0: 6469 6e67 5f66 7261 6d65 0a01 0000 735a  ding_frame....sZ
-000023e0: 0000 000a 080a 0104 020a 010c 010a 010a  ................
-000023f0: 010c 010c 0106 0306 011e 0104 0102 0102  ................
-00002400: 0102 0106 fa0a 0904 0204 0104 0104 010a  ................
-00002410: 0110 0108 0206 010e 0208 0108 0108 020a  ................
-00002420: 0214 0108 010a fe0a 040a 0104 0104 0102  ................
-00002430: 8004 0208 0108 0106 0110 0204 037a 2855  .............z(U
-00002440: 6e70 6169 7265 6446 7261 6d65 4275 696c  npairedFrameBuil
-00002450: 6465 722e 6765 745f 7265 636f 7264 696e  der.get_recordin
-00002460: 675f 6672 616d 654e 2901 7282 0000 0029  g_frameN).r....)
-00002470: 0a72 2500 0000 7226 0000 0072 2700 0000  .r%...r&...r'...
-00002480: 7220 0000 0072 3000 0000 7290 0000 0072  r ...r0...r....r
-00002490: 9a00 0000 72a7 0000 0072 b100 0000 72c1  ....r....r....r.
-000024a0: 0000 0072 2b00 0000 722b 0000 0072 2b00  ...r+...r+...r+.
-000024b0: 0000 722c 0000 0072 3200 0000 b200 0000  ..r,...r2.......
-000024c0: 730e 0000 0008 0010 0108 1508 0508 0f08  s...............
-000024d0: 1f0c 0f72 3200 0000 6300 0000 0000 0000  ...r2...c.......
-000024e0: 0000 0000 0000 0000 0004 0000 0000 0000  ................
-000024f0: 0073 3a00 0000 6500 5a01 6400 5a02 6503  .s:...e.Z.d.Z.e.
-00002500: 6504 8301 5a05 6503 6506 8301 5a07 6401  e...Z.e.e...Z.d.
-00002510: 6508 6602 8700 6601 6402 6403 840c 5a09  e.f...f.d.d...Z.
-00002520: 6404 6405 8400 5a0a 8700 0400 5a0b 5300  d.d...Z.....Z.S.
-00002530: 2906 7234 0000 0072 3300 0000 6302 0000  ).r4...r3...c...
-00002540: 0000 0000 0000 0000 0002 0000 0003 0000  ................
-00002550: 0003 0000 0073 2a00 0000 7400 7401 7c00  .....s*...t.t.|.
-00002560: 8302 a002 a100 0100 7c01 7c00 5f03 7404  ........|.|._.t.
-00002570: a005 6401 a101 0100 7406 8300 7c00 5f07  ..d.....t...|._.
-00002580: 6400 5300 2902 4e7a 2149 6e69 7469 6174  d.S.).Nz!Initiat
-00002590: 6564 2072 6563 6f72 6469 6e67 2066 7261  ed recording fra
-000025a0: 6d65 2065 6d69 7474 6572 2908 722f 0000  me emitter).r/..
-000025b0: 0072 3400 0000 7230 0000 00da 1772 6563  .r4...r0.....rec
-000025c0: 6f72 6469 6e67 5f66 7261 6d65 5f62 7569  ording_frame_bui
-000025d0: 6c64 6572 7273 0000 0072 7400 0000 7204  lderrs...rt...r.
-000025e0: 0000 00da 0f6b 6565 705f 636f 6c6c 6563  .....keep_collec
-000025f0: 7469 6e67 2902 7246 0000 0072 3300 0000  ting).rF...r3...
-00002600: 7247 0000 0072 2b00 0000 722c 0000 0072  rG...r+...r,...r
-00002610: 3000 0000 5001 0000 7308 0000 000e 0206  0...P...s.......
-00002620: 010a 010c 017a 1d55 6e70 6169 7265 6446  .....z.UnpairedF
-00002630: 7261 6d65 456d 6974 7465 722e 5f5f 696e  rameEmitter.__in
-00002640: 6974 5f5f 6301 0000 0000 0000 0000 0000  it__c...........
-00002650: 0003 0000 0003 0000 0043 0000 0073 6400  .........C...sd.
-00002660: 0000 7c00 6a00 a001 a100 0100 7c00 6a00  ..|.j.......|.j.
-00002670: a002 a100 722b 7c00 6a03 a004 a100 7d01  ....r+|.j.....}.
-00002680: 7c01 6400 7501 7226 7405 7c01 8301 7d02  |.d.u.r&t.|...}.
-00002690: 7c00 6a06 a007 7c02 a101 0100 7c00 6a08  |.j...|.....|.j.
-000026a0: a007 7c00 6a03 6a09 6a08 a101 0100 7c00  ..|.j.j.j.....|.
-000026b0: 6a00 a002 a100 730a 740a a00b 6401 a101  j.....s.t...d...
-000026c0: 0100 6400 5300 2902 4e7a 2753 7465 7265  ..d.S.).Nz'Stere
-000026d0: 6f66 7261 6d65 2065 6d69 7474 6572 2072  oframe emitter r
-000026e0: 756e 2074 6872 6561 6420 656e 6465 642e  un thread ended.
-000026f0: 2e2e 290c 72c3 0000 00da 0373 6574 da06  ..).r......set..
-00002700: 6973 5f73 6574 72c2 0000 0072 c100 0000  is_setr....r....
-00002710: da0d 6376 325f 746f 5f71 6c61 6265 6c72  ..cv2_to_qlabelr
-00002720: 6700 0000 da04 656d 6974 726c 0000 0072  g.....emitrl...r
-00002730: 3100 0000 7273 0000 0072 7400 0000 2903  1...rs...rt...).
-00002740: 7246 0000 005a 0f72 6563 6f72 6469 6e67  rF...Z.recording
-00002750: 5f66 7261 6d65 da05 696d 6167 6572 2b00  _frame..imager+.
-00002760: 0000 722b 0000 0072 2c00 0000 da03 7275  ..r+...r,.....ru
-00002770: 6e57 0100 0073 1200 0000 0a02 0a02 0a04  nW...s..........
-00002780: 0802 0801 0c01 1201 0af7 0e0b 7a18 556e  ............z.Un
-00002790: 7061 6972 6564 4672 616d 6545 6d69 7474  pairedFrameEmitt
-000027a0: 6572 2e72 756e 290c 7225 0000 0072 2600  er.run).r%...r&.
-000027b0: 0000 7227 0000 0072 0800 0000 720a 0000  ..r'...r....r...
-000027c0: 0072 6700 0000 7280 0000 0072 6c00 0000  .rg...r....rl...
-000027d0: 7232 0000 0072 3000 0000 72c9 0000 0072  r2...r0...r....r
-000027e0: 8100 0000 722b 0000 0072 2b00 0000 7247  ....r+...r+...rG
-000027f0: 0000 0072 2c00 0000 7234 0000 004c 0100  ...r,...r4...L..
-00002800: 0073 0a00 0000 0800 0801 0801 1202 1007  .s..............
-00002810: 7234 0000 0063 0200 0000 0000 0000 0000  r4...c..........
-00002820: 0000 0300 0000 0300 0000 0300 0000 731a  ..............s.
-00002830: 0000 0087 0066 0164 0164 0284 087c 00a0  .....f.d.d...|..
-00002840: 00a1 0044 0083 017d 027c 0253 0029 034e  ...D...}.|.S.).N
-00002850: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
-00002860: 0004 0000 0013 0000 0073 1c00 0000 6700  .........s....g.
-00002870: 7c00 5d0a 5c02 7d01 7d02 7c02 8800 6b00  |.].\.}.}.|...k.
-00002880: 7202 7c01 9102 7102 5300 722b 0000 0072  r.|...q.S.r+...r
-00002890: 2b00 0000 2903 724e 0000 00da 036b 6579  +...).rN.....key
-000028a0: 723c 0000 00a9 01da 0d6d 696e 5f74 6872  r<.......min_thr
-000028b0: 6573 686f 6c64 722b 0000 0072 2c00 0000  esholdr+...r,...
-000028c0: 7250 0000 006b 0100 0072 5b00 0000 7a23  rP...k...r[...z#
-000028d0: 6765 745f 656d 7074 795f 7061 6972 732e  get_empty_pairs.
-000028e0: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
-000028f0: 6d70 3e29 0172 7800 0000 2903 da0c 626f  mp>).rx...)...bo
-00002900: 6172 645f 636f 756e 7473 72cc 0000 00da  ard_countsr.....
-00002910: 0b65 6d70 7479 5f70 6169 7273 722b 0000  .empty_pairsr+..
-00002920: 0072 cb00 0000 722c 0000 00da 0f67 6574  .r....r,.....get
-00002930: 5f65 6d70 7479 5f70 6169 7273 6a01 0000  _empty_pairsj...
-00002940: 7304 0000 0016 0104 0172 cf00 0000 6302  s........r....c.
-00002950: 0000 0000 0000 0000 0000 0007 0000 0005  ................
-00002960: 0000 0043 0000 0073 4400 0000 7c00 6a00  ...C...sD...|.j.
-00002970: 6400 6401 8502 1900 5c02 7d02 7d03 7c01  d.d.....\.}.}.|.
-00002980: 7401 7c02 8301 1b00 7d04 7402 7c03 7c04  t.|.....}.t.|.|.
-00002990: 1400 8301 7c01 6602 7d05 7403 6a04 7c00  ....|.f.}.t.j.|.
-000029a0: 7c05 7403 6a05 6402 8d03 7d06 7c06 5300  |.t.j.d...}.|.S.
-000029b0: 2903 4e72 9b00 0000 2901 da0d 696e 7465  ).Nr....)...inte
-000029c0: 7270 6f6c 6174 696f 6e29 0672 9d00 0000  rpolation).r....
-000029d0: da05 666c 6f61 7472 5a00 0000 729e 0000  ..floatrZ...r...
-000029e0: 0072 7a00 0000 da0a 494e 5445 525f 4152  .rz.....INTER_AR
-000029f0: 4541 2907 72c8 0000 0072 9c00 0000 da0e  EA).r....r......
-00002a00: 6375 7272 656e 745f 6865 6967 6874 da0d  current_height..
-00002a10: 6375 7272 656e 745f 7769 6474 68da 0572  current_width..r
-00002a20: 6174 696f da03 6469 6dda 0772 6573 697a  atio..dim..resiz
-00002a30: 6564 722b 0000 0072 2b00 0000 722c 0000  edr+...r+...r,..
-00002a40: 0072 7a00 0000 6e01 0000 730a 0000 0012  .rz...n...s.....
-00002a50: 010c 0110 0112 0104 0172 7a00 0000 6301  .........rz...c.
-00002a60: 0000 0000 0000 0000 0000 0003 0000 0005  ................
-00002a70: 0000 0043 0000 0073 3200 0000 7400 a001  ...C...s2...t...
-00002a80: 7c00 7400 6a02 a102 7d01 7403 7c01 6a04  |.t.j...}.t.|.j.
-00002a90: 7c01 6a05 6401 1900 7c01 6a05 6402 1900  |.j.d...|.j.d...
-00002aa0: 7403 6a06 6a07 8304 7d02 7c02 5300 2903  t.j.j...}.|.S.).
-00002ab0: 4e72 5700 0000 7201 0000 0029 0872 9e00  NrW...r....).r..
-00002ac0: 0000 da08 6376 7443 6f6c 6f72 da0d 434f  ....cvtColor..CO
-00002ad0: 4c4f 525f 4247 5232 5247 4272 0a00 0000  LOR_BGR2RGBr....
-00002ae0: da04 6461 7461 729d 0000 00da 0646 6f72  ..datar......For
-00002af0: 6d61 74da 0d46 6f72 6d61 745f 5247 4238  mat..Format_RGB8
-00002b00: 3838 2903 7297 0000 0072 c800 0000 da08  88).r....r......
-00002b10: 7174 5f66 7261 6d65 722b 0000 0072 2b00  qt_framer+...r+.
-00002b20: 0000 722c 0000 0072 c600 0000 7701 0000  ..r,...r....w...
-00002b30: 7310 0000 000e 0102 0204 0108 0108 0106  s...............
-00002b40: 0104 fc04 0672 c600 0000 6301 0000 0000  .....r....c.....
-00002b50: 0000 0000 0000 0005 0000 0004 0000 0043  ...............C
-00002b60: 0000 0073 4800 0000 7400 7c00 8301 7d01  ...sH...t.|...}.
-00002b70: 7401 7c01 8301 7d02 7c02 a002 7403 6a04  t.|...}.|...t.j.
-00002b80: a101 0100 7405 7406 6a07 8301 7d03 7408  ....t.t.j...}.t.
-00002b90: 7c02 8301 7d04 7c04 a009 a100 0100 7406  |...}.|.......t.
-00002ba0: a00a 7c03 a00b a100 a101 0100 6400 5300  ..|.........d.S.
-00002bb0: 7266 0000 0029 0c72 2300 0000 721e 0000  rf...).r#...r...
-00002bc0: 00da 0873 6574 5f6d 6f64 6572 1f00 0000  ...set_moder....
-00002bd0: da09 5265 636f 7264 696e 6772 0d00 0000  ..Recordingr....
-00002be0: da03 7379 73da 0461 7267 7672 2d00 0000  ..sys..argvr-...
-00002bf0: da04 7368 6f77 da04 6578 6974 da04 6578  ..show..exit..ex
-00002c00: 6563 2905 da0c 7365 7373 696f 6e5f 7061  ec)...session_pa
-00002c10: 7468 da06 636f 6e66 6967 722e 0000 00da  th..configr.....
-00002c20: 0341 7070 5a10 7265 636f 7264 696e 675f  .AppZ.recording_
-00002c30: 6469 616c 6f67 722b 0000 0072 2b00 0000  dialogr+...r+...
-00002c40: 722c 0000 00da 176c 6175 6e63 685f 7265  r,.....launch_re
-00002c50: 636f 7264 696e 675f 7769 6467 6574 8301  cording_widget..
-00002c60: 0000 730e 0000 0008 0108 010c 030a 0108  ..s.............
-00002c70: 0108 0112 0272 e800 0000 293f da0d 7079  .....r....)?..py
-00002c80: 7879 3364 2e6c 6f67 6765 72da 0670 7978  xy3d.logger..pyx
-00002c90: 7933 6472 7300 0000 72b8 0000 0072 2500  y3drs...r....r%.
-00002ca0: 0000 72e0 0000 0072 8800 0000 da07 7061  ..r....r......pa
-00002cb0: 7468 6c69 6272 0200 0000 da09 7468 7265  thlibr......thre
-00002cc0: 6164 696e 6772 0300 0000 7204 0000 00da  adingr....r.....
-00002cd0: 056e 756d 7079 7294 0000 00da 0571 7565  .numpyr......que
-00002ce0: 7565 7205 0000 00da 0465 6e75 6d72 0600  uer......enumr..
-00002cf0: 0000 729e 0000 00da 0c50 7951 7436 2e51  ..r......PyQt6.Q
-00002d00: 7443 6f72 6572 0700 0000 7208 0000 0072  tCorer....r....r
-00002d10: 0900 0000 5a0b 5079 5174 362e 5174 4775  ....Z.PyQt6.QtGu
-00002d20: 6972 0a00 0000 720b 0000 0072 0c00 0000  ir....r....r....
-00002d30: da0f 5079 5174 362e 5174 5769 6467 6574  ..PyQt6.QtWidget
-00002d40: 7372 0d00 0000 720e 0000 0072 0f00 0000  sr....r....r....
-00002d50: 7210 0000 0072 1100 0000 7212 0000 0072  r....r....r....r
-00002d60: 1300 0000 7214 0000 0072 1500 0000 7216  ....r....r....r.
-00002d70: 0000 0072 1700 0000 7218 0000 0072 1900  ...r....r....r..
-00002d80: 0000 721a 0000 0072 1b00 0000 721c 0000  ..r....r....r...
-00002d90: 0072 1d00 0000 da16 7079 7879 3364 2e73  .r......pyxy3d.s
-00002da0: 6573 7369 6f6e 2e73 6573 7369 6f6e 721e  ession.sessionr.
-00002db0: 0000 0072 1f00 0000 da1b 7079 7879 3364  ...r......pyxy3d
-00002dc0: 2e63 616d 6572 6173 2e73 796e 6368 726f  .cameras.synchro
-00002dd0: 6e69 7a65 7272 2000 0000 7221 0000 00da  nizerr ...r!....
-00002de0: 1f70 7978 7933 642e 7265 636f 7264 696e  .pyxy3d.recordin
-00002df0: 672e 7669 6465 6f5f 7265 636f 7264 6572  g.video_recorder
-00002e00: 7222 0000 00da 1370 7978 7933 642e 636f  r".....pyxy3d.co
-00002e10: 6e66 6967 7572 6174 6f72 7223 0000 0072  nfiguratorr#...r
-00002e20: 2400 0000 722d 0000 0072 3200 0000 7234  $...r-...r2...r4
-00002e30: 0000 0072 cf00 0000 727a 0000 0072 c600  ...r....rz...r..
-00002e40: 0000 72e8 0000 0072 2b00 0000 722b 0000  ..r....r+...r+..
-00002e50: 0072 2b00 0000 722c 0000 00da 083c 6d6f  .r+...r,.....<mo
-00002e60: 6475 6c65 3e01 0000 0073 3800 0000 0802  dule>....s8.....
-00002e70: 0c01 0802 0801 0c01 1001 0801 0c01 0c01  ................
-00002e80: 0802 1401 1401 4c01 1014 0c01 0c01 0c01  ......L.........
-00002e90: 0c01 1002 1006 007f 0e02 007f 101b 081e  ................
-00002ea0: 0804 0809 0c0c                           ......
+00000ed0: 6a0c a101 0100 7c00 6a06 6a0d 6a0e a002  j.....|.j.j.j...
+00000ee0: 7c00 6a0f a101 0100 6400 5300 a901 4e29  |.j.....d.S...N)
+00000ef0: 1072 3500 0000 da0e 496d 6167 6542 726f  .r5.....ImageBro
+00000f00: 6164 6361 7374 da07 636f 6e6e 6563 74da  adcast..connect.
+00000f10: 0f49 6d61 6765 5570 6461 7465 536c 6f74  .ImageUpdateSlot
+00000f20: 7237 0000 005a 0c76 616c 7565 4368 616e  r7...Z.valueChan
+00000f30: 6765 6472 2e00 0000 5a13 7365 745f 6163  gedr....Z.set_ac
+00000f40: 7469 7665 5f6d 6f64 655f 6670 73da 0b64  tive_mode_fps..d
+00000f50: 726f 7070 6564 5f66 7073 da12 7570 6461  ropped_fps..upda
+00000f60: 7465 5f64 726f 7070 6564 5f66 7073 723a  te_dropped_fpsr:
+00000f70: 0000 005a 0763 6c69 636b 6564 da11 746f  ...Z.clicked..to
+00000f80: 6767 6c65 5f73 7461 7274 5f73 746f 705a  ggle_start_stopZ
+00000f90: 0b71 745f 7369 676e 616c 6572 5a19 7265  .qt_signalerZ.re
+00000fa0: 636f 7264 696e 675f 636f 6d70 6c65 7465  cording_complete
+00000fb0: 5f73 6967 6e61 6cda 156f 6e5f 7265 636f  _signal..on_reco
+00000fc0: 7264 696e 675f 636f 6d70 6c65 7465 7247  rding_completerG
+00000fd0: 0000 0072 2b00 0000 722b 0000 0072 2c00  ...r+...r+...r,.
+00000fe0: 0000 7241 0000 007f 0000 0073 0a00 0000  ..rA.......s....
+00000ff0: 1002 1201 1001 1001 1601 7a1f 5265 636f  ..........z.Reco
+00001000: 7264 696e 6757 6964 6765 742e 636f 6e6e  rdingWidget.conn
+00001010: 6563 745f 7769 6467 6574 7363 0100 0000  ect_widgetsc....
+00001020: 0000 0000 0000 0000 0300 0000 0400 0000  ................
+00001030: 4300 0000 73fe 0000 0074 00a0 0164 01a1  C...s....t...d..
+00001040: 0101 007c 006a 0274 036a 046b 0272 3474  ...|.j.t.j.k.r4t
+00001050: 036a 057c 005f 027c 006a 06a0 077c 006a  .j.|._.|.j...|.j
+00001060: 026a 08a1 0101 007c 006a 09a0 0a64 02a1  .j.....|.j...d..
+00001070: 0101 0074 00a0 0164 03a1 0101 0074 0b7c  ...t...d.....t.|
+00001080: 006a 0c6a 0d7c 006a 09a0 0ea1 0083 027d  .j.j.|.j.......}
+00001090: 017c 006a 0ca0 0f7c 01a1 0101 0064 0053  .|.j...|.....d.S
+000010a0: 007c 006a 0274 036a 056b 0272 707c 006a  .|.j.t.j.k.rp|.j
+000010b0: 06a0 0a64 02a1 0101 0074 036a 107c 005f  ...d.....t.j.|._
+000010c0: 027c 006a 06a0 077c 006a 026a 08a1 0101  .|.j...|.j.j....
+000010d0: 0074 00a0 0164 04a1 0101 007c 006a 0ca0  .t...d.....|.j..
+000010e0: 11a1 0001 007c 00a0 12a1 007d 027c 006a  .....|.....}.|.j
+000010f0: 09a0 0a64 05a1 0101 007c 006a 09a0 077c  ...d.....|.j...|
+00001100: 02a1 0101 0074 00a0 0164 067c 029b 009d  .....t...d.|....
+00001110: 02a1 0101 0064 0053 007c 006a 0274 036a  .....d.S.|.j.t.j
+00001120: 106b 0272 7d74 00a0 0164 07a1 0101 0064  .k.r}t...d.....d
+00001130: 0053 0064 0053 0029 084e 7a1f 5374 6172  .S.d.S.).Nz.Star
+00001140: 742f 5374 6f70 2052 6563 6f72 6469 6e67  t/Stop Recording
+00001150: 2054 6f67 676c 6564 2e2e 2e46 7a12 496e   Toggled...Fz.In
+00001160: 6974 6961 7465 2072 6563 6f72 6469 6e67  itiate recording
+00001170: 7a2e 5374 6f70 2072 6563 6f72 6469 6e67  z.Stop recording
+00001180: 2061 6e64 2069 6e69 7469 6174 6520 6669   and initiate fi
+00001190: 6e61 6c20 7361 7665 206f 6620 6669 6c65  nal save of file
+000011a0: 547a 3b73 7563 6365 7373 6675 6c6c 7920  Tz;successfully 
+000011b0: 7265 7365 7420 7465 7874 2061 6e64 2072  reset text and r
+000011c0: 656e 616d 6564 2072 6563 6f72 6469 6e67  enamed recording
+000011d0: 2064 6972 6563 746f 7279 2074 6f20 7a2c   directory to z,
+000011e0: 7265 636f 7264 696e 6720 6275 7474 6f6e  recording button
+000011f0: 2074 6f67 676c 6564 2077 6869 6c65 2061   toggled while a
+00001200: 7761 6974 696e 6720 7361 7665 2913 da06  waiting save)...
+00001210: 6c6f 6767 6572 da04 696e 666f 7238 0000  logger..infor8..
+00001220: 0072 2400 0000 7228 0000 0072 2900 0000  .r$...r(...r)...
+00001230: 723a 0000 00da 0773 6574 5465 7874 7239  r:.....setTextr9
+00001240: 0000 0072 3d00 0000 7246 0000 0072 0200  ...r=...rF...r..
+00001250: 0000 722e 0000 0072 5700 0000 da04 7465  ..r....rW.....te
+00001260: 7874 5a0f 7374 6172 745f 7265 636f 7264  xtZ.start_record
+00001270: 696e 6772 2a00 0000 5a0e 7374 6f70 5f72  ingr*...Z.stop_r
+00001280: 6563 6f72 6469 6e67 723c 0000 0029 0372  ecordingr<...).r
+00001290: 4300 0000 5a0e 7265 636f 7264 696e 675f  C...Z.recording_
+000012a0: 7061 7468 5a0e 6e65 7874 5f72 6563 6f72  pathZ.next_recor
+000012b0: 6469 6e67 722b 0000 0072 2b00 0000 722c  dingr+...r+...r,
+000012c0: 0000 0072 6200 0000 8700 0000 732a 0000  ...rb.......s*..
+000012d0: 000a 010c 0108 0110 010c 010a 0214 0110  ................
+000012e0: 010c 020c 0108 0210 020a 010a 0108 020c  ................
+000012f0: 010c 0114 010c 020e 0104 ff7a 2152 6563  ...........z!Rec
+00001300: 6f72 6469 6e67 5769 6467 6574 2e74 6f67  ordingWidget.tog
+00001310: 676c 655f 7374 6172 745f 7374 6f70 6301  gle_start_stopc.
+00001320: 0000 0000 0000 0000 0000 0001 0000 0003  ................
+00001330: 0000 0043 0000 0073 4600 0000 7400 a001  ...C...sF...t...
+00001340: 6401 a101 0100 7402 6a03 7c00 5f04 7c00  d.....t.j.|._.|.
+00001350: 6a05 a006 7c00 6a04 6a07 a101 0100 7400  j...|.j.j.....t.
+00001360: a001 6402 a101 0100 7c00 6a05 a008 6403  ..d.....|.j...d.
+00001370: a101 0100 7400 a001 6404 a101 0100 6400  ....t...d.....d.
+00001380: 5300 2905 4e7a 4452 6563 6f72 6469 6e67  S.).NzDRecording
+00001390: 2063 6f6d 706c 6574 6520 7369 676e 616c   complete signal
+000013a0: 2072 6563 6569 7665 642e 2e2e 7570 6461   received...upda
+000013b0: 7469 6e67 206e 6578 7420 6163 7469 6f6e  ting next action
+000013c0: 2061 6e64 2062 7574 746f 6e7a 2445 6e61   and buttonz$Ena
+000013d0: 626c 696e 6720 7374 6172 742f 7374 6f70  bling start/stop
+000013e0: 2072 6563 6f72 6469 6e67 2062 7574 746f   recording butto
+000013f0: 6e54 7a30 5375 6363 6573 7366 756c 6c79  nTz0Successfully
+00001400: 2065 6e61 626c 6564 2073 7461 7274 2f73   enabled start/s
+00001410: 746f 7020 7265 636f 7264 696e 6720 6275  top recording bu
+00001420: 7474 6f6e 2909 7264 0000 0072 6500 0000  tton).rd...re...
+00001430: 7224 0000 0072 2800 0000 7238 0000 0072  r$...r(...r8...r
+00001440: 3a00 0000 7266 0000 0072 3900 0000 7246  :...rf...r9...rF
+00001450: 0000 0072 4700 0000 722b 0000 0072 2b00  ...rG...r+...r+.
+00001460: 0000 722c 0000 0072 6300 0000 a300 0000  ..r,...rc.......
+00001470: 730c 0000 000a 0108 0110 010a 010c 010e  s...............
+00001480: 017a 2552 6563 6f72 6469 6e67 5769 6467  .z%RecordingWidg
+00001490: 6574 2e6f 6e5f 7265 636f 7264 696e 675f  et.on_recording_
+000014a0: 636f 6d70 6c65 7465 7260 0000 0063 0200  completer`...c..
+000014b0: 0000 0000 0000 0000 0000 0500 0000 0600  ................
+000014c0: 0000 4300 0000 733c 0000 0064 017d 027c  ..C...s<...d.}.|
+000014d0: 01a0 00a1 0044 005d 0f5c 027d 037d 047c  .....D.].\.}.}.|
+000014e0: 027c 039b 0064 027c 0464 039b 0464 049d  .|...d.|.d...d..
+000014f0: 0437 007d 0271 067c 006a 01a0 027c 02a1  .7.}.q.|.j...|..
+00001500: 0101 0064 0553 0029 067a 3855 6e72 6176  ...d.S.).z8Unrav
+00001510: 656c 2064 726f 7070 6564 2066 7073 2064  el dropped fps d
+00001520: 6963 7469 6f6e 6172 7920 746f 2061 206d  ictionary to a m
+00001530: 6f72 6520 7265 6164 6162 6c65 2073 7472  ore readable str
+00001540: 696e 677a 2352 6174 6520 6f66 2046 7261  ingz#Rate of Fra
+00001550: 6d65 2044 726f 7070 696e 6720 6279 2050  me Dropping by P
+00001560: 6f72 743a 2020 2020 7a02 3a20 7a03 2e30  ort:    z.: z..0
+00001570: 257a 0820 2020 2020 2020 204e 2903 da05  %z.        N)...
+00001580: 6974 656d 7372 3e00 0000 7266 0000 0029  itemsr>...rf...)
+00001590: 0572 4300 0000 7260 0000 0072 6700 0000  .rC...r`...rg...
+000015a0: da04 706f 7274 5a09 6472 6f70 5f72 6174  ..portZ.drop_rat
+000015b0: 6572 2b00 0000 722b 0000 0072 2c00 0000  er+...r+...r,...
+000015c0: 7261 0000 00ad 0000 0073 0800 0000 0402  ra.......s......
+000015d0: 1001 1801 1002 7a22 5265 636f 7264 696e  ......z"Recordin
+000015e0: 6757 6964 6765 742e 7570 6461 7465 5f64  gWidget.update_d
+000015f0: 726f 7070 6564 5f66 7073 6302 0000 0000  ropped_fpsc.....
+00001600: 0000 0000 0000 0003 0000 0004 0000 0043  ...............C
+00001610: 0000 0073 2c00 0000 7c00 6a00 a001 7c00  ...s,...|.j...|.
+00001620: 6a00 a002 a100 a101 0100 7403 a004 7c01  j.........t...|.
+00001630: a101 7d02 7c00 6a00 a005 7c02 a101 0100  ..}.|.j...|.....
+00001640: 6400 5300 725c 0000 0029 0672 3f00 0000  d.S.r\...).r?...
+00001650: da06 7265 7369 7a65 5a08 7369 7a65 4869  ..resizeZ.sizeHi
+00001660: 6e74 720b 0000 005a 0966 726f 6d49 6d61  ntr....Z.fromIma
+00001670: 6765 5a09 7365 7450 6978 6d61 7029 0372  geZ.setPixmap).r
+00001680: 4300 0000 5a07 715f 696d 6167 655a 0771  C...Z.q_imageZ.q
+00001690: 7069 786d 6170 722b 0000 0072 2b00 0000  pixmapr+...r+...
+000016a0: 722c 0000 0072 5f00 0000 b600 0000 7306  r,...r_.......s.
+000016b0: 0000 0012 010a 0110 017a 1f52 6563 6f72  .........z.Recor
+000016c0: 6469 6e67 5769 6467 6574 2e49 6d61 6765  dingWidget.Image
+000016d0: 5570 6461 7465 536c 6f74 290f 7225 0000  UpdateSlot).r%..
+000016e0: 0072 2600 0000 7227 0000 0072 1e00 0000  .r&...r'...r....
+000016f0: 7230 0000 0072 4200 0000 723c 0000 0072  r0...rB...r<...r
+00001700: 4000 0000 7241 0000 0072 6200 0000 7263  @...rA...rb...rc
+00001710: 0000 00da 0464 6963 7472 6100 0000 725f  .....dictra...r_
+00001720: 0000 00da 0d5f 5f63 6c61 7373 6365 6c6c  .....__classcell
+00001730: 5f5f 722b 0000 0072 2b00 0000 7244 0000  __r+...r+...rD..
+00001740: 0072 2c00 0000 722d 0000 0031 0000 0073  .r,...r-...1...s
+00001750: 1400 0000 0800 1202 0820 0807 0811 0814  ......... ......
+00001760: 0808 081c 0e0a 1009 722d 0000 0063 0000  ........r-...c..
+00001770: 0000 0000 0000 0000 0000 0000 0000 0400  ................
+00001780: 0000 4000 0000 7344 0000 0065 005a 0164  ..@...sD...e.Z.d
+00001790: 005a 0264 1064 0265 0366 0264 0364 0484  .Z.d.d.e.f.d.d..
+000017a0: 055a 0464 0564 0684 005a 0564 0764 0884  .Z.d.d...Z.d.d..
+000017b0: 005a 0664 0964 0a84 005a 0764 0b64 0c84  .Z.d.d...Z.d.d..
+000017c0: 005a 0864 0d64 0e84 005a 0964 0f53 0029  .Z.d.d...Z.d.S.)
+000017d0: 1172 3200 0000 e9fa 0000 0072 3100 0000  .r2........r1...
+000017e0: 6303 0000 0000 0000 0000 0000 0006 0000  c...............
+000017f0: 0005 0000 0043 0000 0073 8c00 0000 7c01  .....C...s....|.
+00001800: 7c00 5f00 7c02 7c00 5f01 6700 7c00 5f02  |._.|.|._.g.|._.
+00001810: 7c00 6a00 6a03 a004 a100 4400 5d0a 5c02  |.j.j.....D.].\.
+00001820: 7d03 7d04 7c00 6a02 a005 7c03 a101 0100  }.}.|.j...|.....
+00001830: 710f 7c00 6a02 a006 a100 0100 7407 7c00  q.|.j.......t.|.
+00001840: 6a02 8301 7d05 7408 7409 a00a 7c05 6401  j...}.t.t...|.d.
+00001850: 1300 a101 8301 7c00 5f0b 7408 7409 a00a  ......|._.t.t...
+00001860: 7c05 7c00 6a0b 1b00 a101 8301 7c00 5f0c  |.|.j.......|._.
+00001870: 740d 8300 7c00 5f0e 7c00 6a00 a00f 7c00  t...|._.|.j...|.
+00001880: 6a0e a101 0100 6400 5300 2902 4e67 0000  j.....d.S.).Ng..
+00001890: 0000 0000 e03f 2910 7231 0000 00da 1373  .....?).r1.....s
+000018a0: 696e 676c 655f 6672 616d 655f 6865 6967  ingle_frame_heig
+000018b0: 6874 da05 706f 7274 73da 0773 7472 6561  ht..ports..strea
+000018c0: 6d73 7268 0000 00da 0661 7070 656e 64da  msrh.....append.
+000018d0: 0473 6f72 7472 5900 0000 7255 0000 00da  .sortrY...rU....
+000018e0: 046d 6174 68da 0463 6569 6cda 0d66 7261  .math..ceil..fra
+000018f0: 6d65 5f63 6f6c 756d 6e73 da0a 6672 616d  me_columns..fram
+00001900: 655f 726f 7773 7205 0000 00da 166e 6577  e_rowsr......new
+00001910: 5f73 796e 635f 7061 636b 6574 5f6e 6f74  _sync_packet_not
+00001920: 6963 655a 1373 7562 7363 7269 6265 5f74  iceZ.subscribe_t
+00001930: 6f5f 6e6f 7469 6365 2906 7243 0000 0072  o_notice).rC...r
+00001940: 3100 0000 726e 0000 0072 6900 0000 da06  1...rn...ri.....
+00001950: 7374 7265 616d 5a0c 6361 6d65 7261 5f63  streamZ.camera_c
+00001960: 6f75 6e74 722b 0000 0072 2b00 0000 722c  ountr+...r+...r,
+00001970: 0000 0072 3000 0000 bc00 0000 7316 0000  ...r0.......s...
+00001980: 0006 0106 0106 0314 010e 030a 010a 0414  ................
+00001990: 0116 0108 0212 017a 1d55 6e70 6169 7265  .......z.Unpaire
+000019a0: 6446 7261 6d65 4275 696c 6465 722e 5f5f  dFrameBuilder.__
+000019b0: 696e 6974 5f5f 6301 0000 0000 0000 0000  init__c.........
+000019c0: 0000 0001 0000 0003 0000 0043 0000 0073  ...........C...s
+000019d0: 1c00 0000 7400 a001 6401 a101 0100 7c00  ....t...d.....|.
+000019e0: 6a02 a003 7c00 6a04 a101 0100 6400 5300  j...|.j.....d.S.
+000019f0: 2902 4e7a 2c55 6e73 7562 7363 7269 6265  ).Nz,Unsubscribe
+00001a00: 2066 7261 6d65 2062 7569 6c64 6572 2066   frame builder f
+00001a10: 726f 6d20 7379 6e63 6872 6f6e 697a 6572  rom synchronizer
+00001a20: 2e29 0572 6400 0000 7265 0000 0072 3100  .).rd...re...r1.
+00001a30: 0000 5a15 756e 7375 6273 6372 6962 655f  ..Z.unsubscribe_
+00001a40: 746f 5f6e 6f74 6963 6572 7700 0000 7247  to_noticerw...rG
+00001a50: 0000 0072 2b00 0000 722b 0000 0072 2c00  ...r+...r+...r,.
+00001a60: 0000 da1d 756e 7375 6273 6372 6962 655f  ....unsubscribe_
+00001a70: 6672 6f6d 5f73 796e 6368 726f 6e69 7a65  from_synchronize
+00001a80: 72d1 0000 0073 0400 0000 0a01 1201 7a32  r....s........z2
+00001a90: 556e 7061 6972 6564 4672 616d 6542 7569  UnpairedFrameBui
+00001aa0: 6c64 6572 2e75 6e73 7562 7363 7269 6265  lder.unsubscribe
+00001ab0: 5f66 726f 6d5f 7379 6e63 6872 6f6e 697a  _from_synchroniz
+00001ac0: 6572 6302 0000 0000 0000 0000 0000 0004  erc.............
+00001ad0: 0000 0004 0000 0043 0000 0073 3c00 0000  .......C...s<...
+00001ae0: 7c00 6a00 7d02 7c01 6401 7500 7219 7401  |.j.}.|.d.u.r.t.
+00001af0: a002 6402 a101 0100 7403 6a04 7c02 7c02  ..d.....t.j.|.|.
+00001b00: 6403 6603 7403 6a05 6404 8d02 7d03 7c03  d.f.t.j.d...}.|.
+00001b10: 5300 7c01 6a06 7d03 7c03 5300 2905 7a7b  S.|.j.}.|.S.).z{
+00001b20: 5379 6e63 6872 6f6e 697a 6174 696f 6e20  Synchronization 
+00001b30: 6973 7375 6573 2063 616e 206c 6561 6420  issues can lead 
+00001b40: 746f 2073 6f6d 6520 6672 616d 6573 2062  to some frames b
+00001b50: 6569 6e67 204e 6f6e 6520 616d 6f6e 670a  eing None among.
+00001b60: 2020 2020 2020 2020 7468 6520 7379 6e63          the sync
+00001b70: 6865 6420 6672 616d 6573 2c20 736f 2070  hed frames, so p
+00001b80: 6c75 6720 7468 6174 2077 6974 6820 6120  lug that with a 
+00001b90: 626c 616e 6b20 6672 616d 654e 7a19 706c  blank frameNz.pl
+00001ba0: 7567 6769 6e67 2062 6c61 6e6b 2066 7261  ugging blank fra
+00001bb0: 6d65 2064 6174 61e9 0300 0000 2901 5a05  me data.....).Z.
+00001bc0: 6474 7970 6529 0772 6e00 0000 7264 0000  dtype).rn...rd..
+00001bd0: 00da 0564 6562 7567 da02 6e70 5a05 7a65  ...debug..npZ.ze
+00001be0: 726f 735a 0575 696e 7438 da05 6672 616d  rosZ.uint8..fram
+00001bf0: 6529 0472 4300 0000 da0c 6672 616d 655f  e).rC.....frame_
+00001c00: 7061 636b 6574 5a04 6564 6765 727d 0000  packetZ.edger}..
+00001c10: 0072 2b00 0000 722b 0000 0072 2c00 0000  .r+...r+...r,...
+00001c20: da12 6765 745f 6672 616d 655f 6f72 5f62  ..get_frame_or_b
+00001c30: 6c61 6e6b d600 0000 730e 0000 0006 0408  lank....s.......
+00001c40: 020a 0116 0104 0406 fe04 027a 2755 6e70  ...........z'Unp
+00001c50: 6169 7265 6446 7261 6d65 4275 696c 6465  airedFrameBuilde
+00001c60: 722e 6765 745f 6672 616d 655f 6f72 5f62  r.get_frame_or_b
+00001c70: 6c61 6e6b 6302 0000 0000 0000 0000 0000  lankc...........
+00001c80: 0008 0000 0009 0000 0043 0000 0073 8600  .........C...s..
+00001c90: 0000 7400 a001 6401 a101 0100 7c01 6a02  ..t...d.....|.j.
+00001ca0: 6402 1900 7d02 7c01 6a02 6403 1900 7d03  d...}.|.j.d...}.
+00001cb0: 7403 7c02 7c03 8302 7d04 7404 7c04 7c02  t.|.|...}.t.|.|.
+00001cc0: 1800 6404 1b00 8301 7d05 7404 7c04 7c03  ..d.....}.t.|.|.
+00001cd0: 1800 6404 1b00 8301 7d06 6700 6405 a201  ..d.....}.g.d...
+00001ce0: 7d07 7400 a001 6406 a101 0100 7405 6a06  }.t...d.....t.j.
+00001cf0: 7c01 7c05 7c05 7c06 7c06 7405 6a07 7c07  |.|.|.|.|.t.j.|.
+00001d00: 6407 8d07 7d01 7408 7c01 7c00 6a09 6408  d...}.t.|.|.j.d.
+00001d10: 8d02 7d01 7c01 5300 2909 7a65 546f 206d  ..}.|.S.).zeTo m
+00001d20: 616b 6520 7375 7265 2074 6861 7420 6672  ake sure that fr
+00001d30: 616d 6573 2061 6c69 676e 2077 656c 6c2c  ames align well,
+00001d40: 2073 6361 6c65 2074 6865 6d20 616c 6c20   scale them all 
+00001d50: 746f 2074 6875 6d62 6e61 696c 730a 2020  to thumbnails.  
+00001d60: 2020 2020 2020 7371 7561 7265 7320 7769        squares wi
+00001d70: 7468 2062 6c61 636b 2062 6f72 6465 7273  th black borders
+00001d80: 2e7a 0f72 6573 697a 696e 6720 7371 7561  .z.resizing squa
+00001d90: 7265 7201 0000 0072 5200 0000 e902 0000  rer....rR.......
+00001da0: 0029 0372 0100 0000 7201 0000 0072 0100  .).r....r....r..
+00001db0: 0000 7a13 6162 6f75 7420 746f 2070 6164  ..z.about to pad
+00001dc0: 2062 6f72 6465 7229 0172 3900 0000 2901   border).r9...).
+00001dd0: da0a 6e65 775f 6865 6967 6874 290a 7264  ..new_height).rd
+00001de0: 0000 0072 7b00 0000 da05 7368 6170 6572  ...r{.....shaper
+00001df0: 5b00 0000 7255 0000 00da 0363 7632 5a0e  [...rU.....cv2Z.
+00001e00: 636f 7079 4d61 6b65 426f 7264 6572 5a0f  copyMakeBorderZ.
+00001e10: 424f 5244 4552 5f43 4f4e 5354 414e 5472  BORDER_CONSTANTr
+00001e20: 6a00 0000 726e 0000 0029 0872 4300 0000  j...rn...).rC...
+00001e30: 727d 0000 005a 0668 6569 6768 74da 0577  r}...Z.height..w
+00001e40: 6964 7468 5a0b 7061 6464 6564 5f73 697a  idthZ.padded_siz
+00001e50: 655a 0a68 6569 6768 745f 7061 645a 0977  eZ.height_padZ.w
+00001e60: 6964 7468 5f70 6164 5a09 7061 645f 636f  idth_padZ.pad_co
+00001e70: 6c6f 7272 2b00 0000 722b 0000 0072 2c00  lorr+...r+...r,.
+00001e80: 0000 da10 7265 7369 7a65 5f74 6f5f 7371  ....resize_to_sq
+00001e90: 7561 7265 e500 0000 7326 0000 000a 030a  uare....s&......
+00001ea0: 040a 010a 0210 0210 0108 010a 0204 0102  ................
+00001eb0: 0102 0102 0102 0102 0104 0102 0106 f90e  ................
+00001ec0: 0a04 017a 2555 6e70 6169 7265 6446 7261  ...z%UnpairedFra
+00001ed0: 6d65 4275 696c 6465 722e 7265 7369 7a65  meBuilder.resize
+00001ee0: 5f74 6f5f 7371 7561 7265 6303 0000 0000  _to_squarec.....
+00001ef0: 0000 0000 0000 0004 0000 0004 0000 0043  ...............C
+00001f00: 0000 0073 6c00 0000 7c00 6a00 6a01 7c02  ...sl...|.j.j.|.
+00001f10: 1900 6a02 6a03 7d03 7c03 6401 6b02 720f  ..j.j.}.|.d.k.r.
+00001f20: 0900 7c01 5300 7c03 6402 7600 721c 7404  ..|.S.|.d.v.r.t.
+00001f30: a005 7c01 7404 6a06 a102 7d01 7c01 5300  ..|.t.j...}.|.S.
+00001f40: 7c03 6403 7600 7229 7404 a005 7c01 7404  |.d.v.r)t...|.t.
+00001f50: 6a07 a102 7d01 7c01 5300 7c03 6404 7600  j...}.|.S.|.d.v.
+00001f60: 7234 7404 a005 7c01 7404 6a08 a102 7d01  r4t...|.t.j...}.
+00001f70: 7c01 5300 2905 4e72 0100 0000 2902 7252  |.S.).Nr....).rR
+00001f80: 0000 00e9 fdff ffff 2902 7280 0000 00e9  ........).r.....
+00001f90: feff ffff 2902 e9ff ffff ff72 7a00 0000  ....)......rz...
+00001fa0: 2909 7231 0000 0072 7000 0000 5a06 6361  ).r1...rp...Z.ca
+00001fb0: 6d65 7261 da0e 726f 7461 7469 6f6e 5f63  mera..rotation_c
+00001fc0: 6f75 6e74 7283 0000 00da 0672 6f74 6174  ountr......rotat
+00001fd0: 655a 1352 4f54 4154 455f 3930 5f43 4c4f  eZ.ROTATE_90_CLO
+00001fe0: 434b 5749 5345 5a0a 524f 5441 5445 5f31  CKWISEZ.ROTATE_1
+00001ff0: 3830 5a1a 524f 5441 5445 5f39 305f 434f  80Z.ROTATE_90_CO
+00002000: 554e 5445 5243 4c4f 434b 5749 5345 2904  UNTERCLOCKWISE).
+00002010: 7243 0000 0072 7d00 0000 7269 0000 0072  rC...r}...ri...r
+00002020: 8900 0000 722b 0000 0072 2b00 0000 722c  ....r+...r+...r,
+00002030: 0000 00da 0e61 7070 6c79 5f72 6f74 6174  .....apply_rotat
+00002040: 696f 6e04 0100 0073 1a00 0000 1002 0801  ion....s........
+00002050: 0201 0408 08f9 0e01 0406 08fb 0e01 0404  ................
+00002060: 08fd 0e01 0402 7a23 556e 7061 6972 6564  ......z#Unpaired
+00002070: 4672 616d 6542 7569 6c64 6572 2e61 7070  FrameBuilder.app
+00002080: 6c79 5f72 6f74 6174 696f 6e63 0100 0000  ly_rotationc....
+00002090: 0000 0000 0000 0000 1100 0000 0a00 0000  ................
+000020a0: 4300 0000 7378 0100 007c 006a 00a0 01a1  C...sx...|.j....
+000020b0: 0001 007c 006a 026a 037c 005f 0369 007d  ...|.j.j.|._.i.}
+000020c0: 017c 006a 0444 005d 3f7d 027c 006a 036a  .|.j.D.]?}.|.j.j
+000020d0: 057c 0219 007d 037c 00a0 067c 03a1 017d  .|...}.|...|...}
+000020e0: 047c 00a0 077c 04a1 017d 057c 00a0 087c  .|...|...}.|...|
+000020f0: 057c 02a1 027d 0674 09a0 0a7c 0664 01a1  .|...}.t...|.d..
+00002100: 027d 0774 096a 0b7c 0774 0c7c 0283 0174  .}.t.j.|.t.|...t
+00002110: 0d7c 076a 0e64 0119 0064 021b 0083 0174  .|.j.d...d.....t
+00002120: 0d7c 006a 0f64 031b 0083 0166 0274 096a  .|.j.d.....f.t.j
+00002130: 1064 0164 0464 0264 058d 077d 087c 087c  .d.d.d.d...}.|.|
+00002140: 017c 023c 0071 0f67 007d 0964 067d 0a64  .|.<.q.g.}.d.}.d
+00002150: 077d 0b64 077d 0c74 117c 006a 0483 017d  .}.d.}.t.|.j...}
+00002160: 0d7c 01a0 12a1 0044 005d 445c 027d 027d  .|.....D.]D\.}.}
+00002170: 0e7c 0a64 0675 0072 6b7c 0e7d 0a6e 0774  .|.d.u.rk|.}.n.t
+00002180: 13a0 147c 0a7c 0e67 02a1 017d 0a7c 0b64  ...|.|.g...}.|.d
+00002190: 0137 007d 0b7c 0d64 0138 007d 0d7c 0d64  .7.}.|.d.8.}.|.d
+000021a0: 076b 0272 967c 0b7c 006a 156b 0072 9674  .k.r.|.|.j.k.r.t
+000021b0: 13a0 147c 0a7c 00a0 0664 06a1 0167 02a1  ...|.|...d...g..
+000021c0: 017d 0a7c 0b64 0137 007d 0b7c 0b7c 006a  .}.|.d.7.}.|.|.j
+000021d0: 156b 0073 837c 0b7c 006a 156b 0272 a47c  .k.s.|.|.j.k.r.|
+000021e0: 09a0 167c 0aa1 0101 0064 067d 0a64 077d  ...|.....d.}.d.}
+000021f0: 0b71 6064 067d 0f7c 0944 005d 107d 107c  .q`d.}.|.D.].}.|
+00002200: 0f64 0675 0072 b27c 107d 0f71 a974 13a0  .d.u.r.|.}.q.t..
+00002210: 177c 0f7c 1067 02a1 017d 0f71 a97c 0f53  .|.|.g...}.q.|.S
+00002220: 0029 087a fb0a 2020 2020 2020 2020 5468  .).z..        Th
+00002230: 6973 2067 6c75 6573 2074 6f67 6574 6865  is glues togethe
+00002240: 7220 7468 6520 696e 6469 7669 6475 616c  r the individual
+00002250: 2066 7261 6d65 7320 696e 2074 6865 2073   frames in the s
+00002260: 796e 6320 7061 636b 6574 2069 6e74 6f20  ync packet into 
+00002270: 6f6e 6520 6c61 7267 6520 626c 6f63 6b0a  one large block.
+00002280: 0a20 2020 2020 2020 2043 7572 7265 6e74  .        Current
+00002290: 6c79 206a 7573 7420 7374 6163 6b69 6e67  ly just stacking
+000022a0: 2061 6c6c 2066 7261 6d65 7320 7665 7274   all frames vert
+000022b0: 6963 616c 6c79 2c20 6275 7420 7468 6973  ically, but this
+000022c0: 2073 686f 756c 6420 6265 2065 7870 616e   should be expan
+000022d0: 6465 6420 6f6e 2074 6865 200a 2020 2020  ded on the .    
+000022e0: 2020 2020 7468 6520 6675 7475 7265 2074      the future t
+000022f0: 6f20 616c 6c6f 7720 7772 6170 7069 6e67  o allow wrapping
+00002300: 2074 6f20 6120 6d6f 7265 2073 7175 6172   to a more squar
+00002310: 6520 7368 6170 650a 2020 2020 2020 2020  e shape.        
+00002320: 7252 0000 0072 8000 0000 e904 0000 0029  rR...r.........)
+00002330: 0372 0100 0000 7201 0000 00e9 ff00 0000  .r....r.........
+00002340: 2904 5a08 666f 6e74 4661 6365 5a09 666f  ).Z.fontFaceZ.fo
+00002350: 6e74 5363 616c 655a 0563 6f6c 6f72 5a09  ntScaleZ.colorZ.
+00002360: 7468 6963 6b6e 6573 734e 7201 0000 0029  thicknessNr....)
+00002370: 1872 7700 0000 da03 6765 7472 3100 0000  .rw.....getr1...
+00002380: 5a13 6375 7272 656e 745f 7379 6e63 5f70  Z.current_sync_p
+00002390: 6163 6b65 7472 6f00 0000 5a0d 6672 616d  acketro...Z.fram
+000023a0: 655f 7061 636b 6574 7372 7f00 0000 7285  e_packetsr....r.
+000023b0: 0000 0072 8b00 0000 7283 0000 005a 0466  ...r....r....Z.f
+000023c0: 6c69 705a 0770 7574 5465 7874 725a 0000  lipZ.putTextrZ..
+000023d0: 0072 5500 0000 7282 0000 0072 6e00 0000  .rU...r....rn...
+000023e0: 5a14 464f 4e54 5f48 4552 5348 4559 5f53  Z.FONT_HERSHEY_S
+000023f0: 494d 504c 4558 7259 0000 0072 6800 0000  IMPLEXrY...rh...
+00002400: 727c 0000 005a 0668 7374 6163 6b72 7500  r|...Z.hstackru.
+00002410: 0000 7271 0000 005a 0676 7374 6163 6b29  ..rq...Z.vstack)
+00002420: 1172 4300 0000 5a10 7468 756d 626e 6169  .rC...Z.thumbnai
+00002430: 6c5f 6672 616d 6573 7269 0000 0072 7e00  l_framesri...r~.
+00002440: 0000 5a09 7261 775f 6672 616d 655a 0c73  ..Z.raw_frameZ.s
+00002450: 7175 6172 655f 6672 616d 655a 0d72 6f74  quare_frameZ.rot
+00002460: 6174 6564 5f66 7261 6d65 5a0d 666c 6970  ated_frameZ.flip
+00002470: 7065 645f 6672 616d 655a 0a74 6578 745f  ped_frameZ.text_
+00002480: 6672 616d 6572 7600 0000 5a0b 6375 7272  framerv...Z.curr
+00002490: 656e 745f 726f 775a 1263 7572 7265 6e74  ent_rowZ.current
+000024a0: 5f72 6f77 5f6c 656e 6774 685a 0c66 7261  _row_lengthZ.fra
+000024b0: 6d65 735f 6164 6465 645a 1066 7261 6d65  mes_addedZ.frame
+000024c0: 735f 7265 6d61 696e 696e 6772 7d00 0000  s_remainingr}...
+000024d0: 5a0a 6d65 6761 5f66 7261 6d65 da03 726f  Z.mega_frame..ro
+000024e0: 7772 2b00 0000 722b 0000 0072 2c00 0000  wr+...r+...r,...
+000024f0: da13 6765 745f 7265 636f 7264 696e 675f  ..get_recording_
+00002500: 6672 616d 6513 0100 0073 5a00 0000 0a08  frame....sZ.....
+00002510: 0a01 0402 0a01 0c01 0a01 0a01 0c01 0c01  ................
+00002520: 0603 0601 1e01 0401 0201 0201 0201 06fa  ................
+00002530: 0a09 0402 0401 0401 0401 0a01 1001 0802  ................
+00002540: 0601 0e02 0801 0801 0802 0a02 1401 0801  ................
+00002550: 0afe 0a04 0a01 0401 0401 0280 0402 0801  ................
+00002560: 0801 0601 1002 0403 7a28 556e 7061 6972  ........z(Unpair
+00002570: 6564 4672 616d 6542 7569 6c64 6572 2e67  edFrameBuilder.g
+00002580: 6574 5f72 6563 6f72 6469 6e67 5f66 7261  et_recording_fra
+00002590: 6d65 4e29 0172 6d00 0000 290a 7225 0000  meN).rm...).r%..
+000025a0: 0072 2600 0000 7227 0000 0072 2000 0000  .r&...r'...r ...
+000025b0: 7230 0000 0072 7900 0000 727f 0000 0072  r0...ry...r....r
+000025c0: 8500 0000 728b 0000 0072 9000 0000 722b  ....r....r....r+
+000025d0: 0000 0072 2b00 0000 722b 0000 0072 2c00  ...r+...r+...r,.
+000025e0: 0000 7232 0000 00bb 0000 0073 0e00 0000  ..r2.......s....
+000025f0: 0800 1001 0815 0805 080f 081f 0c0f 7232  ..............r2
+00002600: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00002610: 0000 0000 0400 0000 0000 0000 733a 0000  ............s:..
+00002620: 0065 005a 0164 005a 0265 0365 0483 015a  .e.Z.d.Z.e.e...Z
+00002630: 0565 0365 0683 015a 0764 0165 0866 0287  .e.e...Z.d.e.f..
+00002640: 0066 0164 0264 0384 0c5a 0964 0464 0584  .f.d.d...Z.d.d..
+00002650: 005a 0a87 0004 005a 0b53 0029 0672 3400  .Z.....Z.S.).r4.
+00002660: 0000 7233 0000 0063 0200 0000 0000 0000  ..r3...c........
+00002670: 0000 0000 0200 0000 0300 0000 0300 0000  ................
+00002680: 732a 0000 0074 0074 017c 0083 02a0 02a1  s*...t.t.|......
+00002690: 0001 007c 017c 005f 0374 04a0 0564 01a1  ...|.|._.t...d..
+000026a0: 0101 0074 0683 007c 005f 0764 0053 0029  ...t...|._.d.S.)
+000026b0: 024e 7a21 496e 6974 6961 7465 6420 7265  .Nz!Initiated re
+000026c0: 636f 7264 696e 6720 6672 616d 6520 656d  cording frame em
+000026d0: 6974 7465 7229 0872 2f00 0000 7234 0000  itter).r/...r4..
+000026e0: 0072 3000 0000 da17 7265 636f 7264 696e  .r0.....recordin
+000026f0: 675f 6672 616d 655f 6275 696c 6465 7272  g_frame_builderr
+00002700: 6400 0000 7265 0000 0072 0400 0000 da0f  d...re...r......
+00002710: 6b65 6570 5f63 6f6c 6c65 6374 696e 6729  keep_collecting)
+00002720: 0272 4300 0000 7233 0000 0072 4400 0000  .rC...r3...rD...
+00002730: 722b 0000 0072 2c00 0000 7230 0000 0059  r+...r,...r0...Y
+00002740: 0100 0073 0800 0000 0e02 0601 0a01 0c01  ...s............
+00002750: 7a1d 556e 7061 6972 6564 4672 616d 6545  z.UnpairedFrameE
+00002760: 6d69 7474 6572 2e5f 5f69 6e69 745f 5f63  mitter.__init__c
+00002770: 0100 0000 0000 0000 0000 0000 0300 0000  ................
+00002780: 0300 0000 4300 0000 7364 0000 007c 006a  ....C...sd...|.j
+00002790: 00a0 01a1 0001 007c 006a 00a0 02a1 0072  .......|.j.....r
+000027a0: 2b7c 006a 03a0 04a1 007d 017c 0164 0075  +|.j.....}.|.d.u
+000027b0: 0172 2674 057c 0183 017d 027c 006a 06a0  .r&t.|...}.|.j..
+000027c0: 077c 02a1 0101 007c 006a 08a0 077c 006a  .|.....|.j...|.j
+000027d0: 036a 096a 08a1 0101 007c 006a 00a0 02a1  .j.j.....|.j....
+000027e0: 0073 0a74 0aa0 0b64 01a1 0101 0064 0053  .s.t...d.....d.S
+000027f0: 0029 024e 7a27 5374 6572 656f 6672 616d  .).Nz'Stereofram
+00002800: 6520 656d 6974 7465 7220 7275 6e20 7468  e emitter run th
+00002810: 7265 6164 2065 6e64 6564 2e2e 2e29 0c72  read ended...).r
+00002820: 9200 0000 da03 7365 74da 0669 735f 7365  ......set..is_se
+00002830: 7472 9100 0000 7290 0000 00da 0d63 7632  tr....r......cv2
+00002840: 5f74 6f5f 716c 6162 656c 725d 0000 00da  _to_qlabelr]....
+00002850: 0465 6d69 7472 6000 0000 7231 0000 0072  .emitr`...r1...r
+00002860: 6400 0000 7265 0000 0029 0372 4300 0000  d...re...).rC...
+00002870: 5a0f 7265 636f 7264 696e 675f 6672 616d  Z.recording_fram
+00002880: 65da 0569 6d61 6765 722b 0000 0072 2b00  e..imager+...r+.
+00002890: 0000 722c 0000 00da 0372 756e 6001 0000  ..r,.....run`...
+000028a0: 7312 0000 000a 020a 020a 0408 0208 010c  s...............
+000028b0: 0112 010a f70e 0b7a 1855 6e70 6169 7265  .......z.Unpaire
+000028c0: 6446 7261 6d65 456d 6974 7465 722e 7275  dFrameEmitter.ru
+000028d0: 6e29 0c72 2500 0000 7226 0000 0072 2700  n).r%...r&...r'.
+000028e0: 0000 7208 0000 0072 0a00 0000 725d 0000  ..r....r....r]..
+000028f0: 0072 6b00 0000 7260 0000 0072 3200 0000  .rk...r`...r2...
+00002900: 7230 0000 0072 9800 0000 726c 0000 0072  r0...r....rl...r
+00002910: 2b00 0000 722b 0000 0072 4400 0000 722c  +...r+...rD...r,
+00002920: 0000 0072 3400 0000 5501 0000 730a 0000  ...r4...U...s...
+00002930: 0008 0008 0108 0112 0210 0772 3400 0000  ...........r4...
+00002940: 6302 0000 0000 0000 0000 0000 0003 0000  c...............
+00002950: 0003 0000 0003 0000 0073 1a00 0000 8700  .........s......
+00002960: 6601 6401 6402 8408 7c00 a000 a100 4400  f.d.d...|.....D.
+00002970: 8301 7d02 7c02 5300 2903 4e63 0100 0000  ..}.|.S.).Nc....
+00002980: 0000 0000 0000 0000 0300 0000 0400 0000  ................
+00002990: 1300 0000 731c 0000 0067 007c 005d 0a5c  ....s....g.|.].\
+000029a0: 027d 017d 027c 0288 006b 0072 027c 0191  .}.}.|...k.r.|..
+000029b0: 0271 0253 0072 2b00 0000 722b 0000 0029  .q.S.r+...r+...)
+000029c0: 0372 4a00 0000 da03 6b65 7972 3900 0000  .rJ.....keyr9...
+000029d0: a901 da0d 6d69 6e5f 7468 7265 7368 6f6c  ....min_threshol
+000029e0: 6472 2b00 0000 722c 0000 0072 4c00 0000  dr+...r,...rL...
+000029f0: 7401 0000 7256 0000 007a 2367 6574 5f65  t...rV...z#get_e
+00002a00: 6d70 7479 5f70 6169 7273 2e3c 6c6f 6361  mpty_pairs.<loca
+00002a10: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 2901  ls>.<listcomp>).
+00002a20: 7268 0000 0029 035a 0c62 6f61 7264 5f63  rh...).Z.board_c
+00002a30: 6f75 6e74 7372 9b00 0000 5a0b 656d 7074  ountsr....Z.empt
+00002a40: 795f 7061 6972 7372 2b00 0000 729a 0000  y_pairsr+...r...
+00002a50: 0072 2c00 0000 da0f 6765 745f 656d 7074  .r,.....get_empt
+00002a60: 795f 7061 6972 7373 0100 0073 0400 0000  y_pairss...s....
+00002a70: 1601 0401 729c 0000 0063 0200 0000 0000  ....r....c......
+00002a80: 0000 0000 0000 0700 0000 0500 0000 4300  ..............C.
+00002a90: 0000 7344 0000 007c 006a 0064 0064 0185  ..sD...|.j.d.d..
+00002aa0: 0219 005c 027d 027d 037c 0174 017c 0283  ...\.}.}.|.t.|..
+00002ab0: 011b 007d 0474 027c 037c 0414 0083 017c  ...}.t.|.|.....|
+00002ac0: 0166 027d 0574 036a 047c 007c 0574 036a  .f.}.t.j.|.|.t.j
+00002ad0: 0564 028d 037d 067c 0653 0029 034e 7280  .d...}.|.S.).Nr.
+00002ae0: 0000 0029 015a 0d69 6e74 6572 706f 6c61  ...).Z.interpola
+00002af0: 7469 6f6e 2906 7282 0000 00da 0566 6c6f  tion).r......flo
+00002b00: 6174 7255 0000 0072 8300 0000 726a 0000  atrU...r....rj..
+00002b10: 005a 0a49 4e54 4552 5f41 5245 4129 0772  .Z.INTER_AREA).r
+00002b20: 9700 0000 7281 0000 005a 0e63 7572 7265  ....r....Z.curre
+00002b30: 6e74 5f68 6569 6768 745a 0d63 7572 7265  nt_heightZ.curre
+00002b40: 6e74 5f77 6964 7468 5a05 7261 7469 6f5a  nt_widthZ.ratioZ
+00002b50: 0364 696d 5a07 7265 7369 7a65 6472 2b00  .dimZ.resizedr+.
+00002b60: 0000 722b 0000 0072 2c00 0000 726a 0000  ..r+...r,...rj..
+00002b70: 0077 0100 0073 0a00 0000 1201 0c01 1001  .w...s..........
+00002b80: 1201 0401 726a 0000 0063 0100 0000 0000  ....rj...c......
+00002b90: 0000 0000 0000 0300 0000 0500 0000 4300  ..............C.
+00002ba0: 0000 7332 0000 0074 00a0 017c 0074 006a  ..s2...t...|.t.j
+00002bb0: 02a1 027d 0174 037c 016a 047c 016a 0564  ...}.t.|.j.|.j.d
+00002bc0: 0119 007c 016a 0564 0219 0074 036a 066a  ...|.j.d...t.j.j
+00002bd0: 0783 047d 027c 0253 0029 034e 7252 0000  ...}.|.S.).NrR..
+00002be0: 0072 0100 0000 2908 7283 0000 005a 0863  .r....).r....Z.c
+00002bf0: 7674 436f 6c6f 725a 0d43 4f4c 4f52 5f42  vtColorZ.COLOR_B
+00002c00: 4752 3252 4742 720a 0000 00da 0464 6174  GR2RGBr......dat
+00002c10: 6172 8200 0000 5a06 466f 726d 6174 5a0d  ar....Z.FormatZ.
+00002c20: 466f 726d 6174 5f52 4742 3838 3829 0372  Format_RGB888).r
+00002c30: 7d00 0000 7297 0000 005a 0871 745f 6672  }...r....Z.qt_fr
+00002c40: 616d 6572 2b00 0000 722b 0000 0072 2c00  amer+...r+...r,.
+00002c50: 0000 7295 0000 0080 0100 0073 1000 0000  ..r........s....
+00002c60: 0e01 0202 0401 0801 0801 0601 04fc 0406  ................
+00002c70: 7295 0000 0063 0100 0000 0000 0000 0000  r....c..........
+00002c80: 0000 0500 0000 0400 0000 4300 0000 7348  ..........C...sH
+00002c90: 0000 0074 007c 0083 017d 0174 017c 0183  ...t.|...}.t.|..
+00002ca0: 017d 027c 02a0 0274 036a 04a1 0101 0074  .}.|...t.j.....t
+00002cb0: 0574 066a 0783 017d 0374 087c 0283 017d  .t.j...}.t.|...}
+00002cc0: 047c 04a0 09a1 0001 0074 06a0 0a7c 03a0  .|.......t...|..
+00002cd0: 0ba1 00a1 0101 0064 0053 0072 5c00 0000  .......d.S.r\...
+00002ce0: 290c 7223 0000 0072 1e00 0000 5a08 7365  ).r#...r....Z.se
+00002cf0: 745f 6d6f 6465 721f 0000 005a 0952 6563  t_moder....Z.Rec
+00002d00: 6f72 6469 6e67 720d 0000 00da 0373 7973  ordingr......sys
+00002d10: da04 6172 6776 722d 0000 005a 0473 686f  ..argvr-...Z.sho
+00002d20: 77da 0465 7869 74da 0465 7865 6329 05da  w..exit..exec)..
+00002d30: 0c73 6573 7369 6f6e 5f70 6174 68da 0663  .session_path..c
+00002d40: 6f6e 6669 6772 2e00 0000 5a03 4170 705a  onfigr....Z.AppZ
+00002d50: 1072 6563 6f72 6469 6e67 5f64 6961 6c6f  .recording_dialo
+00002d60: 6772 2b00 0000 722b 0000 0072 2c00 0000  gr+...r+...r,...
+00002d70: da17 6c61 756e 6368 5f72 6563 6f72 6469  ..launch_recordi
+00002d80: 6e67 5f77 6964 6765 748c 0100 0073 0e00  ng_widget....s..
+00002d90: 0000 0801 0801 0c03 0a01 0801 0801 1202  ................
+00002da0: 72a5 0000 0029 3fda 0d70 7978 7933 642e  r....)?..pyxy3d.
+00002db0: 6c6f 6767 6572 da06 7079 7879 3364 7264  logger..pyxy3drd
+00002dc0: 0000 0072 8e00 0000 7225 0000 0072 9f00  ...r....r%...r..
+00002dd0: 0000 7273 0000 00da 0770 6174 686c 6962  ..rs.....pathlib
+00002de0: 7202 0000 00da 0974 6872 6561 6469 6e67  r......threading
+00002df0: 7203 0000 0072 0400 0000 da05 6e75 6d70  r....r......nump
+00002e00: 7972 7c00 0000 da05 7175 6575 6572 0500  yr|.....queuer..
+00002e10: 0000 da04 656e 756d 7206 0000 0072 8300  ....enumr....r..
+00002e20: 0000 5a0c 5079 5174 362e 5174 436f 7265  ..Z.PyQt6.QtCore
+00002e30: 7207 0000 0072 0800 0000 7209 0000 005a  r....r....r....Z
+00002e40: 0b50 7951 7436 2e51 7447 7569 720a 0000  .PyQt6.QtGuir...
+00002e50: 0072 0b00 0000 720c 0000 00da 0f50 7951  .r....r......PyQ
+00002e60: 7436 2e51 7457 6964 6765 7473 720d 0000  t6.QtWidgetsr...
+00002e70: 0072 0e00 0000 720f 0000 0072 1000 0000  .r....r....r....
+00002e80: 7211 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
+00002e90: 1400 0000 7215 0000 0072 1600 0000 7217  ....r....r....r.
+00002ea0: 0000 0072 1800 0000 7219 0000 0072 1a00  ...r....r....r..
+00002eb0: 0000 721b 0000 0072 1c00 0000 721d 0000  ..r....r....r...
+00002ec0: 005a 1670 7978 7933 642e 7365 7373 696f  .Z.pyxy3d.sessio
+00002ed0: 6e2e 7365 7373 696f 6e72 1e00 0000 721f  n.sessionr....r.
+00002ee0: 0000 005a 1b70 7978 7933 642e 6361 6d65  ...Z.pyxy3d.came
+00002ef0: 7261 732e 7379 6e63 6872 6f6e 697a 6572  ras.synchronizer
+00002f00: 7220 0000 0072 2100 0000 5a1f 7079 7879  r ...r!...Z.pyxy
+00002f10: 3364 2e72 6563 6f72 6469 6e67 2e76 6964  3d.recording.vid
+00002f20: 656f 5f72 6563 6f72 6465 7272 2200 0000  eo_recorderr"...
+00002f30: 5a13 7079 7879 3364 2e63 6f6e 6669 6775  Z.pyxy3d.configu
+00002f40: 7261 746f 7272 2300 0000 7224 0000 0072  ratorr#...r$...r
+00002f50: 2d00 0000 7232 0000 0072 3400 0000 729c  -...r2...r4...r.
+00002f60: 0000 0072 6a00 0000 7295 0000 0072 a500  ...rj...r....r..
+00002f70: 0000 722b 0000 0072 2b00 0000 722b 0000  ..r+...r+...r+..
+00002f80: 0072 2c00 0000 da08 3c6d 6f64 756c 653e  .r,.....<module>
+00002f90: 0100 0000 7338 0000 0008 020c 0108 0208  ....s8..........
+00002fa0: 010c 0110 0108 010c 010c 0108 0214 0114  ................
+00002fb0: 014c 0110 140c 010c 010c 010c 0110 0210  .L..............
+00002fc0: 0600 7f0e 0b00 7f10 1b08 1e08 0408 090c  ................
+00002fd0: 0c                                       .
```

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/__pycache__/recording_widget.cpython-38.pyc` & `pyxy3d-0.1.4/pyxy3d/gui/__pycache__/recording_widget.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/__pycache__/widgets.cpython-310.pyc` & `pyxy3d-0.1.4/pyxy3d/gui/__pycache__/widgets.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/__pycache__/widgets.cpython-38.pyc` & `pyxy3d-0.1.4/pyxy3d/gui/__pycache__/widgets.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/__pycache__/wizard_charuco.cpython-310.pyc` & `pyxy3d-0.1.4/pyxy3d/gui/__pycache__/wizard_charuco.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/__pycache__/wizard_charuco.cpython-38.pyc` & `pyxy3d-0.1.4/pyxy3d/gui/__pycache__/wizard_charuco.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/__pycache__/wizard_directory.cpython-310.pyc` & `pyxy3d-0.1.4/pyxy3d/gui/__pycache__/wizard_directory.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/__pycache__/wizard_directory.cpython-38.pyc` & `pyxy3d-0.1.4/pyxy3d/gui/__pycache__/wizard_directory.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/calibrate_capture_volume_widget.py` & `pyxy3d-0.1.4/pyxy3d/gui/calibrate_capture_volume_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/camera_config/__pycache__/camera_config_dialogue.cpython-310.pyc` & `pyxy3d-0.1.4/pyxy3d/gui/camera_config/__pycache__/camera_config_dialogue.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/camera_config/__pycache__/camera_config_dialogue.cpython-38.pyc` & `pyxy3d-0.1.4/pyxy3d/gui/camera_config/__pycache__/camera_config_dialogue.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/camera_config/__pycache__/camera_summary_widget.cpython-310.pyc` & `pyxy3d-0.1.4/pyxy3d/gui/camera_config/__pycache__/camera_summary_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/camera_config/__pycache__/camera_tabs.cpython-310.pyc` & `pyxy3d-0.1.4/pyxy3d/gui/camera_config/__pycache__/camera_tabs.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/camera_config/__pycache__/camera_tabs.cpython-38.pyc` & `pyxy3d-0.1.4/pyxy3d/gui/camera_config/__pycache__/camera_tabs.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/camera_config/__pycache__/frame_emitter.cpython-310.pyc` & `pyxy3d-0.1.4/pyxy3d/gui/camera_config/__pycache__/frame_emitter.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/camera_config/__pycache__/frame_emitter.cpython-38.pyc` & `pyxy3d-0.1.4/pyxy3d/gui/camera_config/__pycache__/frame_emitter.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/camera_config/__pycache__/intrinsic_calibration_widget.cpython-310.pyc` & `pyxy3d-0.1.4/pyxy3d/gui/camera_config/__pycache__/intrinsic_calibration_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/camera_config/camera_config_dialogue.py` & `pyxy3d-0.1.4/pyxy3d/gui/camera_config/camera_config_dialogue.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/camera_config/camera_summary_widget.py` & `pyxy3d-0.1.4/pyxy3d/gui/camera_config/camera_summary_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/camera_config/frame_emitter.py` & `pyxy3d-0.1.4/pyxy3d/gui/camera_config/frame_emitter.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/camera_config/intrinsic_calibration_widget.py` & `pyxy3d-0.1.4/pyxy3d/gui/camera_config/intrinsic_calibration_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/charuco_widget.py` & `pyxy3d-0.1.4/pyxy3d/gui/charuco_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/extrinsic_calibration_widget.py` & `pyxy3d-0.1.4/pyxy3d/gui/extrinsic_calibration_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/frame_builders/__pycache__/extrinsic_calibration_widget.cpython-310.pyc` & `pyxy3d-0.1.4/pyxy3d/gui/frame_builders/__pycache__/extrinsic_calibration_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/frame_builders/__pycache__/omni_frame_builder.cpython-38.pyc` & `pyxy3d-0.1.4/pyxy3d/gui/frame_builders/__pycache__/omni_frame_builder.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/frame_builders/__pycache__/omni_frame_widget.cpython-38.pyc` & `pyxy3d-0.1.4/pyxy3d/gui/frame_builders/__pycache__/omni_frame_widget.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/frame_builders/__pycache__/paired_frame_builder.cpython-310.pyc` & `pyxy3d-0.1.4/pyxy3d/gui/frame_builders/__pycache__/paired_frame_builder.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_builder.cpython-310.pyc` & `pyxy3d-0.1.4/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_builder.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_builder.cpython-38.pyc` & `pyxy3d-0.1.4/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_builder.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_widget.cpython-310.pyc` & `pyxy3d-0.1.4/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_widget.cpython-38.pyc` & `pyxy3d-0.1.4/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_widget.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/frame_builders/paired_frame_builder.py` & `pyxy3d-0.1.4/pyxy3d/gui/frame_builders/paired_frame_builder.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/icons/pyxy_logo.svg` & `pyxy3d-0.1.4/pyxy3d/gui/icons/pyxy_logo.svg`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/icons/rotate-camera-left.svg` & `pyxy3d-0.1.4/pyxy3d/gui/icons/rotate-camera-left.svg`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/icons/rotate-camera-right.svg` & `pyxy3d-0.1.4/pyxy3d/gui/icons/rotate-camera-right.svg`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/log_widget.py` & `pyxy3d-0.1.4/pyxy3d/gui/log_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/main_widget.py` & `pyxy3d-0.1.4/pyxy3d/gui/main_widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 from enum import Enum
 from PyQt6.QtGui import QIcon, QAction, QKeySequence, QShortcut
 from PyQt6.QtCore import Qt
 from pyxy3d import __root__, __settings_path__, __user_dir__
 from pyxy3d.session.session import Session, SessionMode
 from pyxy3d.gui.log_widget import LogWidget
 from pyxy3d.configurator import Configurator
-from pyxy3d.gui.calibration_widget import CalibrationWidget
 from pyxy3d.gui.charuco_widget import CharucoWidget
 from pyxy3d.gui.camera_config.intrinsic_calibration_widget import (
     IntrinsicCalibrationWidget,
 )
 from pyxy3d.gui.calibrate_capture_volume_widget import CalibrateCaptureVolumeWidget
 from pyxy3d.gui.recording_widget import RecordingWidget
 from pyxy3d.gui.post_processing_widget import PostProcessingWidget
@@ -130,15 +129,15 @@
         logger.info("Pausing all frame reading at load of stream tools; should be on charuco tab right now")
         self.session.pause_all_monocalibrators()
         self.session.pause_synchronizer()  
 
     def load_stream_tools(self):
         self.connect_cameras_action.setEnabled(False)
         self.disconnect_cameras_action.setEnabled(True)
-        self.session.stream_tools_loaded_signal.connect(self.pause_all_frame_reading)
+        self.session.qt_signaler.stream_tools_loaded_signal.connect(self.pause_all_frame_reading)
         self.thread = Thread(
             target=self.session.load_stream_tools, args=(), daemon=True
         )
         self.thread.start()
 
             
             
@@ -262,16 +261,16 @@
 
 
     def connect_session_signals(self):
         """
         After launching a session, connect signals and slots.
         Much of these will be from the GUI to the session and vice-versa
         """
-        self.session.unlock_postprocessing.connect(self.load_post_processing_widget)
-        self.session.stream_tools_loaded_signal.connect(self.update_tabs)
+        self.session.qt_signaler.unlock_postprocessing.connect(self.load_post_processing_widget)
+        self.session.qt_signaler.stream_tools_loaded_signal.connect(self.update_tabs)
 
     def load_recording_widget(self):
         # recording_index = self.tab_widget.indexOf(self.recording_widget)
         self.tab_widget.removeTab(TabIndex.Recording.value)
         self.recording_widget.deleteLater()
         new_recording_widget = RecordingWidget(self.session)
         self.tab_widget.insertTab(
```

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/navigation_bars.py` & `pyxy3d-0.1.4/pyxy3d/gui/navigation_bars.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/playback_widget.py` & `pyxy3d-0.1.4/pyxy3d/gui/playback_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/post_processing_widget.py` & `pyxy3d-0.1.4/pyxy3d/gui/post_processing_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/progress_dialog.py` & `pyxy3d-0.1.4/pyxy3d/gui/progress_dialog.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/recording_widget.py` & `pyxy3d-0.1.4/pyxy3d/gui/recording_widget.py`

 * *Files 3% similar despite different names*

```diff
@@ -126,17 +126,18 @@
 
     def connect_widgets(self):
     
         self.unpaired_frame_emitter.ImageBroadcast.connect(self.ImageUpdateSlot)
         self.frame_rate_spin.valueChanged.connect(self.session.set_active_mode_fps)
         self.unpaired_frame_emitter.dropped_fps.connect(self.update_dropped_fps)
         self.start_stop.clicked.connect(self.toggle_start_stop)
-        self.session.recording_complete_signal.connect(self.on_recording_complete)
+        self.session.qt_signaler.recording_complete_signal.connect(self.on_recording_complete)
 
     def toggle_start_stop(self):
+        logger.info("Start/Stop Recording Toggled...")
         if self.next_action == NextRecordingActions.StartRecording:
             self.next_action = NextRecordingActions.StopRecording
             self.start_stop.setText(self.next_action.value)
             self.recording_directory.setEnabled(False)
 
             logger.info("Initiate recording")
             recording_path:Path = Path(self.session.path, self.recording_directory.text()) 
@@ -144,26 +145,34 @@
 
         elif self.next_action == NextRecordingActions.StopRecording:
             self.start_stop.setEnabled(False)
             # need to wait for session to signal that recording is complete
             self.next_action = NextRecordingActions.AwaitSave
             # self.start_stop.setText("HELLO")
             self.start_stop.setText(self.next_action.value)
+            logger.info("Stop recording and initiate final save of file") 
             self.session.stop_recording()
 
+            next_recording = self.get_next_recording_directory()
             self.recording_directory.setEnabled(True)
-            logger.info("Stop recording and initiate final save of file") 
-            self.recording_directory.setText(self.get_next_recording_directory())
+            self.recording_directory.setText(next_recording)
+            logger.info(f"successfully reset text and renamed recording directory to {next_recording}")
 
+        elif self.next_action == NextRecordingActions.AwaitSave:
+            logger.info("recording button toggled while awaiting save")
+            
     def on_recording_complete(self):
         logger.info("Recording complete signal received...updating next action and button")
         self.next_action = NextRecordingActions.StartRecording
         self.start_stop.setText(self.next_action.value)
-        self.start_stop.setEnabled(True)
         logger.info("Enabling start/stop recording button")
+        self.start_stop.setEnabled(True)
+        logger.info("Successfully enabled start/stop recording button")
+        # pass
+        
                     
     def update_dropped_fps(self, dropped_fps:dict):
         "Unravel dropped fps dictionary to a more readable string"
         text = "Rate of Frame Dropping by Port:    "
         for port, drop_rate in dropped_fps.items():
             text += f"{port}: {drop_rate:.0%}        "
```

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/vizualize/__pycache__/camera_mesh.cpython-310.pyc` & `pyxy3d-0.1.4/pyxy3d/gui/vizualize/__pycache__/camera_mesh.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/vizualize/__pycache__/camera_mesh.cpython-38.pyc` & `pyxy3d-0.1.4/pyxy3d/gui/vizualize/__pycache__/camera_mesh.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/vizualize/__pycache__/capture_volume_dialog.cpython-38.pyc` & `pyxy3d-0.1.4/pyxy3d/gui/vizualize/__pycache__/capture_volume_dialog.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/vizualize/__pycache__/capture_volume_visualizer.cpython-38.pyc` & `pyxy3d-0.1.4/pyxy3d/gui/vizualize/__pycache__/capture_volume_visualizer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/vizualize/__pycache__/capture_volume_widget.cpython-38.pyc` & `pyxy3d-0.1.4/pyxy3d/gui/vizualize/__pycache__/capture_volume_widget.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/vizualize/__pycache__/playback_triangulation_widget.cpython-310.pyc` & `pyxy3d-0.1.4/pyxy3d/gui/vizualize/__pycache__/playback_triangulation_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/vizualize/__pycache__/realtime_triangulation_widget.cpython-310.pyc` & `pyxy3d-0.1.4/pyxy3d/gui/vizualize/__pycache__/realtime_triangulation_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_visualizer.cpython-310.pyc` & `pyxy3d-0.1.4/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_visualizer.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_visualizer.cpython-38.pyc` & `pyxy3d-0.1.4/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_visualizer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_widget.cpython-310.pyc` & `pyxy3d-0.1.4/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_widget.cpython-38.pyc` & `pyxy3d-0.1.4/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_widget.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/vizualize/calibration/capture_volume_visualizer.py` & `pyxy3d-0.1.4/pyxy3d/gui/vizualize/calibration/capture_volume_visualizer.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/vizualize/calibration/capture_volume_widget.py` & `pyxy3d-0.1.4/pyxy3d/gui/vizualize/calibration/capture_volume_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/vizualize/camera_mesh.py` & `pyxy3d-0.1.4/pyxy3d/gui/vizualize/camera_mesh.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/vizualize/playback_triangulation_widget.py` & `pyxy3d-0.1.4/pyxy3d/gui/vizualize/playback_triangulation_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/gui/vizualize/realtime_triangulation_widget.py` & `pyxy3d-0.1.4/pyxy3d/gui/vizualize/realtime_triangulation_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/helper.py` & `pyxy3d-0.1.4/pyxy3d/helper.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/interface.py` & `pyxy3d-0.1.4/pyxy3d/interface.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/logger.py` & `pyxy3d-0.1.4/pyxy3d/logger.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/post_processor.py` & `pyxy3d-0.1.4/pyxy3d/post_processor.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,19 +28,19 @@
 from pyxy3d.trackers.tracker_enum import TrackerEnum
 from pyxy3d.gui.playback_widget import PlaybackWidget
 
 # specify a source directory (with recordings)
 from pyxy3d.helper import copy_contents
 
 
-class PostProcessor(QObject):
-    progress_update = pyqtSignal(dict)  # {"stage": str, "percent":int}
+class PostProcessor:
+    # progress_update = pyqtSignal(dict)  # {"stage": str, "percent":int}
 
     def __init__(self,config:Configurator ):
-        super().__init__()
+        # super().__init__()
         self.config = config
 
     def create_xyz(self, recording_path: Path, tracker_enum: TrackerEnum,) -> None:
         """
         creates xyz_{tracker name}.csv file within the recording_path directory
 
         Uses the two functions above, first creating the xy points based on the tracker if they 
@@ -100,20 +100,20 @@
         logger.info("Initiate playback and processing")
         stream_pool.play_videos()
 
         while video_recorder.recording:
             sleep(1)
             percent_complete = int((video_recorder.sync_index / sync_index_count) * 100)
             logger.info(f"(Stage 1 of 2): {percent_complete}% of frames processed for (x,y) landmark detection")
-            self.progress_update.emit(
-                {
-                    "stage": "Estimating (x,y) landmark positions (stage 1 of 2)",
-                    "percent": percent_complete,
-                }
-            )
+            # self.progress_update.emit(
+            #     {
+            #         "stage": "Estimating (x,y) landmark positions (stage 1 of 2)",
+            #         "percent": percent_complete,
+            #     }
+            # )
 
 
     def triangulate_xy_data(self, xy_data: pd.DataFrame) -> Dict[str, List]:
         
         camera_array = self.config.get_camera_array()
         # assemble numba compatible dictionary
         projection_matrices = Dict()
@@ -159,25 +159,24 @@
             # only log percent complete each second
             if int(time()) - last_log_update >= 1:
                 percent_complete = int(100*(index/sync_index_max))
                 logger.info(
                     f"(Stage 2 of 2): Triangulation of (x,y) point estimates is {percent_complete}% complete"
                 )
                 last_log_update = int(time())
-                self.progress_update.emit(
-                    {
-                        "stage": "Triangulating (x,y,z) estimates (stage 2 of 2)",
-                        "percent": percent_complete,
-                    }
-                )
+                # self.progress_update.emit(
+                #     {
+                #         "stage": "Triangulating (x,y,z) estimates (stage 2 of 2)",
+                #         "percent": percent_complete,
+                #     }
+                # )
 
         # signalling the progress bar can now close
-        self.progress_update.emit(
-            {
-                "stage": "Triangulating (x,y,z) estimates (stage 2 of 2)",
-                "percent": 100,
-                "close": True
-            }
-        )
+        # self.progress_update.emit(
+        #     {
+        #         "stage": "Triangulating (x,y,z) estimates (stage 2 of 2)",
+        #         "percent": 100,
+        #         "close": True
+        #     }
+        # )
 
         return xyz_history
-
```

### Comparing `pyxy3d-0.1.3/pyxy3d/recording/__pycache__/recorded_stream.cpython-310.pyc` & `pyxy3d-0.1.4/pyxy3d/recording/__pycache__/recorded_stream.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/recording/__pycache__/recorded_stream.cpython-38.pyc` & `pyxy3d-0.1.4/pyxy3d/recording/__pycache__/recorded_stream.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/recording/__pycache__/video_recorder.cpython-310.pyc` & `pyxy3d-0.1.4/pyxy3d/recording/__pycache__/video_recorder.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jun 12 12:14:10 2023 UTC, .py size: 8730 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,371 +1,381 @@
-00000000: 6f0d 0d0a 0000 0000 120c 8764 1a22 0000  o..........d."..
+00000000: 6f0d 0d0a 0000 0000 06e2 9564 9123 0000  o..........d.#..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 a800 0000 6400  .....@...s....d.
+00000020: 0003 0000 0040 0000 0073 9600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6501 6a02 a003 6504 a101  d.l.Z.e.j...e...
-00000040: 5a02 6400 6402 6c05 6d06 5a06 6d07 5a07  Z.d.d.l.m.Z.m.Z.
-00000050: 0100 6400 6403 6c08 6d09 5a09 0100 6400  ..d.d.l.m.Z...d.
-00000060: 6404 6c0a 6d0b 5a0b 0100 6400 6405 6c0c  d.l.m.Z...d.d.l.
-00000070: 6d0d 5a0d 6d0e 5a0e 0100 6400 6401 6c0f  m.Z.m.Z...d.d.l.
-00000080: 5a0f 6400 6401 6c10 5a10 6400 6401 6c11  Z.d.d.l.Z.d.d.l.
-00000090: 5a12 6400 6401 6c13 5a13 6400 6406 6c14  Z.d.d.l.Z.d.d.l.
-000000a0: 6d15 5a15 0100 6400 6407 6c16 6d17 5a17  m.Z...d.d.l.m.Z.
-000000b0: 0100 6400 6408 6c18 6d19 5a19 6d1a 5a1a  ..d.d.l.m.Z.m.Z.
-000000c0: 0100 4700 6409 640a 8400 640a 6506 8303  ..G.d.d...d.e...
-000000d0: 5a1b 6401 5300 290b e900 0000 004e 2902  Z.d.S.)......N).
-000000e0: da07 514f 626a 6563 74da 0a70 7971 7453  ..QObject..pyqtS
-000000f0: 6967 6e61 6c29 01da 0450 6174 6829 01da  ignal)...Path)..
-00000100: 0551 7565 7565 2902 da06 5468 7265 6164  .Queue)...Thread
-00000110: da05 4576 656e 7429 01da 0c53 796e 6368  ..Event)...Synch
-00000120: 726f 6e69 7a65 7229 01da 0a4c 6976 6553  ronizer)...LiveS
-00000130: 7472 6561 6d29 02da 0b46 7261 6d65 5061  tream)...FramePa
-00000140: 636b 6574 da0a 5379 6e63 5061 636b 6574  cket..SyncPacket
-00000150: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000160: 0006 0000 0000 0000 0073 8800 0000 6500  .........s....e.
-00000170: 5a01 6400 5a02 6503 8300 5a04 6503 8300  Z.d.Z.e...Z.e...
-00000180: 5a05 641a 6402 6506 6403 6507 6604 8700  Z.d.d.e.d.e.f...
-00000190: 6601 6404 6405 840d 5a08 6406 6407 8400  f.d.d...Z.d.d...
-000001a0: 5a09 6408 650a 6409 650a 640a 650a 6606  Z.d.e.d.e.d.e.f.
-000001b0: 640b 640c 8404 5a0b 640d 640e 8400 5a0c  d.d...Z.d.d...Z.
-000001c0: 640f 6410 8400 5a0d 6411 6412 8400 5a0e  d.d...Z.d.d...Z.
-000001d0: 0913 0914 0913 641b 6415 650f 6602 6416  ......d.d.e.f.d.
-000001e0: 6417 8405 5a10 6418 6419 8400 5a11 8700  d...Z.d.d...Z...
-000001f0: 0400 5a12 5300 291c da0d 5669 6465 6f52  ..Z.S.)...VideoR
-00000200: 6563 6f72 6465 724e da0c 7379 6e63 6872  ecorderN..synchr
-00000210: 6f6e 697a 6572 da06 7375 6666 6978 6303  onizer..suffixc.
-00000220: 0000 0000 0000 0000 0000 0003 0000 0002  ................
-00000230: 0000 0003 0000 0073 4200 0000 7400 8300  .......sB...t...
-00000240: a001 a100 0100 7c01 7c00 5f02 7c02 6400  ......|.|._.|.d.
-00000250: 7501 7212 6401 7c02 1700 7c00 5f03 6e03  u.r.d.|...|._.n.
-00000260: 6402 7c00 5f03 6403 7c00 5f04 6404 7c00  d.|._.d.|._.d.|.
-00000270: 5f05 7406 8300 7c00 5f07 6400 5300 2905  _.t...|._.d.S.).
-00000280: 4eda 015f da00 4672 0100 0000 2908 da05  N.._..Fr....)...
-00000290: 7375 7065 72da 085f 5f69 6e69 745f 5f72  super..__init__r
-000002a0: 0d00 0000 720e 0000 00da 0972 6563 6f72  ....r......recor
-000002b0: 6469 6e67 da0a 7379 6e63 5f69 6e64 6578  ding..sync_index
-000002c0: 7207 0000 00da 0c74 7269 6767 6572 5f73  r......trigger_s
-000002d0: 746f 7029 03da 0473 656c 6672 0d00 0000  top)...selfr....
-000002e0: 720e 0000 00a9 01da 095f 5f63 6c61 7373  r........__class
-000002f0: 5f5f a900 fa43 433a 5c55 7365 7273 5c4d  __...CC:\Users\M
-00000300: 6163 2050 7269 626c 655c 7265 706f 735c  ac Prible\repos\
-00000310: 7079 7879 3364 5c70 7978 7933 645c 7265  pyxy3d\pyxy3d\re
-00000320: 636f 7264 696e 675c 7669 6465 6f5f 7265  cording\video_re
-00000330: 636f 7264 6572 2e70 7972 1200 0000 1700  corder.pyr......
-00000340: 0000 7310 0000 000a 0106 0108 040c 0106  ..s.............
-00000350: 0206 0206 010c 027a 1656 6964 656f 5265  .......z.VideoRe
-00000360: 636f 7264 6572 2e5f 5f69 6e69 745f 5f63  corder.__init__c
-00000370: 0100 0000 0000 0000 0000 0000 0700 0000  ................
-00000380: 0800 0000 4300 0000 7382 0000 0069 007c  ....C...s....i.|
-00000390: 005f 007c 006a 016a 02a0 03a1 0044 005d  ._.|.j.j.....D.]
-000003a0: 355c 027d 017d 0274 0474 057c 006a 0664  5\.}.}.t.t.|.j.d
-000003b0: 017c 019b 007c 006a 079b 0064 029d 0483  .|...|.j...d....
-000003c0: 0283 017d 0374 08a0 0964 037c 019b 0064  ...}.t...d.|...d
-000003d0: 047c 039b 009d 04a1 0101 0074 0a6a 0b64  .|.........t.j.d
-000003e0: 058e 007d 047c 026a 0c6a 0d7d 0574 0aa0  ...}.|.j.j.}.t..
-000003f0: 0e7c 037c 047c 026a 0f7c 05a1 047d 067c  .|.|.|.j.|...}.|
-00000400: 067c 006a 007c 013c 0071 0964 0653 0029  .|.j.|.<.q.d.S.)
-00000410: 077a ba0a 2020 2020 2020 2020 7375 6666  .z..        suff
-00000420: 6978 2070 726f 7669 6465 7320 6120 7761  ix provides a wa
-00000430: 7920 746f 2070 726f 7669 6465 2061 6464  y to provide add
-00000440: 6974 696f 6e61 6c20 6c61 6265 6c73 2074  itional labels t
-00000450: 6f20 7468 6520 6d70 3420 6669 6c65 206e  o the mp4 file n
-00000460: 616d 650a 2020 2020 2020 2020 5468 6973  ame.        This
-00000470: 2077 6f75 6c64 2062 6520 7265 6c65 7661   would be releva
-00000480: 6e74 2077 6865 6e20 7065 7266 6f72 6d69  nt when performi
-00000490: 6e67 2070 6f73 742d 7072 6f63 6573 7369  ng post-processi
-000004a0: 6e67 2061 6e64 2073 6176 696e 6720 6f75  ng and saving ou
-000004b0: 7420 6672 616d 6573 2077 6974 6820 706f  t frames with po
-000004c0: 696e 7473 0a20 2020 2020 2020 205a 0570  ints.        Z.p
-000004d0: 6f72 745f 7a04 2e6d 7034 7a1f 4275 696c  ort_z..mp4z.Buil
-000004e0: 6469 6e67 2076 6964 656f 2077 7269 7465  ding video write
-000004f0: 7220 666f 7220 706f 7274 207a 0f3b 2072  r for port z.; r
-00000500: 6563 6f72 6469 6e67 2074 6f20 5a04 4d50  ecording to Z.MP
-00000510: 3456 4e29 10da 0d76 6964 656f 5f77 7269  4VN)...video_wri
-00000520: 7465 7273 720d 0000 00da 0773 7472 6561  tersr......strea
-00000530: 6d73 da05 6974 656d 73da 0373 7472 7204  ms..items..strr.
-00000540: 0000 00da 1264 6573 7469 6e61 7469 6f6e  .....destination
-00000550: 5f66 6f6c 6465 7272 0e00 0000 da06 6c6f  _folderr......lo
-00000560: 6767 6572 da04 696e 666f da03 6376 32da  gger..info..cv2.
-00000570: 1256 6964 656f 5772 6974 6572 5f66 6f75  .VideoWriter_fou
-00000580: 7263 63da 0663 616d 6572 61da 0473 697a  rcc..camera..siz
-00000590: 65da 0b56 6964 656f 5772 6974 6572 da03  e..VideoWriter..
-000005a0: 6670 7329 0772 1600 0000 da04 706f 7274  fps).r......port
-000005b0: da06 7374 7265 616d da04 7061 7468 5a06  ..stream..pathZ.
-000005c0: 666f 7572 6363 da0a 6672 616d 655f 7369  fourcc..frame_si
-000005d0: 7a65 da06 7772 6974 6572 7219 0000 0072  ze..writerr....r
-000005e0: 1900 0000 721a 0000 00da 1362 7569 6c64  ....r......build
-000005f0: 5f76 6964 656f 5f77 7269 7465 7273 2700  _video_writers'.
-00000600: 0000 7312 0000 0006 0614 011e 0116 010a  ..s.............
-00000610: 0108 0112 020c 0104 f97a 2156 6964 656f  .........z!Video
-00000620: 5265 636f 7264 6572 2e62 7569 6c64 5f76  Recorder.build_v
-00000630: 6964 656f 5f77 7269 7465 7273 da0d 696e  ideo_writers..in
-00000640: 636c 7564 655f 7669 6465 6fda 0b73 686f  clude_video..sho
-00000650: 775f 706f 696e 7473 da13 7374 6f72 655f  w_points..store_
-00000660: 706f 696e 745f 6869 7374 6f72 7963 0400  point_historyc..
-00000670: 0000 0000 0000 0000 0000 0f00 0000 0a00  ................
-00000680: 0000 4300 0000 7358 0200 007c 0172 067c  ..C...sX...|.r.|
-00000690: 00a0 00a1 0001 0067 0067 0067 0067 0064  .......g.g.g.g.d
-000006a0: 019c 047c 005f 0167 0067 0067 0067 0067  ...|._.g.g.g.g.g
-000006b0: 0067 0067 0067 0067 0064 029c 097c 005f  .g.g.g.g.d...|._
-000006c0: 0274 0364 0383 017c 005f 047c 006a 05a0  .t.d...|._.|.j..
-000006d0: 067c 006a 04a1 0101 0064 047d 047c 006a  .|.j.....d.}.|.j
-000006e0: 04a0 07a1 0064 056b 0473 357c 006a 08a0  .....d.k.s5|.j..
-000006f0: 09a1 0073 f07c 006a 04a0 0aa1 007d 057c  ...s.|.j.....}.|
-00000700: 006a 04a0 07a1 007d 067c 0664 0616 0064  .j.....}.|.d...d
-00000710: 056b 0272 547c 0664 056b 0372 5474 0ba0  .k.rT|.d.k.rTt..
-00000720: 0c64 077c 006a 04a0 07a1 009b 009d 02a1  .d.|.j..........
-00000730: 0101 007c 0564 0075 0072 5e74 0ba0 0c64  ...|.d.u.r^t...d
-00000740: 08a1 0101 006e 927c 056a 0d7c 005f 0d7c  .....n.|.j.|._.|
-00000750: 056a 0ea0 0fa1 0044 005d 625c 027d 077d  .j.....D.]b\.}.}
-00000760: 087c 0864 0075 0172 c97c 0272 757c 086a  .|.d.u.r.|.ru|.j
-00000770: 107d 096e 037c 086a 117d 097c 086a 127d  .}.n.|.j.}.|.j.}
-00000780: 0a7c 086a 137d 0b7c 0172 a97c 006a 147c  .|.j.}.|.r.|.j.|
-00000790: 0719 00a0 157c 09a1 0101 007c 006a 0164  .....|.....|.j.d
-000007a0: 0919 00a0 167c 006a 0da1 0101 007c 006a  .....|.j.....|.j
-000007b0: 0164 0a19 00a0 167c 07a1 0101 007c 006a  .d.....|.....|.j
-000007c0: 0164 0b19 00a0 167c 0aa1 0101 007c 006a  .d.....|.....|.j
-000007d0: 0164 0c19 00a0 167c 0ba1 0101 007c 08a0  .d.....|.....|..
-000007e0: 177c 006a 0da1 017d 0c7c 0c64 0075 0172  .|.j...}.|.d.u.r
-000007f0: c97c 006a 02a0 18a1 00a0 0fa1 0044 005d  .|.j.........D.]
-00000800: 0e5c 027d 0d7d 0e7c 006a 027c 0d19 00a0  .\.}.}.|.j.|....
-00000810: 197c 0c7c 0d19 00a1 0101 0071 ba71 677c  .|.|.......q.qg|
-00000820: 0473 e47c 006a 08a0 09a1 0072 e474 0ba0  .s.|.j.....r.t..
-00000830: 0c64 0da1 0101 0064 0e7d 047c 006a 05a0  .d.....d.}.|.j..
-00000840: 1a7c 006a 04a1 0101 007c 006a 1ba0 1ca1  .|.j.....|.j....
-00000850: 0001 007c 006a 04a0 07a1 0064 056b 0473  ...|.j.....d.k.s
-00000860: 357c 006a 08a0 09a1 0072 357c 0190 0172  5|.j.....r5|...r
-00000870: 1174 0ba0 0c64 0fa1 0101 007c 006a 056a  .t...d.....|.j.j
-00000880: 1d44 005d 097d 077c 006a 147c 0719 00a0  .D.].}.|.j.|....
-00000890: 1ea1 0001 0071 fc7c 0060 1474 0ba0 0c64  .....q.|.`.t...d
-000008a0: 10a1 0101 007c 00a0 1fa1 0001 0074 0ba0  .....|.......t..
-000008b0: 0c64 11a1 0101 007c 0390 0172 1d7c 00a0  .d.....|...r.|..
-000008c0: 20a1 0001 007c 006a 08a0 21a1 0001 0064   ....|.j..!....d
-000008d0: 047c 005f 227c 006a 23a0 1ca1 0001 0064  .|._"|.j#......d
-000008e0: 0053 0029 124e 2904 7214 0000 0072 2800  .S.).N).r....r(.
-000008f0: 0000 da0b 6672 616d 655f 696e 6465 78da  ....frame_index.
-00000900: 0a66 7261 6d65 5f74 696d 6529 0972 1400  .frame_time).r..
-00000910: 0000 7228 0000 0072 3100 0000 7232 0000  ..r(...r1...r2..
-00000920: 00da 0870 6f69 6e74 5f69 64da 0969 6d67  ...point_id..img
-00000930: 5f6c 6f63 5f78 da09 696d 675f 6c6f 635f  _loc_x..img_loc_
-00000940: 79da 096f 626a 5f6c 6f63 5f78 da09 6f62  y..obj_loc_x..ob
-00000950: 6a5f 6c6f 635f 79e9 ffff ffff 4672 0100  j_loc_y.....Fr..
-00000960: 0000 e919 0000 007a 3153 697a 6520 6f66  .......z1Size of
-00000970: 2075 6e73 6176 6564 2066 7261 6d65 7320   unsaved frames 
-00000980: 6f6e 2074 6865 2072 6563 6f72 6469 6e67  on the recording
-00000990: 2071 7565 7565 2069 7320 7a33 456e 6420   queue is z3End 
-000009a0: 6f66 2073 796e 6320 7061 636b 6574 7320  of sync packets 
-000009b0: 7369 676e 616c 6564 2e2e 2e62 7265 616b  signaled...break
-000009c0: 696e 6720 7265 636f 7264 206c 6f6f 7072  ing record loopr
-000009d0: 1400 0000 7228 0000 0072 3100 0000 7232  ....r(...r1...r2
-000009e0: 0000 007a 2153 6176 6520 6672 616d 6520  ...z!Save frame 
-000009f0: 776f 726b 6572 2077 696e 6469 6e67 2064  worker winding d
-00000a00: 6f77 6e2e 2e2e 547a 1a72 656c 6561 7369  own...Tz.releasi
-00000a10: 6e67 2076 6964 656f 2077 7269 7465 7273  ng video writers
-00000a20: 2e2e 2e7a 2149 6e69 7469 6174 6520 7374  ...z!Initiate st
-00000a30: 6f72 696e 6720 6f66 2066 7261 6d65 2068  oring of frame h
-00000a40: 6973 746f 7279 7a21 496e 6974 6961 7465  istoryz!Initiate
-00000a50: 2073 746f 7269 6e67 206f 6620 706f 696e   storing of poin
-00000a60: 7420 6869 7374 6f72 7929 2472 2d00 0000  t history)$r-...
-00000a70: da0d 6672 616d 655f 6869 7374 6f72 79da  ..frame_history.
-00000a80: 1270 6f69 6e74 5f64 6174 615f 6869 7374  .point_data_hist
-00000a90: 6f72 7972 0500 0000 5a10 7379 6e63 5f70  oryr....Z.sync_p
-00000aa0: 6163 6b65 745f 696e 5f71 720d 0000 00da  acket_in_qr.....
-00000ab0: 1973 7562 7363 7269 6265 5f74 6f5f 7379  .subscribe_to_sy
-00000ac0: 6e63 5f70 6163 6b65 7473 da05 7173 697a  nc_packets..qsiz
-00000ad0: 6572 1500 0000 da06 6973 5f73 6574 da03  er......is_set..
-00000ae0: 6765 7472 2000 0000 7221 0000 0072 1400  getr ...r!...r..
-00000af0: 0000 da0d 6672 616d 655f 7061 636b 6574  ....frame_packet
-00000b00: 7372 1d00 0000 da11 6672 616d 655f 7769  sr......frame_wi
-00000b10: 7468 5f70 6f69 6e74 73da 0566 7261 6d65  th_points..frame
-00000b20: 7231 0000 0072 3200 0000 721b 0000 00da  r1...r2...r.....
-00000b30: 0577 7269 7465 da06 6170 7065 6e64 da0d  .write..append..
-00000b40: 746f 5f74 6964 795f 7461 626c 65da 0463  to_tidy_table..c
-00000b50: 6f70 79da 0665 7874 656e 64da 1572 656c  opy..extend..rel
-00000b60: 6561 7365 5f73 796e 635f 7061 636b 6574  ease_sync_packet
-00000b70: 5f71 da15 7265 636f 7264 696e 675f 7374  _q..recording_st
-00000b80: 6f70 5f73 6967 6e61 6cda 0465 6d69 74da  op_signal..emit.
-00000b90: 0570 6f72 7473 da07 7265 6c65 6173 65da  .ports..release.
-00000ba0: 1373 746f 7265 5f66 7261 6d65 5f68 6973  .store_frame_his
-00000bb0: 746f 7279 7230 0000 00da 0563 6c65 6172  toryr0.....clear
-00000bc0: 7213 0000 00da 1761 6c6c 5f66 7261 6d65  r......all_frame
-00000bd0: 735f 7361 7665 645f 7369 676e 616c 290f  s_saved_signal).
-00000be0: 7216 0000 0072 2e00 0000 722f 0000 0072  r....r....r/...r
-00000bf0: 3000 0000 5a21 7379 6e63 726f 6e69 7a65  0...Z!syncronize
-00000c00: 725f 7375 6273 6372 6970 7469 6f6e 5f72  r_subscription_r
-00000c10: 656c 6561 7365 64da 0b73 796e 635f 7061  eleased..sync_pa
-00000c20: 636b 6574 da07 6261 636b 6c6f 6772 2800  cket..backlogr(.
-00000c30: 0000 da0c 6672 616d 655f 7061 636b 6574  ....frame_packet
-00000c40: 7242 0000 0072 3100 0000 7232 0000 005a  rB...r1...r2...Z
-00000c50: 0e6e 6577 5f74 6964 795f 7461 626c 65da  .new_tidy_table.
-00000c60: 036b 6579 da05 7661 6c75 6572 1900 0000  .key..valuer....
-00000c70: 7219 0000 0072 1a00 0000 da10 7361 7665  r....r......save
-00000c80: 5f64 6174 615f 776f 726b 6572 3700 0000  _data_worker7...
-00000c90: 7384 0000 0004 0308 0102 0402 0102 0102  s...............
-00000ca0: 0108 fc02 0802 0102 0102 0102 0102 0102  ................
-00000cb0: 0102 0102 0108 f70a 0c0e 0104 0118 030a  ................
-00000cc0: 010a 0314 0116 0108 020a 0202 0108 0212  ................
-00000cd0: 0208 0104 0308 0106 0206 0206 0104 0210  ................
-00000ce0: 0212 0310 0110 0110 010c 0208 0116 0116  ................
-00000cf0: 0102 800e 020a 0104 010e 010a 0118 d206  ................
-00000d00: 310a 010c 0110 0104 020a 0208 010a 0206  1...............
-00000d10: 0108 010a 0106 010e 017a 1e56 6964 656f  .........z.Video
-00000d20: 5265 636f 7264 6572 2e73 6176 655f 6461  Recorder.save_da
-00000d30: 7461 5f77 6f72 6b65 7263 0100 0000 0000  ta_workerc......
-00000d40: 0000 0000 0000 0300 0000 0600 0000 4300  ..............C.
-00000d50: 0000 734a 0000 0074 00a0 017c 006a 02a1  ..sJ...t...|.j..
-00000d60: 017d 0174 0374 047c 006a 0564 017c 006a  .}.t.t.|.j.d.|.j
-00000d70: 069b 0064 029d 0383 0283 017d 0274 07a0  ...d.......}.t..
-00000d80: 0864 037c 029b 009d 02a1 0101 007c 016a  .d.|.........|.j
-00000d90: 097c 0264 0464 0564 068d 0301 0064 0053  .|.d.d.d.....d.S
-00000da0: 0029 074e da02 7879 7a04 2e63 7376 7a16  .).N..xyz..csvz.
-00000db0: 5374 6f72 696e 6720 706f 696e 7420 6461  Storing point da
-00000dc0: 7461 2069 6e20 4654 a902 da05 696e 6465  ta in FT....inde
-00000dd0: 78da 0668 6561 6465 7229 0ada 0270 64da  x..header)...pd.
-00000de0: 0944 6174 6146 7261 6d65 723b 0000 0072  .DataFramer;...r
-00000df0: 1e00 0000 7204 0000 0072 1f00 0000 720e  ....r....r....r.
-00000e00: 0000 0072 2000 0000 7221 0000 00da 0674  ...r ...r!.....t
-00000e10: 6f5f 6373 7629 0372 1600 0000 da02 6466  o_csv).r......df
-00000e20: da0f 706f 696e 745f 6461 7461 5f70 6174  ..point_data_pat
-00000e30: 6872 1900 0000 7219 0000 0072 1a00 0000  hr....r....r....
-00000e40: 7230 0000 0099 0000 0073 0800 0000 0c01  r0.......s......
-00000e50: 1a01 1001 1401 7a21 5669 6465 6f52 6563  ......z!VideoRec
-00000e60: 6f72 6465 722e 7374 6f72 655f 706f 696e  order.store_poin
-00000e70: 745f 6869 7374 6f72 7963 0100 0000 0000  t_historyc......
-00000e80: 0000 0000 0000 0300 0000 0500 0000 4300  ..............C.
-00000e90: 0000 7340 0000 0074 00a0 017c 006a 02a1  ..s@...t...|.j..
-00000ea0: 017d 0174 0374 047c 006a 0564 0183 0283  .}.t.t.|.j.d....
-00000eb0: 017d 0274 06a0 0764 027c 029b 009d 02a1  .}.t...d.|......
-00000ec0: 0101 007c 016a 087c 0264 0364 0464 058d  ...|.j.|.d.d.d..
-00000ed0: 0301 0064 0053 0029 064e 7a16 6672 616d  ...d.S.).Nz.fram
-00000ee0: 655f 7469 6d65 5f68 6973 746f 7279 2e63  e_time_history.c
-00000ef0: 7376 7a19 5374 6f72 696e 6720 6672 616d  svz.Storing fram
-00000f00: 6520 6869 7374 6f72 7920 746f 2046 5472  e history to FTr
-00000f10: 5700 0000 2909 725a 0000 0072 5b00 0000  W...).rZ...r[...
-00000f20: 723a 0000 0072 1e00 0000 7204 0000 0072  r:...r....r....r
-00000f30: 1f00 0000 7220 0000 0072 2100 0000 725c  ....r ...r!...r\
-00000f40: 0000 0029 0372 1600 0000 725d 0000 005a  ...).r....r]...Z
-00000f50: 0f66 7261 6d65 5f68 6973 745f 7061 7468  .frame_hist_path
-00000f60: 7219 0000 0072 1900 0000 721a 0000 0072  r....r....r....r
-00000f70: 4d00 0000 9f00 0000 7308 0000 000c 0110  M.......s.......
-00000f80: 0110 0114 017a 2156 6964 656f 5265 636f  .....z!VideoReco
-00000f90: 7264 6572 2e73 746f 7265 5f66 7261 6d65  rder.store_frame
-00000fa0: 5f68 6973 746f 7279 6301 0000 0000 0000  _historyc.......
-00000fb0: 0000 0000 0001 0000 0001 0000 0043 0000  .............C..
-00000fc0: 0073 0400 0000 6400 5300 a901 4e72 1900  .s....d.S...Nr..
-00000fd0: 0000 a901 7216 0000 0072 1900 0000 7219  ....r....r....r.
-00000fe0: 0000 0072 1a00 0000 da13 7374 6f72 655f  ...r......store_
-00000ff0: 6163 7469 7665 5f63 6f6e 6669 67a5 0000  active_config...
-00001000: 0073 0200 0000 0401 7a21 5669 6465 6f52  .s......z!VideoR
-00001010: 6563 6f72 6465 722e 7374 6f72 655f 6163  ecorder.store_ac
-00001020: 7469 7665 5f63 6f6e 6669 6754 4672 1f00  tive_configTFr..
-00001030: 0000 6305 0000 0000 0000 0000 0000 0007  ..c.............
-00001040: 0000 0005 0000 0043 0000 0073 9800 0000  .......C...s....
-00001050: 7400 a001 6401 7c01 9b00 9d02 a101 0100  t...d.|.........
-00001060: 7c01 7c00 5f02 7c00 6a02 6a03 6402 6402  |.|._.|.j.j.d.d.
-00001070: 6403 8d02 0100 7c00 6a02 6a04 6a05 6404  d.....|.j.j.j.d.
-00001080: 6b02 7223 7406 7c00 6a02 6a04 6a04 6405  k.r#t.|.j.j.j.d.
-00001090: 8302 7d05 6e07 7406 7c00 6a02 6a04 6405  ..}.n.t.|.j.j.d.
-000010a0: 8302 7d05 7406 7c00 6a02 6405 8302 7d06  ..}.t.|.j.d...}.
-000010b0: 7407 a008 7c05 7c06 a102 0100 6402 7c00  t...|.|.....d.|.
-000010c0: 5f09 740a 7c00 6a0b 7c02 7c03 7c04 6703  _.t.|.j.|.|.|.g.
-000010d0: 6402 6406 8d03 7c00 5f0c 7c00 6a0c a00d  d.d...|._.|.j...
-000010e0: a100 0100 6407 5300 2908 61f5 0100 000a  ....d.S.).a.....
-000010f0: 2020 2020 2020 2020 4f70 7469 6f6e 2065          Option e
-00001100: 7869 7374 7320 746f 206e 6f74 2073 746f  xists to not sto
-00001110: 7265 2076 6964 656f 2069 6620 6f6e 6c79  re video if only
-00001120: 2069 6e74 6572 6573 7465 6420 696e 2067   interested in g
-00001130: 6574 7469 6e67 2070 6f69 6e74 7320 6672  etting points fr
-00001140: 6f6d 206f 7269 6769 6e61 6c20 7669 6465  om original vide
-00001150: 6f0a 2020 2020 2020 2020 0a20 2020 2020  o.        .     
-00001160: 2020 2050 6172 656e 7420 6f66 2064 6573     Parent of des
-00001170: 7469 6e61 7469 6f6e 2066 6f6c 6465 7220  tination folder 
-00001180: 7769 6c6c 2062 6520 7468 6520 736f 7572  will be the sour
-00001190: 6365 206f 6620 7468 6520 636f 6e66 6967  ce of the config
-000011a0: 2066 696c 6520 7468 6174 2077 696c 6c20   file that will 
-000011b0: 6265 2073 746f 7265 6420 7769 7468 2074  be stored with t
-000011c0: 6865 2076 6964 656f 0a20 2020 2020 2020  he video.       
-000011d0: 2054 6869 7320 656e 6162 6c65 7320 7468   This enables th
-000011e0: 6520 6e65 7374 6564 2070 726f 6365 7373  e nested process
-000011f0: 696e 6720 6f66 2076 6964 656f 7320 2869  ing of videos (i
-00001200: 2e65 2e20 5265 636f 7264 696e 675f 3120  .e. Recording_1 
-00001210: 7769 6c6c 2073 746f 7265 2074 6865 206d  will store the m
-00001220: 6169 6e20 636f 6e66 6967 2e74 6f6d 6c2c  ain config.toml,
-00001230: 0a20 2020 2020 2020 2074 6865 6e20 504f  .        then PO
-00001240: 5345 2073 7562 666f 6c64 6572 2077 696c  SE subfolder wil
-00001250: 6c20 7374 6f72 6520 636f 6e66 6967 2e74  l store config.t
-00001260: 6f6d 6c20 6672 6f6d 2052 6563 6f72 6469  oml from Recordi
-00001270: 6e67 5f31 292e 2045 6163 6820 666f 6c64  ng_1). Each fold
-00001280: 6572 2073 686f 756c 6420 6c61 7267 656c  er should largel
-00001290: 7920 6265 636f 6d65 2073 656c 660a 2020  y become self.  
-000012a0: 2020 2020 2020 636f 6e74 6169 6e65 6420        contained 
-000012b0: 616e 6420 706f 7274 6162 6c65 2066 6f72  and portable for
-000012c0: 2061 6e61 6c79 7369 7320 2f20 7265 636f   analysis / reco
-000012d0: 6e73 7472 7563 7469 6f6e 2e0a 2020 2020  nstruction..    
-000012e0: 2020 2020 7a1e 416c 6c20 7669 6465 6f20      z.All video 
-000012f0: 6461 7461 2074 6f20 6265 2073 6176 6564  data to be saved
-00001300: 2074 6f20 5429 02da 0865 7869 7374 5f6f   to T)...exist_o
-00001310: 6bda 0770 6172 656e 7473 da0b 6361 6c69  k..parents..cali
-00001320: 6272 6174 696f 6e7a 0b63 6f6e 6669 672e  brationz.config.
-00001330: 746f 6d6c 2903 da06 7461 7267 6574 da04  toml)...target..
-00001340: 6172 6773 da06 6461 656d 6f6e 4e29 0e72  args..daemonN).r
-00001350: 2000 0000 7221 0000 0072 1f00 0000 da05   ...r!...r......
-00001360: 6d6b 6469 72da 0670 6172 656e 74da 0473  mkdir..parent..s
-00001370: 7465 6d72 0400 0000 da06 7368 7574 696c  temr......shutil
-00001380: da05 636f 7079 3272 1300 0000 7206 0000  ..copy2r....r...
-00001390: 0072 5500 0000 5a10 7265 636f 7264 696e  .rU...Z.recordin
-000013a0: 675f 7468 7265 6164 da05 7374 6172 7429  g_thread..start)
-000013b0: 0772 1600 0000 721f 0000 0072 2e00 0000  .r....r....r....
-000013c0: 722f 0000 0072 3000 0000 5a12 736f 7572  r/...r0...Z.sour
-000013d0: 6365 5f63 6f6e 6669 675f 7061 7468 5a15  ce_config_pathZ.
-000013e0: 6475 706c 6963 6174 655f 636f 6e66 6967  duplicate_config
-000013f0: 5f70 6174 6872 1900 0000 7219 0000 0072  _pathr....r....r
-00001400: 1a00 0000 da0f 7374 6172 745f 7265 636f  ......start_reco
-00001410: 7264 696e 67a8 0000 0073 1a00 0000 100f  rding....s......
-00001420: 0602 1002 0e04 1201 0e02 0c02 0c02 0602  ................
-00001430: 0201 0e01 08ff 0e03 7a1d 5669 6465 6f52  ........z.VideoR
-00001440: 6563 6f72 6465 722e 7374 6172 745f 7265  ecorder.start_re
-00001450: 636f 7264 696e 6763 0100 0000 0000 0000  cordingc........
-00001460: 0000 0000 0100 0000 0300 0000 4300 0000  ............C...
-00001470: 7318 0000 0074 00a0 0164 01a1 0101 007c  s....t...d.....|
-00001480: 006a 02a0 03a1 0001 0064 0053 0029 024e  .j.......d.S.).N
-00001490: 7a2d 5374 6f70 2072 6563 6f72 6469 6e67  z-Stop recording
-000014a0: 2069 6e69 7469 6174 6564 2077 6974 6869   initiated withi
-000014b0: 6e20 5669 6465 6f52 6563 6f72 6465 7229  n VideoRecorder)
-000014c0: 0472 2000 0000 7221 0000 0072 1500 0000  .r ...r!...r....
-000014d0: da03 7365 7472 6000 0000 7219 0000 0072  ..setr`...r....r
-000014e0: 1900 0000 721a 0000 00da 0e73 746f 705f  ....r......stop_
-000014f0: 7265 636f 7264 696e 67ce 0000 0073 0400  recording....s..
-00001500: 0000 0a01 0e01 7a1c 5669 6465 6f52 6563  ......z.VideoRec
-00001510: 6f72 6465 722e 7374 6f70 5f72 6563 6f72  order.stop_recor
-00001520: 6469 6e67 725f 0000 0029 0354 4654 2913  dingr_...).TFT).
-00001530: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
-00001540: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
-00001550: 6d65 5f5f 7203 0000 0072 4900 0000 724f  me__r....rI...rO
-00001560: 0000 0072 0800 0000 721e 0000 0072 1200  ...r....r....r..
-00001570: 0000 722d 0000 00da 0462 6f6f 6c72 5500  ..r-.....boolrU.
-00001580: 0000 7230 0000 0072 4d00 0000 7261 0000  ..r0...rM...ra..
-00001590: 0072 0400 0000 726e 0000 0072 7000 0000  .r....rn...rp...
-000015a0: da0d 5f5f 636c 6173 7363 656c 6c5f 5f72  ..__classcell__r
-000015b0: 1900 0000 7219 0000 0072 1700 0000 721a  ....r....r....r.
-000015c0: 0000 0072 0c00 0000 1300 0000 7320 0000  ...r........s ..
-000015d0: 0008 0006 0106 0118 0208 1016 1008 6208  ..............b.
-000015e0: 0608 0602 0602 0102 0104 fb02 020a fe10  ................
-000015f0: 2672 0c00 0000 291c da0d 7079 7879 3364  &r....)...pyxy3d
-00001600: 2e6c 6f67 6765 72da 0670 7978 7933 6472  .logger..pyxy3dr
-00001610: 2000 0000 723f 0000 0072 7100 0000 da0c   ...r?...rq.....
-00001620: 5079 5174 362e 5174 436f 7265 7202 0000  PyQt6.QtCorer...
-00001630: 0072 0300 0000 da07 7061 7468 6c69 6272  .r......pathlibr
-00001640: 0400 0000 da05 7175 6575 6572 0500 0000  ......queuer....
-00001650: da09 7468 7265 6164 696e 6772 0600 0000  ..threadingr....
-00001660: 7207 0000 0072 2200 0000 da03 7379 73da  r....r".....sys.
-00001670: 0670 616e 6461 7372 5a00 0000 726b 0000  .pandasrZ...rk..
-00001680: 00da 1b70 7978 7933 642e 6361 6d65 7261  ...pyxy3d.camera
-00001690: 732e 7379 6e63 6872 6f6e 697a 6572 7208  s.synchronizerr.
-000016a0: 0000 00da 1a70 7978 7933 642e 6361 6d65  .....pyxy3d.came
-000016b0: 7261 732e 6c69 7665 5f73 7472 6561 6d72  ras.live_streamr
-000016c0: 0900 0000 da10 7079 7879 3364 2e69 6e74  ......pyxy3d.int
-000016d0: 6572 6661 6365 720a 0000 0072 0b00 0000  erfacer....r....
-000016e0: 720c 0000 0072 1900 0000 7219 0000 0072  r....r....r....r
-000016f0: 1900 0000 721a 0000 00da 083c 6d6f 6475  ....r......<modu
-00001700: 6c65 3e01 0000 0073 1c00 0000 0800 0c02  le>....s........
-00001710: 1002 0c01 0c01 1001 0801 0801 0801 0801  ................
-00001720: 0c02 0c01 1001 1403                      ........
+00000040: 5a02 6400 6402 6c05 6d06 5a06 0100 6400  Z.d.d.l.m.Z...d.
+00000050: 6403 6c07 6d08 5a08 0100 6400 6404 6c09  d.l.m.Z...d.d.l.
+00000060: 6d0a 5a0a 6d0b 5a0b 0100 6400 6401 6c0c  m.Z.m.Z...d.d.l.
+00000070: 5a0c 6400 6401 6c0d 5a0d 6400 6401 6c0e  Z.d.d.l.Z.d.d.l.
+00000080: 5a0f 6400 6401 6c10 5a10 6400 6405 6c11  Z.d.d.l.Z.d.d.l.
+00000090: 6d12 5a12 0100 6400 6406 6c13 6d14 5a14  m.Z...d.d.l.m.Z.
+000000a0: 0100 6400 6407 6c15 6d16 5a16 6d17 5a17  ..d.d.l.m.Z.m.Z.
+000000b0: 0100 4700 6408 6409 8400 6409 8302 5a18  ..G.d.d...d...Z.
+000000c0: 6401 5300 290a e900 0000 004e 2901 da04  d.S.)......N)...
+000000d0: 5061 7468 2901 da05 5175 6575 6529 02da  Path)...Queue)..
+000000e0: 0654 6872 6561 64da 0545 7665 6e74 2901  .Thread..Event).
+000000f0: da0c 5379 6e63 6872 6f6e 697a 6572 2901  ..Synchronizer).
+00000100: da0a 4c69 7665 5374 7265 616d 2902 da0b  ..LiveStream)...
+00000110: 4672 616d 6550 6163 6b65 74da 0a53 796e  FramePacket..Syn
+00000120: 6350 6163 6b65 7463 0000 0000 0000 0000  cPacketc........
+00000130: 0000 0000 0000 0000 0600 0000 0000 0000  ................
+00000140: 737c 0000 0065 005a 0164 005a 0264 1a64  s|...e.Z.d.Z.d.d
+00000150: 0265 0364 0365 0466 0487 0066 0164 0464  .e.d.e.f...f.d.d
+00000160: 0584 0d5a 0564 0664 0784 005a 0664 0865  ...Z.d.d...Z.d.e
+00000170: 0764 0965 0764 0a65 0766 0664 0b64 0c84  .d.e.d.e.f.d.d..
+00000180: 045a 0864 0d64 0e84 005a 0964 0f64 1084  .Z.d.d...Z.d.d..
+00000190: 005a 0a64 1164 1284 005a 0b09 1309 1409  .Z.d.d...Z......
+000001a0: 1364 1b64 1565 0c66 0264 1664 1784 055a  .d.d.e.f.d.d...Z
+000001b0: 0d64 1864 1984 005a 0e87 0004 005a 0f53  .d.d...Z.....Z.S
+000001c0: 0029 1cda 0d56 6964 656f 5265 636f 7264  .)...VideoRecord
+000001d0: 6572 4eda 0c73 796e 6368 726f 6e69 7a65  erN..synchronize
+000001e0: 72da 0673 7566 6669 7863 0300 0000 0000  r..suffixc......
+000001f0: 0000 0000 0000 0300 0000 0200 0000 0300  ................
+00000200: 0000 734c 0000 0074 0083 00a0 01a1 0001  ..sL...t........
+00000210: 007c 017c 005f 027c 0264 0075 0172 1264  .|.|._.|.d.u.r.d
+00000220: 017c 0217 007c 005f 036e 0364 027c 005f  .|...|._.n.d.|._
+00000230: 0364 037c 005f 0464 047c 005f 0574 0683  .d.|._.d.|._.t..
+00000240: 007c 005f 0774 0864 0583 017c 005f 0964  .|._.t.d...|._.d
+00000250: 0053 0029 064e da01 5fda 0046 7201 0000  .S.).N.._..Fr...
+00000260: 00e9 ffff ffff 290a da05 7375 7065 72da  ......)...super.
+00000270: 085f 5f69 6e69 745f 5f72 0b00 0000 720c  .__init__r....r.
+00000280: 0000 00da 0972 6563 6f72 6469 6e67 da0a  .....recording..
+00000290: 7379 6e63 5f69 6e64 6578 7205 0000 00da  sync_indexr.....
+000002a0: 0c74 7269 6767 6572 5f73 746f 7072 0300  .trigger_stopr..
+000002b0: 0000 da10 7379 6e63 5f70 6163 6b65 745f  ....sync_packet_
+000002c0: 696e 5f71 2903 da04 7365 6c66 720b 0000  in_q)...selfr...
+000002d0: 0072 0c00 0000 a901 da09 5f5f 636c 6173  .r........__clas
+000002e0: 735f 5fa9 00fa 4343 3a5c 5573 6572 735c  s__...CC:\Users\
+000002f0: 4d61 6320 5072 6962 6c65 5c72 6570 6f73  Mac Prible\repos
+00000300: 5c70 7978 7933 645c 7079 7879 3364 5c72  \pyxy3d\pyxy3d\r
+00000310: 6563 6f72 6469 6e67 5c76 6964 656f 5f72  ecording\video_r
+00000320: 6563 6f72 6465 722e 7079 7211 0000 0015  ecorder.pyr.....
+00000330: 0000 0073 1200 0000 0a01 0601 0804 0c01  ...s............
+00000340: 0602 0602 0601 0802 0e02 7a16 5669 6465  ..........z.Vide
+00000350: 6f52 6563 6f72 6465 722e 5f5f 696e 6974  oRecorder.__init
+00000360: 5f5f 6301 0000 0000 0000 0000 0000 0007  __c.............
+00000370: 0000 0008 0000 0043 0000 0073 8200 0000  .......C...s....
+00000380: 6900 7c00 5f00 7c00 6a01 6a02 a003 a100  i.|._.|.j.j.....
+00000390: 4400 5d35 5c02 7d01 7d02 7404 7405 7c00  D.]5\.}.}.t.t.|.
+000003a0: 6a06 6401 7c01 9b00 7c00 6a07 9b00 6402  j.d.|...|.j...d.
+000003b0: 9d04 8302 8301 7d03 7408 a009 6403 7c01  ......}.t...d.|.
+000003c0: 9b00 6404 7c03 9b00 9d04 a101 0100 740a  ..d.|.........t.
+000003d0: 6a0b 6405 8e00 7d04 7c02 6a0c 6a0d 7d05  j.d...}.|.j.j.}.
+000003e0: 740a a00e 7c03 7c04 7c02 6a0f 7c05 a104  t...|.|.|.j.|...
+000003f0: 7d06 7c06 7c00 6a00 7c01 3c00 7109 6406  }.|.|.j.|.<.q.d.
+00000400: 5300 2907 7aba 0a20 2020 2020 2020 2073  S.).z..        s
+00000410: 7566 6669 7820 7072 6f76 6964 6573 2061  uffix provides a
+00000420: 2077 6179 2074 6f20 7072 6f76 6964 6520   way to provide 
+00000430: 6164 6469 7469 6f6e 616c 206c 6162 656c  additional label
+00000440: 7320 746f 2074 6865 206d 7034 2066 696c  s to the mp4 fil
+00000450: 6520 6e61 6d65 0a20 2020 2020 2020 2054  e name.        T
+00000460: 6869 7320 776f 756c 6420 6265 2072 656c  his would be rel
+00000470: 6576 616e 7420 7768 656e 2070 6572 666f  evant when perfo
+00000480: 726d 696e 6720 706f 7374 2d70 726f 6365  rming post-proce
+00000490: 7373 696e 6720 616e 6420 7361 7669 6e67  ssing and saving
+000004a0: 206f 7574 2066 7261 6d65 7320 7769 7468   out frames with
+000004b0: 2070 6f69 6e74 730a 2020 2020 2020 2020   points.        
+000004c0: 5a05 706f 7274 5f7a 042e 6d70 347a 1f42  Z.port_z..mp4z.B
+000004d0: 7569 6c64 696e 6720 7669 6465 6f20 7772  uilding video wr
+000004e0: 6974 6572 2066 6f72 2070 6f72 7420 7a0f  iter for port z.
+000004f0: 3b20 7265 636f 7264 696e 6720 746f 205a  ; recording to Z
+00000500: 044d 5034 564e 2910 da0d 7669 6465 6f5f  .MP4VN)...video_
+00000510: 7772 6974 6572 7372 0b00 0000 da07 7374  writersr......st
+00000520: 7265 616d 73da 0569 7465 6d73 da03 7374  reams..items..st
+00000530: 7272 0200 0000 da12 6465 7374 696e 6174  rr......destinat
+00000540: 696f 6e5f 666f 6c64 6572 720c 0000 00da  ion_folderr.....
+00000550: 066c 6f67 6765 72da 0469 6e66 6fda 0363  .logger..info..c
+00000560: 7632 da12 5669 6465 6f57 7269 7465 725f  v2..VideoWriter_
+00000570: 666f 7572 6363 da06 6361 6d65 7261 da04  fourcc..camera..
+00000580: 7369 7a65 da0b 5669 6465 6f57 7269 7465  size..VideoWrite
+00000590: 72da 0366 7073 2907 7216 0000 00da 0470  r..fps).r......p
+000005a0: 6f72 74da 0673 7472 6561 6dda 0470 6174  ort..stream..pat
+000005b0: 685a 0666 6f75 7263 63da 0a66 7261 6d65  hZ.fourcc..frame
+000005c0: 5f73 697a 65da 0677 7269 7465 7272 1900  _size..writerr..
+000005d0: 0000 7219 0000 0072 1a00 0000 da13 6275  ..r....r......bu
+000005e0: 696c 645f 7669 6465 6f5f 7772 6974 6572  ild_video_writer
+000005f0: 7327 0000 0073 1200 0000 0606 1401 1e01  s'...s..........
+00000600: 1601 0a01 0801 1202 0c01 04f9 7a21 5669  ............z!Vi
+00000610: 6465 6f52 6563 6f72 6465 722e 6275 696c  deoRecorder.buil
+00000620: 645f 7669 6465 6f5f 7772 6974 6572 73da  d_video_writers.
+00000630: 0d69 6e63 6c75 6465 5f76 6964 656f da0b  .include_video..
+00000640: 7368 6f77 5f70 6f69 6e74 73da 1373 746f  show_points..sto
+00000650: 7265 5f70 6f69 6e74 5f68 6973 746f 7279  re_point_history
+00000660: 6304 0000 0000 0000 0000 0000 000f 0000  c...............
+00000670: 000a 0000 0043 0000 0073 7402 0000 7c01  .....C...st...|.
+00000680: 7206 7c00 a000 a100 0100 6700 6700 6700  r.|.......g.g.g.
+00000690: 6700 6401 9c04 7c00 5f01 6700 6700 6700  g.d...|._.g.g.g.
+000006a0: 6700 6700 6700 6700 6700 6700 6402 9c09  g.g.g.g.g.g.d...
+000006b0: 7c00 5f02 7c00 6a03 a004 7c00 6a05 a101  |._.|.j...|.j...
+000006c0: 0100 6403 7d04 7406 a007 6404 a101 0100  ..d.}.t...d.....
+000006d0: 7c00 6a05 a008 a100 6405 6b04 7335 7c00  |.j.....d.k.s5|.
+000006e0: 6a09 a00a a100 73ff 7c00 6a05 a00b a100  j.....s.|.j.....
+000006f0: 7d05 7406 a007 6406 a101 0100 7c00 6a05  }.t...d.....|.j.
+00000700: a008 a100 7d06 7c06 6407 1600 6405 6b02  ....}.|.d...d.k.
+00000710: 7259 7c06 6405 6b03 7259 7406 a007 6408  rY|.d.k.rYt...d.
+00000720: 7c00 6a05 a008 a100 9b00 9d02 a101 0100  |.j.............
+00000730: 7c05 6400 7500 7263 7406 a007 6409 a101  |.d.u.rct...d...
+00000740: 0100 6e9c 7c05 6a0c 7c00 5f0c 7c05 6a0d  ..n.|.j.|._.|.j.
+00000750: a00e a100 4400 5d71 5c02 7d07 7d08 7c08  ....D.]q\.}.}.|.
+00000760: 6400 7501 72dd 7406 a007 640a a101 0100  d.u.r.t...d.....
+00000770: 7c02 727f 7c08 6a0f 7d09 6e03 7c08 6a10  |.r.|.j.}.n.|.j.
+00000780: 7d09 7c08 6a11 7d0a 7c08 6a12 7d0b 7c01  }.|.j.}.|.j.}.|.
+00000790: 72b8 7406 a007 640b a101 0100 7c00 6a13  r.t...d.....|.j.
+000007a0: 7c07 1900 a014 7c09 a101 0100 7c00 6a01  |.....|.....|.j.
+000007b0: 640c 1900 a015 7c00 6a0c a101 0100 7c00  d.....|.j.....|.
+000007c0: 6a01 640d 1900 a015 7c07 a101 0100 7c00  j.d.....|.....|.
+000007d0: 6a01 640e 1900 a015 7c0a a101 0100 7c00  j.d.....|.....|.
+000007e0: 6a01 640f 1900 a015 7c0b a101 0100 7c08  j.d.....|.....|.
+000007f0: a016 7c00 6a0c a101 7d0c 7c0c 6400 7501  ..|.j...}.|.d.u.
+00000800: 72dd 7c00 6a02 a017 a100 a00e a100 4400  r.|.j.........D.
+00000810: 5d13 5c02 7d0d 7d0e 7406 a007 6410 a101  ].\.}.}.t...d...
+00000820: 0100 7c00 6a02 7c0d 1900 a018 7c0c 7c0d  ..|.j.|.....|.|.
+00000830: 1900 a101 0100 71c9 716c 7c04 73f3 7c00  ......q.ql|.s.|.
+00000840: 6a09 a00a a100 72f3 7406 a007 6411 a101  j.....r.t...d...
+00000850: 0100 6412 7d04 7c00 6a03 a019 7c00 6a05  ..d.}.|.j...|.j.
+00000860: a101 0100 7c00 6a05 a008 a100 6405 6b04  ....|.j.....d.k.
+00000870: 7335 7c00 6a09 a00a a100 7235 7c01 9001  s5|.j.....r5|...
+00000880: 721f 7406 a007 6413 a101 0100 7c00 6a03  r.t...d.....|.j.
+00000890: 6a1a 4400 5d0a 7d07 7c00 6a13 7c07 1900  j.D.].}.|.j.|...
+000008a0: a01b a100 0100 9001 710b 7406 a007 6414  ........q.t...d.
+000008b0: a101 0100 7c00 a01c a100 0100 7406 a007  ....|.......t...
+000008c0: 6415 a101 0100 7c03 9001 722b 7c00 a01d  d.....|...r+|...
+000008d0: a100 0100 7c00 6a09 a01e a100 0100 6403  ....|.j.......d.
+000008e0: 7c00 5f1f 7406 a007 6416 a101 0100 6400  |._.t...d.....d.
+000008f0: 5300 2917 4e29 0472 1300 0000 7228 0000  S.).N).r....r(..
+00000900: 00da 0b66 7261 6d65 5f69 6e64 6578 da0a  ...frame_index..
+00000910: 6672 616d 655f 7469 6d65 2909 7213 0000  frame_time).r...
+00000920: 0072 2800 0000 7231 0000 0072 3200 0000  .r(...r1...r2...
+00000930: da08 706f 696e 745f 6964 da09 696d 675f  ..point_id..img_
+00000940: 6c6f 635f 78da 0969 6d67 5f6c 6f63 5f79  loc_x..img_loc_y
+00000950: da09 6f62 6a5f 6c6f 635f 78da 096f 626a  ..obj_loc_x..obj
+00000960: 5f6c 6f63 5f79 467a 2645 6e74 6572 696e  _loc_yFz&Enterin
+00000970: 6720 5361 7665 2064 6174 6120 776f 726b  g Save data work
+00000980: 6572 206c 6f6f 7020 656e 7465 7265 6472  er loop enteredr
+00000990: 0100 0000 7a1e 4765 7474 696e 6720 7369  ....z.Getting si
+000009a0: 647a 6520 6f66 2073 796e 6320 7061 636b  dze of sync pack
+000009b0: 6574 2071 e919 0000 007a 3153 697a 6520  et q.....z1Size 
+000009c0: 6f66 2075 6e73 6176 6564 2066 7261 6d65  of unsaved frame
+000009d0: 7320 6f6e 2074 6865 2072 6563 6f72 6469  s on the recordi
+000009e0: 6e67 2071 7565 7565 2069 7320 7a33 456e  ng queue is z3En
+000009f0: 6420 6f66 2073 796e 6320 7061 636b 6574  d of sync packet
+00000a00: 7320 7369 676e 616c 6564 2e2e 2e62 7265  s signaled...bre
+00000a10: 616b 696e 6720 7265 636f 7264 206c 6f6f  aking record loo
+00000a20: 707a 1b50 726f 6365 7373 696f 6e67 2066  pz.Processiong f
+00000a30: 7261 6d65 2070 6163 6b65 742e 2e2e 7a0d  rame packet...z.
+00000a40: 5772 6974 696e 6720 6672 616d 6572 1300  Writing framer..
+00000a50: 0000 7228 0000 0072 3100 0000 7232 0000  ..r(...r1...r2..
+00000a60: 007a 2545 7874 656e 6469 6e67 2074 6964  .z%Extending tid
+00000a70: 7920 7461 626c 6520 6f66 2070 6f69 6e74  y table of point
+00000a80: 2068 6973 746f 7279 7a21 5361 7665 2066   historyz!Save f
+00000a90: 7261 6d65 2077 6f72 6b65 7220 7769 6e64  rame worker wind
+00000aa0: 696e 6720 646f 776e 2e2e 2e54 7a1a 7265  ing down...Tz.re
+00000ab0: 6c65 6173 696e 6720 7669 6465 6f20 7772  leasing video wr
+00000ac0: 6974 6572 732e 2e2e 7a21 496e 6974 6961  iters...z!Initia
+00000ad0: 7465 2073 746f 7269 6e67 206f 6620 6672  te storing of fr
+00000ae0: 616d 6520 6869 7374 6f72 797a 2149 6e69  ame historyz!Ini
+00000af0: 7469 6174 6520 7374 6f72 696e 6720 6f66  tiate storing of
+00000b00: 2070 6f69 6e74 2068 6973 746f 7279 7a27   point historyz'
+00000b10: 4162 6f75 7420 746f 2065 6d69 7420 6061  About to emit `a
+00000b20: 6c6c 2066 7261 6d65 7320 7361 7665 6460  ll frames saved`
+00000b30: 2073 6967 6e61 6c29 2072 2d00 0000 da0d   signal) r-.....
+00000b40: 6672 616d 655f 6869 7374 6f72 79da 1270  frame_history..p
+00000b50: 6f69 6e74 5f64 6174 615f 6869 7374 6f72  oint_data_histor
+00000b60: 7972 0b00 0000 da19 7375 6273 6372 6962  yr......subscrib
+00000b70: 655f 746f 5f73 796e 635f 7061 636b 6574  e_to_sync_packet
+00000b80: 7372 1500 0000 7220 0000 0072 2100 0000  sr....r ...r!...
+00000b90: da05 7173 697a 6572 1400 0000 da06 6973  ..qsizer......is
+00000ba0: 5f73 6574 da03 6765 7472 1300 0000 da0d  _set..getr......
+00000bb0: 6672 616d 655f 7061 636b 6574 7372 1d00  frame_packetsr..
+00000bc0: 0000 da11 6672 616d 655f 7769 7468 5f70  ....frame_with_p
+00000bd0: 6f69 6e74 73da 0566 7261 6d65 7231 0000  oints..framer1..
+00000be0: 0072 3200 0000 721b 0000 00da 0577 7269  .r2...r......wri
+00000bf0: 7465 da06 6170 7065 6e64 da0d 746f 5f74  te..append..to_t
+00000c00: 6964 795f 7461 626c 65da 0463 6f70 79da  idy_table..copy.
+00000c10: 0665 7874 656e 64da 1572 656c 6561 7365  .extend..release
+00000c20: 5f73 796e 635f 7061 636b 6574 5f71 da05  _sync_packet_q..
+00000c30: 706f 7274 73da 0772 656c 6561 7365 da13  ports..release..
+00000c40: 7374 6f72 655f 6672 616d 655f 6869 7374  store_frame_hist
+00000c50: 6f72 7972 3000 0000 da05 636c 6561 7272  oryr0.....clearr
+00000c60: 1200 0000 290f 7216 0000 0072 2e00 0000  ....).r....r....
+00000c70: 722f 0000 0072 3000 0000 5a21 7379 6e63  r/...r0...Z!sync
+00000c80: 726f 6e69 7a65 725f 7375 6273 6372 6970  ronizer_subscrip
+00000c90: 7469 6f6e 5f72 656c 6561 7365 64da 0b73  tion_released..s
+00000ca0: 796e 635f 7061 636b 6574 da07 6261 636b  ync_packet..back
+00000cb0: 6c6f 6772 2800 0000 da0c 6672 616d 655f  logr(.....frame_
+00000cc0: 7061 636b 6574 7241 0000 0072 3100 0000  packetrA...r1...
+00000cd0: 7232 0000 005a 0e6e 6577 5f74 6964 795f  r2...Z.new_tidy_
+00000ce0: 7461 626c 65da 036b 6579 da05 7661 6c75  table..key..valu
+00000cf0: 6572 1900 0000 7219 0000 0072 1a00 0000  er....r....r....
+00000d00: da10 7361 7665 5f64 6174 615f 776f 726b  ..save_data_work
+00000d10: 6572 3700 0000 7388 0000 0004 0208 0102  er7...s.........
+00000d20: 0402 0102 0102 0108 fc02 0802 0102 0102  ................
+00000d30: 0102 0102 0102 0102 0102 0108 f70e 0d04  ................
+00000d40: 010a 0318 010a 010a 030a 0114 0116 0108  ................
+00000d50: 020a 0202 0108 0212 0208 010a 0104 0208  ................
+00000d60: 0106 0206 0206 0104 020a 0210 0112 0310  ................
+00000d70: 0110 0110 010c 0208 0116 010a 0116 0102  ................
+00000d80: 800e 020a 0104 010e 0118 d006 350a 010c  ............5...
+00000d90: 0112 010a 0408 010a 0206 0108 010a 0106  ................
+00000da0: 010e 017a 1e56 6964 656f 5265 636f 7264  ...z.VideoRecord
+00000db0: 6572 2e73 6176 655f 6461 7461 5f77 6f72  er.save_data_wor
+00000dc0: 6b65 7263 0100 0000 0000 0000 0000 0000  kerc............
+00000dd0: 0300 0000 0600 0000 4300 0000 734a 0000  ........C...sJ..
+00000de0: 0074 00a0 017c 006a 02a1 017d 0174 0374  .t...|.j...}.t.t
+00000df0: 047c 006a 0564 017c 006a 069b 0064 029d  .|.j.d.|.j...d..
+00000e00: 0383 0283 017d 0274 07a0 0864 037c 029b  .....}.t...d.|..
+00000e10: 009d 02a1 0101 007c 016a 097c 0264 0464  .......|.j.|.d.d
+00000e20: 0564 068d 0301 0064 0053 0029 074e da02  .d.....d.S.).N..
+00000e30: 7879 7a04 2e63 7376 7a16 5374 6f72 696e  xyz..csvz.Storin
+00000e40: 6720 706f 696e 7420 6461 7461 2069 6e20  g point data in 
+00000e50: 4654 a902 da05 696e 6465 78da 0668 6561  FT....index..hea
+00000e60: 6465 7229 0ada 0270 64da 0944 6174 6146  der)...pd..DataF
+00000e70: 7261 6d65 723a 0000 0072 1e00 0000 7202  ramer:...r....r.
+00000e80: 0000 0072 1f00 0000 720c 0000 0072 2000  ...r....r....r .
+00000e90: 0000 7221 0000 00da 0674 6f5f 6373 7629  ..r!.....to_csv)
+00000ea0: 0372 1600 0000 da02 6466 da0f 706f 696e  .r......df..poin
+00000eb0: 745f 6461 7461 5f70 6174 6872 1900 0000  t_data_pathr....
+00000ec0: 7219 0000 0072 1a00 0000 7230 0000 009e  r....r....r0....
+00000ed0: 0000 0073 0800 0000 0c01 1a01 1001 1401  ...s............
+00000ee0: 7a21 5669 6465 6f52 6563 6f72 6465 722e  z!VideoRecorder.
+00000ef0: 7374 6f72 655f 706f 696e 745f 6869 7374  store_point_hist
+00000f00: 6f72 7963 0100 0000 0000 0000 0000 0000  oryc............
+00000f10: 0300 0000 0500 0000 4300 0000 7340 0000  ........C...s@..
+00000f20: 0074 00a0 017c 006a 02a1 017d 0174 0374  .t...|.j...}.t.t
+00000f30: 047c 006a 0564 0183 0283 017d 0274 06a0  .|.j.d.....}.t..
+00000f40: 0764 027c 029b 009d 02a1 0101 007c 016a  .d.|.........|.j
+00000f50: 087c 0264 0364 0464 058d 0301 0064 0053  .|.d.d.d.....d.S
+00000f60: 0029 064e 7a16 6672 616d 655f 7469 6d65  .).Nz.frame_time
+00000f70: 5f68 6973 746f 7279 2e63 7376 7a19 5374  _history.csvz.St
+00000f80: 6f72 696e 6720 6672 616d 6520 6869 7374  oring frame hist
+00000f90: 6f72 7920 746f 2046 5472 5300 0000 2909  ory to FTrS...).
+00000fa0: 7256 0000 0072 5700 0000 7239 0000 0072  rV...rW...r9...r
+00000fb0: 1e00 0000 7202 0000 0072 1f00 0000 7220  ....r....r....r 
+00000fc0: 0000 0072 2100 0000 7258 0000 0029 0372  ...r!...rX...).r
+00000fd0: 1600 0000 7259 0000 005a 0f66 7261 6d65  ....rY...Z.frame
+00000fe0: 5f68 6973 745f 7061 7468 7219 0000 0072  _hist_pathr....r
+00000ff0: 1900 0000 721a 0000 0072 4a00 0000 a400  ....r....rJ.....
+00001000: 0000 7308 0000 000c 0110 0110 0114 017a  ..s............z
+00001010: 2156 6964 656f 5265 636f 7264 6572 2e73  !VideoRecorder.s
+00001020: 746f 7265 5f66 7261 6d65 5f68 6973 746f  tore_frame_histo
+00001030: 7279 6301 0000 0000 0000 0000 0000 0001  ryc.............
+00001040: 0000 0001 0000 0043 0000 0073 0400 0000  .......C...s....
+00001050: 6400 5300 a901 4e72 1900 0000 a901 7216  d.S...Nr......r.
+00001060: 0000 0072 1900 0000 7219 0000 0072 1a00  ...r....r....r..
+00001070: 0000 da13 7374 6f72 655f 6163 7469 7665  ....store_active
+00001080: 5f63 6f6e 6669 67aa 0000 0073 0200 0000  _config....s....
+00001090: 0401 7a21 5669 6465 6f52 6563 6f72 6465  ..z!VideoRecorde
+000010a0: 722e 7374 6f72 655f 6163 7469 7665 5f63  r.store_active_c
+000010b0: 6f6e 6669 6754 4672 1f00 0000 6305 0000  onfigTFr....c...
+000010c0: 0000 0000 0000 0000 0007 0000 0005 0000  ................
+000010d0: 0043 0000 0073 9800 0000 7400 a001 6401  .C...s....t...d.
+000010e0: 7c01 9b00 9d02 a101 0100 7c01 7c00 5f02  |.........|.|._.
+000010f0: 7c00 6a02 6a03 6402 6402 6403 8d02 0100  |.j.j.d.d.d.....
+00001100: 7c00 6a02 6a04 6a05 6404 6b02 7223 7406  |.j.j.j.d.k.r#t.
+00001110: 7c00 6a02 6a04 6a04 6405 8302 7d05 6e07  |.j.j.j.d...}.n.
+00001120: 7406 7c00 6a02 6a04 6405 8302 7d05 7406  t.|.j.j.d...}.t.
+00001130: 7c00 6a02 6405 8302 7d06 7407 a008 7c05  |.j.d...}.t...|.
+00001140: 7c06 a102 0100 6402 7c00 5f09 740a 7c00  |.....d.|._.t.|.
+00001150: 6a0b 7c02 7c03 7c04 6703 6402 6406 8d03  j.|.|.|.g.d.d...
+00001160: 7c00 5f0c 7c00 6a0c a00d a100 0100 6407  |._.|.j.......d.
+00001170: 5300 2908 61f5 0100 000a 2020 2020 2020  S.).a.....      
+00001180: 2020 4f70 7469 6f6e 2065 7869 7374 7320    Option exists 
+00001190: 746f 206e 6f74 2073 746f 7265 2076 6964  to not store vid
+000011a0: 656f 2069 6620 6f6e 6c79 2069 6e74 6572  eo if only inter
+000011b0: 6573 7465 6420 696e 2067 6574 7469 6e67  ested in getting
+000011c0: 2070 6f69 6e74 7320 6672 6f6d 206f 7269   points from ori
+000011d0: 6769 6e61 6c20 7669 6465 6f0a 2020 2020  ginal video.    
+000011e0: 2020 2020 0a20 2020 2020 2020 2050 6172      .        Par
+000011f0: 656e 7420 6f66 2064 6573 7469 6e61 7469  ent of destinati
+00001200: 6f6e 2066 6f6c 6465 7220 7769 6c6c 2062  on folder will b
+00001210: 6520 7468 6520 736f 7572 6365 206f 6620  e the source of 
+00001220: 7468 6520 636f 6e66 6967 2066 696c 6520  the config file 
+00001230: 7468 6174 2077 696c 6c20 6265 2073 746f  that will be sto
+00001240: 7265 6420 7769 7468 2074 6865 2076 6964  red with the vid
+00001250: 656f 0a20 2020 2020 2020 2054 6869 7320  eo.        This 
+00001260: 656e 6162 6c65 7320 7468 6520 6e65 7374  enables the nest
+00001270: 6564 2070 726f 6365 7373 696e 6720 6f66  ed processing of
+00001280: 2076 6964 656f 7320 2869 2e65 2e20 5265   videos (i.e. Re
+00001290: 636f 7264 696e 675f 3120 7769 6c6c 2073  cording_1 will s
+000012a0: 746f 7265 2074 6865 206d 6169 6e20 636f  tore the main co
+000012b0: 6e66 6967 2e74 6f6d 6c2c 0a20 2020 2020  nfig.toml,.     
+000012c0: 2020 2074 6865 6e20 504f 5345 2073 7562     then POSE sub
+000012d0: 666f 6c64 6572 2077 696c 6c20 7374 6f72  folder will stor
+000012e0: 6520 636f 6e66 6967 2e74 6f6d 6c20 6672  e config.toml fr
+000012f0: 6f6d 2052 6563 6f72 6469 6e67 5f31 292e  om Recording_1).
+00001300: 2045 6163 6820 666f 6c64 6572 2073 686f   Each folder sho
+00001310: 756c 6420 6c61 7267 656c 7920 6265 636f  uld largely beco
+00001320: 6d65 2073 656c 660a 2020 2020 2020 2020  me self.        
+00001330: 636f 6e74 6169 6e65 6420 616e 6420 706f  contained and po
+00001340: 7274 6162 6c65 2066 6f72 2061 6e61 6c79  rtable for analy
+00001350: 7369 7320 2f20 7265 636f 6e73 7472 7563  sis / reconstruc
+00001360: 7469 6f6e 2e0a 2020 2020 2020 2020 7a1e  tion..        z.
+00001370: 416c 6c20 7669 6465 6f20 6461 7461 2074  All video data t
+00001380: 6f20 6265 2073 6176 6564 2074 6f20 5429  o be saved to T)
+00001390: 02da 0865 7869 7374 5f6f 6bda 0770 6172  ...exist_ok..par
+000013a0: 656e 7473 da0b 6361 6c69 6272 6174 696f  ents..calibratio
+000013b0: 6e7a 0b63 6f6e 6669 672e 746f 6d6c 2903  nz.config.toml).
+000013c0: da06 7461 7267 6574 da04 6172 6773 da06  ..target..args..
+000013d0: 6461 656d 6f6e 4e29 0e72 2000 0000 7221  daemonN).r ...r!
+000013e0: 0000 0072 1f00 0000 da05 6d6b 6469 72da  ...r......mkdir.
+000013f0: 0670 6172 656e 74da 0473 7465 6d72 0200  .parent..stemr..
+00001400: 0000 da06 7368 7574 696c da05 636f 7079  ....shutil..copy
+00001410: 3272 1200 0000 7204 0000 0072 5100 0000  2r....r....rQ...
+00001420: 5a10 7265 636f 7264 696e 675f 7468 7265  Z.recording_thre
+00001430: 6164 da05 7374 6172 7429 0772 1600 0000  ad..start).r....
+00001440: 721f 0000 0072 2e00 0000 722f 0000 0072  r....r....r/...r
+00001450: 3000 0000 5a12 736f 7572 6365 5f63 6f6e  0...Z.source_con
+00001460: 6669 675f 7061 7468 5a15 6475 706c 6963  fig_pathZ.duplic
+00001470: 6174 655f 636f 6e66 6967 5f70 6174 6872  ate_config_pathr
+00001480: 1900 0000 7219 0000 0072 1a00 0000 da0f  ....r....r......
+00001490: 7374 6172 745f 7265 636f 7264 696e 67ad  start_recording.
+000014a0: 0000 0073 1a00 0000 100f 0602 1002 0e04  ...s............
+000014b0: 1201 0e02 0c02 0c02 0602 0201 0e01 08ff  ................
+000014c0: 0e03 7a1d 5669 6465 6f52 6563 6f72 6465  ..z.VideoRecorde
+000014d0: 722e 7374 6172 745f 7265 636f 7264 696e  r.start_recordin
+000014e0: 6763 0100 0000 0000 0000 0000 0000 0100  gc..............
+000014f0: 0000 0300 0000 4300 0000 7322 0000 0074  ......C...s"...t
+00001500: 00a0 0164 01a1 0101 007c 006a 02a0 03a1  ...d.....|.j....
+00001510: 0001 0074 00a0 0164 02a1 0101 0064 0053  ...t...d.....d.S
+00001520: 0029 034e 7a36 6162 6f75 7420 746f 2053  .).Nz6about to S
+00001530: 746f 7020 7265 636f 7264 696e 6720 696e  top recording in
+00001540: 6974 6961 7465 6420 7769 7468 696e 2056  itiated within V
+00001550: 6964 656f 5265 636f 7264 6572 7a2d 5374  ideoRecorderz-St
+00001560: 6f70 2072 6563 6f72 6469 6e67 2069 6e69  op recording ini
+00001570: 7469 6174 6564 2077 6974 6869 6e20 5669  tiated within Vi
+00001580: 6465 6f52 6563 6f72 6465 7229 0472 2000  deoRecorder).r .
+00001590: 0000 7221 0000 0072 1400 0000 da03 7365  ..r!...r......se
+000015a0: 7472 5c00 0000 7219 0000 0072 1900 0000  tr\...r....r....
+000015b0: 721a 0000 00da 0e73 746f 705f 7265 636f  r......stop_reco
+000015c0: 7264 696e 67d3 0000 0073 0600 0000 0a01  rding....s......
+000015d0: 0a01 0e01 7a1c 5669 6465 6f52 6563 6f72  ....z.VideoRecor
+000015e0: 6465 722e 7374 6f70 5f72 6563 6f72 6469  der.stop_recordi
+000015f0: 6e67 725b 0000 0029 0354 4654 2910 da08  ngr[...).TFT)...
+00001600: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
+00001610: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
+00001620: 5f5f 7206 0000 0072 1e00 0000 7211 0000  __r....r....r...
+00001630: 0072 2d00 0000 da04 626f 6f6c 7251 0000  .r-.....boolrQ..
+00001640: 0072 3000 0000 724a 0000 0072 5d00 0000  .r0...rJ...r]...
+00001650: 7202 0000 0072 6a00 0000 726c 0000 00da  r....rj...rl....
+00001660: 0d5f 5f63 6c61 7373 6365 6c6c 5f5f 7219  .__classcell__r.
+00001670: 0000 0072 1900 0000 7217 0000 0072 1a00  ...r....r....r..
+00001680: 0000 720a 0000 0013 0000 0073 1c00 0000  ..r........s....
+00001690: 0800 1802 0812 1610 0867 0806 0806 0206  .........g......
+000016a0: 0201 0201 04fb 0202 0afe 1026 720a 0000  ...........&r...
+000016b0: 0029 19da 0d70 7978 7933 642e 6c6f 6767  .)...pyxy3d.logg
+000016c0: 6572 da06 7079 7879 3364 7220 0000 0072  er..pyxy3dr ...r
+000016d0: 3e00 0000 726d 0000 00da 0770 6174 686c  >...rm.....pathl
+000016e0: 6962 7202 0000 00da 0571 7565 7565 7203  ibr......queuer.
+000016f0: 0000 00da 0974 6872 6561 6469 6e67 7204  .....threadingr.
+00001700: 0000 0072 0500 0000 7222 0000 00da 0373  ...r....r".....s
+00001710: 7973 da06 7061 6e64 6173 7256 0000 0072  ys..pandasrV...r
+00001720: 6700 0000 da1b 7079 7879 3364 2e63 616d  g.....pyxy3d.cam
+00001730: 6572 6173 2e73 796e 6368 726f 6e69 7a65  eras.synchronize
+00001740: 7272 0600 0000 da1a 7079 7879 3364 2e63  rr......pyxy3d.c
+00001750: 616d 6572 6173 2e6c 6976 655f 7374 7265  ameras.live_stre
+00001760: 616d 7207 0000 00da 1070 7978 7933 642e  amr......pyxy3d.
+00001770: 696e 7465 7266 6163 6572 0800 0000 7209  interfacer....r.
+00001780: 0000 0072 0a00 0000 7219 0000 0072 1900  ...r....r....r..
+00001790: 0000 7219 0000 0072 1a00 0000 da08 3c6d  ..r....r......<m
+000017a0: 6f64 756c 653e 0100 0000 731a 0000 0008  odule>....s.....
+000017b0: 000c 020c 030c 0110 0108 0108 0108 0108  ................
+000017c0: 010c 020c 0110 0112 03                   .........
```

### Comparing `pyxy3d-0.1.3/pyxy3d/recording/__pycache__/video_recorder.cpython-38.pyc` & `pyxy3d-0.1.4/pyxy3d/recording/__pycache__/video_recorder.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/recording/recorded_stream.py` & `pyxy3d-0.1.4/pyxy3d/recording/recorded_stream.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/recording/video_recorder.py` & `pyxy3d-0.1.4/pyxy3d/recording/video_recorder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 import pyxy3d.logger
 
 logger = pyxy3d.logger.get(__name__)
 
-from PyQt6.QtCore import QObject, pyqtSignal
+# from PyQt6.QtCore import QObject, pyqtSignal
 from pathlib import Path
 from queue import Queue
 from threading import Thread, Event
 import cv2
 import sys
 import pandas as pd
 import shutil
 
 from pyxy3d.cameras.synchronizer import Synchronizer
 from pyxy3d.cameras.live_stream import LiveStream
 from pyxy3d.interface import FramePacket, SyncPacket
 
 
-class VideoRecorder(QObject):
-    recording_stop_signal = pyqtSignal()
-    all_frames_saved_signal = pyqtSignal()
+class VideoRecorder:
 
     def __init__(self, synchronizer: Synchronizer, suffix: str = None):
         super().__init__()
         self.synchronizer = synchronizer
 
         # set text to be appended as port_X_{suffix}.mp4
         # will also be appended to xy_{suffix}
@@ -32,14 +30,16 @@
             self.suffix = ""
 
         self.recording = False
         self.sync_index = 0  # no sync packets at init... absence of initialized value can cause errors elsewhere
         # build dict that will be stored to csv
         self.trigger_stop = Event()
 
+        self.sync_packet_in_q = Queue(-1)
+
     def build_video_writers(self):
         """
         suffix provides a way to provide additional labels to the mp4 file name
         This would be relevant when performing post-processing and saving out frames with points
         """
         # create a dictionary of videowriters
         self.video_writers = {}
@@ -50,15 +50,14 @@
             frame_size = stream.camera.size
 
             writer = cv2.VideoWriter(path, fourcc, stream.fps, frame_size)
             self.video_writers[port] = writer
 
     def save_data_worker(self, include_video: bool, show_points: bool, store_point_history:bool):
         # connect video recorder to synchronizer via an "in" queue
-
         if include_video:
             self.build_video_writers()
 
         # I think I put this here so that it will get reset if you reuse the same recorder..
         self.frame_history = {
             "sync_index": [],
             "port": [],
@@ -74,84 +73,90 @@
             "point_id": [],
             "img_loc_x": [],
             "img_loc_y": [],
             "obj_loc_x": [],
             "obj_loc_y": [],
         }
 
-        self.sync_packet_in_q = Queue(-1)
+        
         self.synchronizer.subscribe_to_sync_packets(self.sync_packet_in_q)
         syncronizer_subscription_released = False
         
         # this is where the issue is... need to figure out when the queue is empty...
+        logger.info("Entering Save data worker loop entered")
         while self.sync_packet_in_q.qsize() > 0 or not self.trigger_stop.is_set(): 
             sync_packet: SyncPacket = self.sync_packet_in_q.get()
 
             # provide periodic updates of recording queue
+            logger.info("Getting sidze of sync packet q")
             backlog = self.sync_packet_in_q.qsize()
             if backlog % 25 == 0 and backlog !=0:
                 logger.info(f"Size of unsaved frames on the recording queue is {self.sync_packet_in_q.qsize()}")
 
             if sync_packet is None:
                 # relenvant when 
                 logger.info("End of sync packets signaled...breaking record loop")
                 break
 
             self.sync_index = sync_packet.sync_index
 
             for port, frame_packet in sync_packet.frame_packets.items():
                 if frame_packet is not None:
-                    # logger.info("Processiong frame packet...")
+                    logger.debug("Processiong frame packet...")
                     # read in the data for this frame for this port
                     if show_points:
                         frame = frame_packet.frame_with_points
                     else:
                         frame = frame_packet.frame
 
                     frame_index = frame_packet.frame_index
                     frame_time = frame_packet.frame_time
 
                     if include_video:
                         # store the frame
+                        logger.debug("Writing frame")
                         self.video_writers[port].write(frame)
 
                         # store to assocated data in the dictionary
                         self.frame_history["sync_index"].append(self.sync_index)
                         self.frame_history["port"].append(port)
                         self.frame_history["frame_index"].append(frame_index)
                         self.frame_history["frame_time"].append(frame_time)
 
                     new_tidy_table = frame_packet.to_tidy_table(self.sync_index)
                     if new_tidy_table is not None:  # i.e. it has data
                         for key, value in self.point_data_history.copy().items():
+                            logger.debug("Extending tidy table of point history")
                             self.point_data_history[key].extend(new_tidy_table[key])
                         
             if not syncronizer_subscription_released and self.trigger_stop.is_set():
                 logger.info("Save frame worker winding down...")
                 syncronizer_subscription_released = True
                 self.synchronizer.release_sync_packet_q(self.sync_packet_in_q)
-                self.recording_stop_signal.emit()
+                # self.sync_packet_in_q = Queue(-1)
+                # self.recording_stop_signal.emit()
 
         # a proper release is strictly necessary to ensure file is readable
         if include_video:
             logger.info("releasing video writers...")
             for port in self.synchronizer.ports:
                 self.video_writers[port].release()
 
-            del self.video_writers
+            # del self.video_writers
 
             logger.info("Initiate storing of frame history")
             self.store_frame_history()
 
         logger.info("Initiate storing of point history")
         if store_point_history:
             self.store_point_history()
         self.trigger_stop.clear()  # reset stop recording trigger
         self.recording = False
-        self.all_frames_saved_signal.emit()
+        logger.info("About to emit `all frames saved` signal")
+        # self.all_frames_saved_signal.emit()
 
 
     def store_point_history(self):
         df = pd.DataFrame(self.point_data_history)
         point_data_path = str(Path(self.destination_folder, f"xy{self.suffix}.csv"))
         logger.info(f"Storing point data in {point_data_path}")
         df.to_csv(point_data_path, index=False, header=True)
@@ -200,9 +205,10 @@
         self.recording = True
         self.recording_thread = Thread(
             target=self.save_data_worker, args=[include_video, show_points, store_point_history], daemon=True
         )
         self.recording_thread.start()
 
     def stop_recording(self):
-        logger.info("Stop recording initiated within VideoRecorder")
+        logger.info("about to Stop recording initiated within VideoRecorder")
         self.trigger_stop.set()
+        logger.info("Stop recording initiated within VideoRecorder")
```

### Comparing `pyxy3d-0.1.3/pyxy3d/session/__pycache__/get_stage.cpython-310.pyc` & `pyxy3d-0.1.4/pyxy3d/session/__pycache__/get_stage.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/session/__pycache__/session.cpython-310.pyc` & `pyxy3d-0.1.4/pyxy3d/session/__pycache__/session.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jun 15 18:45:15 2023 UTC, .py size: 21437 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,1019 +1,1040 @@
-00000000: 6f0d 0d0a 0000 0000 3b5c 8b64 bd53 0000  o.......;\.d.S..
+00000000: 6f0d 0d0a 0000 0000 cfda 9564 b954 0000  o..........d.T..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 3801 0000 6400  .....@...s8...d.
-00000030: 6401 6c00 5a01 6501 6a02 a003 6504 a101  d.l.Z.e.j...e...
-00000040: 5a02 6400 6402 6c05 6d06 5a06 6d07 5a07  Z.d.d.l.m.Z.m.Z.
-00000050: 0100 6400 6403 6c08 6d09 5a09 0100 6400  ..d.d.l.m.Z...d.
-00000060: 6404 6c0a 6d0b 5a0b 0100 6400 6405 6c0c  d.l.m.Z...d.d.l.
-00000070: 6d0d 5a0d 0100 6400 6406 6c0e 6d0f 5a0f  m.Z...d.d.l.m.Z.
-00000080: 6d10 5a10 0100 6400 6407 6c11 6d12 5a12  m.Z...d.d.l.m.Z.
-00000090: 0100 6400 6408 6c13 6d14 5a14 0100 6400  ..d.d.l.m.Z...d.
-000000a0: 6409 6c15 6d16 5a16 0100 6400 640a 6c17  d.l.m.Z...d.d.l.
-000000b0: 6d18 5a18 0100 6400 640b 6c19 6d1a 5a1a  m.Z...d.d.l.m.Z.
-000000c0: 0100 6400 640c 6c1b 6d1c 5a1c 0100 6400  ..d.d.l.m.Z...d.
-000000d0: 640d 6c1d 6d1e 5a1e 0100 6400 640e 6c1f  d.l.m.Z...d.d.l.
-000000e0: 6d20 5a20 0100 6400 640f 6c21 6d22 5a22  m Z ..d.d.l!m"Z"
-000000f0: 0100 6400 6410 6c23 6d24 5a24 0100 6400  ..d.d.l#m$Z$..d.
-00000100: 6411 6c25 6d26 5a26 0100 6400 6412 6c27  d.l%m&Z&..d.d.l'
-00000110: 6d28 5a28 0100 6400 6413 6c29 6d2a 5a2a  m(Z(..d.d.l)m*Z*
-00000120: 0100 6400 6414 6c2b 6d2c 5a2c 0100 6400  ..d.d.l+m,Z,..d.
-00000130: 6415 6c2d 6d2e 5a2e 0100 6416 5a2f 6417  d.l-m.Z...d.Z/d.
-00000140: 5a30 4700 6418 6419 8400 6419 650f 8303  Z0G.d.d...d.e...
-00000150: 5a31 4700 641a 641b 8400 641b 6506 8303  Z1G.d.d...d.e...
-00000160: 5a32 6401 5300 291c e900 0000 004e 2902  Z2d.S.)......N).
-00000170: da07 514f 626a 6563 74da 0a70 7971 7453  ..QObject..pyqtS
-00000180: 6967 6e61 6c29 01da 1254 6872 6561 6450  ignal)...ThreadP
-00000190: 6f6f 6c45 7865 6375 746f 7229 01da 0450  oolExecutor)...P
-000001a0: 6174 6829 01da 0573 6c65 6570 2902 da04  ath)...sleep)...
-000001b0: 456e 756d da04 6175 746f 2901 da0e 4368  Enum..auto)...Ch
-000001c0: 6172 7563 6f54 7261 636b 6572 2901 da0e  arucoTracker)...
-000001d0: 4d6f 6e6f 4361 6c69 6272 6174 6f72 2901  MonoCalibrator).
-000001e0: da06 4361 6d65 7261 2901 da0c 5379 6e63  ..Camera)...Sync
-000001f0: 6872 6f6e 697a 6572 2901 da16 4361 6d65  hronizer)...Came
-00000200: 7261 4172 7261 7949 6e69 7469 616c 697a  raArrayInitializ
-00000210: 6572 2901 da07 5472 6163 6b65 7229 01da  er)...Tracker)..
-00000220: 1053 7465 7265 6f43 616c 6962 7261 746f  .StereoCalibrato
-00000230: 7229 01da 0e50 6f69 6e74 4573 7469 6d61  r)...PointEstima
-00000240: 7465 7329 01da 0d43 6170 7475 7265 566f  tes)...CaptureVo
-00000250: 6c75 6d65 2901 da11 5175 616c 6974 7943  lume)...QualityC
-00000260: 6f6e 7472 6f6c 6c65 7229 01da 0b43 616d  ontroller)...Cam
-00000270: 6572 6141 7272 6179 2901 da13 6765 745f  eraArray)...get_
-00000280: 706f 696e 745f 6573 7469 6d61 7465 7329  point_estimates)
-00000290: 01da 0c43 6f6e 6669 6775 7261 746f 7229  ...Configurator)
-000002a0: 01da 0a4c 6976 6553 7472 6561 6d29 01da  ...LiveStream)..
-000002b0: 0d56 6964 656f 5265 636f 7264 6572 e90a  .VideoRecorder..
-000002c0: 0000 0067 9a99 9999 9999 a93f 6300 0000  ...g.......?c...
-000002d0: 0000 0000 0000 0000 0000 0000 0001 0000  ................
-000002e0: 0040 0000 0073 3400 0000 6500 5a01 6400  .@...s4...e.Z.d.
-000002f0: 5a02 6401 5a03 6504 8300 5a05 6504 8300  Z.d.Z.e...Z.e...
-00000300: 5a06 6504 8300 5a07 6504 8300 5a08 6504  Z.e...Z.e...Z.e.
-00000310: 8300 5a09 6504 8300 5a0a 6402 5300 2903  ..Z.e...Z.d.S.).
-00000320: da0b 5365 7373 696f 6e4d 6f64 65fa 0120  ..SessionMode.. 
-00000330: 4e29 0bda 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
-00000340: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
-00000350: 6c6e 616d 655f 5fda 075f 5f64 6f63 5f5f  lname__..__doc__
-00000360: 7208 0000 00da 0743 6861 7275 636f da14  r......Charuco..
-00000370: 496e 7472 696e 7369 6343 616c 6962 7261  IntrinsicCalibra
-00000380: 7469 6f6e da14 4578 7472 696e 7369 6343  tion..ExtrinsicC
-00000390: 616c 6962 7261 7469 6f6e da13 4361 7074  alibration..Capt
-000003a0: 7572 6556 6f6c 756d 654f 7269 6769 6eda  ureVolumeOrigin.
-000003b0: 0952 6563 6f72 6469 6e67 da0e 506f 7374  .Recording..Post
-000003c0: 5072 6f63 6573 7369 6e67 a900 7225 0000  Processing..r%..
-000003d0: 0072 2500 0000 fa3a 433a 5c55 7365 7273  .r%....:C:\Users
-000003e0: 5c4d 6163 2050 7269 626c 655c 7265 706f  \Mac Prible\repo
-000003f0: 735c 7079 7879 3364 5c70 7978 7933 645c  s\pyxy3d\pyxy3d\
-00000400: 7365 7373 696f 6e5c 7365 7373 696f 6e2e  session\session.
-00000410: 7079 7219 0000 0025 0000 0073 1000 0000  pyr....%...s....
-00000420: 0800 0401 0602 0601 0601 0601 0601 0a01  ................
-00000430: 7219 0000 0063 0000 0000 0000 0000 0000  r....c..........
-00000440: 0000 0000 0000 0500 0000 0000 0000 7338  ..............s8
-00000450: 0100 0065 005a 0164 005a 0265 0383 005a  ...e.Z.d.Z.e...Z
-00000460: 0465 0383 005a 0565 0383 005a 0665 0383  .e...Z.e...Z.e..
-00000470: 005a 0765 0365 0883 015a 0964 0165 0a66  .Z.e.e...Z.d.e.f
-00000480: 0287 0066 0164 0264 0384 0c5a 0b64 0464  ...f.d.d...Z.d.d
-00000490: 0584 005a 0c64 0664 0784 005a 0d64 0864  ...Z.d.d...Z.d.d
-000004a0: 0984 005a 0e64 0a64 0b84 005a 0f64 0c64  ...Z.d.d...Z.d.d
-000004b0: 0d84 005a 1064 0e64 0f84 005a 1164 1065  ...Z.d.d...Z.d.e
-000004c0: 0866 0264 1164 1284 045a 1264 1365 1366  .f.d.d...Z.d.e.f
-000004d0: 0264 1464 1584 045a 1464 1665 1366 0264  .d.d...Z.d.e.f.d
-000004e0: 1764 1884 045a 1564 1964 1a84 005a 1664  .d...Z.d.d...Z.d
-000004f0: 1b65 1766 0264 1c64 1d84 045a 1864 1e64  .e.f.d.d...Z.d.d
-00000500: 1f84 005a 1964 2064 2184 005a 1a64 2264  ...Z.d d!..Z.d"d
-00000510: 2384 005a 1b64 2464 2584 005a 1c64 2664  #..Z.d$d%..Z.d&d
-00000520: 2784 005a 1d64 2864 2984 005a 1e64 2a64  '..Z.d(d)..Z.d*d
-00000530: 2b84 005a 1f64 3f64 2d65 1366 0264 2e64  +..Z.d?d-e.f.d.d
-00000540: 2f84 055a 2064 3064 3184 005a 2109 3264  /..Z d0d1..Z!.2d
-00000550: 4064 3365 2264 3465 1766 0464 3564 3684  @d3e"d4e.f.d5d6.
-00000560: 055a 2364 3764 3884 005a 2464 3964 3a84  .Z#d7d8..Z$d9d:.
-00000570: 005a 2564 3b64 3c84 005a 2664 3d64 3e84  .Z%d;d<..Z&d=d>.
-00000580: 005a 2787 0004 005a 2853 0029 41da 0753  .Z'....Z(S.)A..S
-00000590: 6573 7369 6f6e da06 636f 6e66 6967 6302  ession..configc.
-000005a0: 0000 0000 0000 0000 0000 0002 0000 0005  ................
-000005b0: 0000 0003 0000 0073 ba00 0000 7400 7401  .......s....t.t.
-000005c0: 7c00 8302 a002 a100 0100 7c01 7c00 5f03  |.........|.|._.
-000005d0: 7c00 6a03 6a04 7c00 5f05 7406 7c00 6a05  |.j.j.|._.t.|.j.
-000005e0: 6401 6402 6403 8304 7c00 5f07 6900 7c00  d.d.d...|._.i.|.
-000005f0: 5f08 6900 7c00 5f09 6404 7c00 5f0a 6404  _.i.|._.d.|._.d.
-00000600: 7c00 5f0b 6900 7c00 5f0c 6400 7c00 5f0d  |._.i.|._.d.|._.
-00000610: 7c00 6a03 a00e a100 7c00 5f0f 7c00 6a03  |.j.....|._.|.j.
-00000620: a010 a100 7c00 5f11 7c00 6a03 a012 a100  ....|._.|.j.....
-00000630: 7c00 5f13 7c00 6a03 a014 a100 7c00 5f15  |._.|.j.....|._.
-00000640: 7c00 6a03 a016 a100 7c00 5f17 6404 7c00  |.j.....|._.d.|.
-00000650: 5f18 7c00 6a03 a019 a100 7c00 5f1a 741b  _.|.j.....|._.t.
-00000660: 7c00 6a1a 8301 7c00 5f1c 741d 6a1e 7c00  |.j...|._.t.j.|.
-00000670: 5f1f 6400 5300 2905 4e5a 0b63 616c 6962  _.d.S.).NZ.calib
-00000680: 7261 7469 6f6e 5a09 6578 7472 696e 7369  rationZ.extrinsi
-00000690: 637a 0678 792e 6373 7646 2920 da05 7375  cz.xy.csvF) ..su
-000006a0: 7065 7272 2700 0000 da08 5f5f 696e 6974  perr'.....__init
-000006b0: 5f5f 7228 0000 00da 0c73 6573 7369 6f6e  __r(.....session
-000006c0: 5f70 6174 68da 0470 6174 6872 0500 0000  _path..pathr....
-000006d0: da18 6578 7472 696e 7369 635f 6361 6c69  ..extrinsic_cali
-000006e0: 6272 6174 696f 6e5f 7879 da07 6361 6d65  bration_xy..came
-000006f0: 7261 73da 0773 7472 6561 6d73 da17 7374  ras..streams..st
-00000700: 7265 616d 5f74 6f6f 6c73 5f69 6e5f 7072  ream_tools_in_pr
-00000710: 6f63 6573 73da 1373 7472 6561 6d5f 746f  ocess..stream_to
-00000720: 6f6c 735f 6c6f 6164 6564 da0f 6d6f 6e6f  ols_loaded..mono
-00000730: 6361 6c69 6272 6174 6f72 73da 1561 6374  calibrators..act
-00000740: 6976 655f 6d6f 6e6f 6361 6c69 6272 6174  ive_monocalibrat
-00000750: 6f72 5a11 6765 745f 6670 735f 7265 636f  orZ.get_fps_reco
-00000760: 7264 696e 67da 0d66 7073 5f72 6563 6f72  rding..fps_recor
-00000770: 6469 6e67 5a1d 6765 745f 6670 735f 6578  dingZ.get_fps_ex
-00000780: 7472 696e 7369 635f 6361 6c69 6272 6174  trinsic_calibrat
-00000790: 696f 6eda 1966 7073 5f65 7874 7269 6e73  ion..fps_extrins
-000007a0: 6963 5f63 616c 6962 7261 7469 6f6e 5a1d  ic_calibrationZ.
-000007b0: 6765 745f 6670 735f 696e 7472 696e 7369  get_fps_intrinsi
-000007c0: 635f 6361 6c69 6272 6174 696f 6eda 1966  c_calibration..f
-000007d0: 7073 5f69 6e74 7269 6e73 6963 5f63 616c  ps_intrinsic_cal
-000007e0: 6962 7261 7469 6f6e 5a17 6765 745f 6578  ibrationZ.get_ex
-000007f0: 7472 696e 7369 635f 7761 6974 5f74 696d  trinsic_wait_tim
-00000800: 655a 1377 6169 745f 7469 6d65 5f65 7874  eZ.wait_time_ext
-00000810: 7269 6e73 6963 5a17 6765 745f 696e 7472  rinsicZ.get_intr
-00000820: 696e 7369 635f 7761 6974 5f74 696d 655a  insic_wait_timeZ
-00000830: 1377 6169 745f 7469 6d65 5f69 6e74 7269  .wait_time_intri
-00000840: 6e73 6963 da0c 6973 5f72 6563 6f72 6469  nsic..is_recordi
-00000850: 6e67 5a0b 6765 745f 6368 6172 7563 6fda  ngZ.get_charuco.
-00000860: 0763 6861 7275 636f 7209 0000 00da 0f63  .charucor......c
-00000870: 6861 7275 636f 5f74 7261 636b 6572 7219  haruco_trackerr.
-00000880: 0000 0072 1f00 0000 da04 6d6f 6465 2902  ...r......mode).
-00000890: da04 7365 6c66 7228 0000 00a9 01da 095f  ..selfr(......._
-000008a0: 5f63 6c61 7373 5f5f 7225 0000 0072 2600  _class__r%...r&.
-000008b0: 0000 722a 0000 0038 0000 0073 2a00 0000  ..r*...8...s*...
-000008c0: 0e01 0601 0a02 0204 0a01 06ff 0605 0601  ................
-000008d0: 0601 0601 0602 0601 0c03 0c01 0c01 0c01  ................
-000008e0: 0c01 0602 0c02 0c01 0c01 7a10 5365 7373  ..........z.Sess
-000008f0: 696f 6e2e 5f5f 696e 6974 5f5f 6301 0000  ion.__init__c...
-00000900: 0000 0000 0000 0000 0005 0000 0003 0000  ................
-00000910: 0043 0000 0073 8a00 0000 7c00 6a00 a001  .C...s....|.j...
-00000920: a100 4400 5d09 5c02 7d01 7d02 7c02 6a02  ..D.].\.}.}.|.j.
-00000930: a003 a100 0100 7105 6900 7c00 5f00 7c00  ......q.i.|._.|.
-00000940: 6a04 a001 a100 4400 5d08 5c02 7d01 7d03  j.....D.].\.}.}.
-00000950: 7c03 a005 a100 0100 7117 6900 7c00 5f04  |.......q.i.|._.
-00000960: 7c00 6a06 a001 a100 4400 5d09 5c02 7d01  |.j.....D.].\.}.
-00000970: 7d04 7c04 6a02 a003 a100 0100 7128 6900  }.|.j.......q(i.
-00000980: 7c00 5f06 7c00 6a07 6a02 a003 a100 0100  |._.|.j.j.......
-00000990: 6401 7c00 5f07 7c00 6a08 a009 a100 0100  d.|._.|.j.......
-000009a0: 6401 5300 2902 7a72 0a20 2020 2020 2020  d.S.).zr.       
-000009b0: 2053 6875 7420 646f 776e 2074 6865 2073   Shut down the s
-000009c0: 7472 6561 6d73 2c20 636c 6f73 6520 7468  treams, close th
-000009d0: 6520 6361 6d65 7261 2063 6170 7475 7265  e camera capture
-000009e0: 7320 616e 6420 6465 6c65 7465 2074 6865  s and delete the
-000009f0: 206d 6f6e 6f63 616c 6962 7261 746f 7273   monocalibrators
-00000a00: 2061 6e64 2073 796e 6368 726f 6e69 7a65   and synchronize
-00000a10: 720a 2020 2020 2020 2020 4e29 0a72 2f00  r.        N).r/.
-00000a20: 0000 da05 6974 656d 735a 0a73 746f 705f  ....itemsZ.stop_
-00000a30: 6576 656e 74da 0373 6574 722e 0000 00da  event..setr.....
-00000a40: 0a64 6973 636f 6e6e 6563 7472 3200 0000  .disconnectr2...
-00000a50: da0c 7379 6e63 6872 6f6e 697a 6572 da20  ..synchronizer. 
-00000a60: 7374 7265 616d 5f74 6f6f 6c73 5f64 6973  stream_tools_dis
-00000a70: 636f 6e6e 6563 7465 645f 7369 676e 616c  connected_signal
-00000a80: da04 656d 6974 2905 723b 0000 00da 0470  ..emit).r;.....p
-00000a90: 6f72 74da 0673 7472 6561 6dda 0363 616d  ort..stream..cam
-00000aa0: da07 6d6f 6e6f 6361 6c72 2500 0000 7225  ..monocalr%...r%
-00000ab0: 0000 0072 2600 0000 da12 6469 7363 6f6e  ...r&.....discon
-00000ac0: 6e65 6374 5f63 616d 6572 6173 5a00 0000  nect_camerasZ...
-00000ad0: 7318 0000 0012 040c 0106 0112 010a 0106  s...............
-00000ae0: 0112 010c 0106 010c 0106 010e 027a 1a53  .............z.S
-00000af0: 6573 7369 6f6e 2e64 6973 636f 6e6e 6563  ession.disconnec
-00000b00: 745f 6361 6d65 7261 7363 0100 0000 0000  t_camerasc......
-00000b10: 0000 0000 0000 0200 0000 0200 0000 4300  ..............C.
-00000b20: 0000 731e 0000 0074 007c 006a 0183 0164  ..s....t.|.j...d
-00000b30: 016b 0472 0b64 027d 017c 0153 0064 037d  .k.r.d.}.|.S.d.}
-00000b40: 017c 0153 0029 044e 7201 0000 0054 4629  .|.S.).Nr....TF)
-00000b50: 02da 036c 656e 722e 0000 0029 0272 3b00  ...lenr....).r;.
-00000b60: 0000 da08 656c 6967 6962 6c65 7225 0000  ....eligibler%..
-00000b70: 0072 2500 0000 7226 0000 00da 1869 735f  .r%...r&.....is_
-00000b80: 6361 6d65 7261 5f73 6574 7570 5f65 6c69  camera_setup_eli
-00000b90: 6769 626c 656c 0000 0073 0a00 0000 0e01  giblel...s......
-00000ba0: 0401 0403 04ff 0401 7a20 5365 7373 696f  ........z Sessio
-00000bb0: 6e2e 6973 5f63 616d 6572 615f 7365 7475  n.is_camera_setu
-00000bc0: 705f 656c 6967 6962 6c65 6301 0000 0000  p_eligiblec.....
-00000bd0: 0000 0000 0000 0004 0000 0003 0000 0043  ...............C
-00000be0: 0000 0073 4c00 0000 7c00 6a00 a001 a100  ...sL...|.j.....
-00000bf0: 0100 7c00 6a00 a002 a100 7c00 5f03 6401  ..|.j.....|._.d.
-00000c00: 7d01 7c00 6a03 6a04 a005 a100 4400 5d10  }.|.j.j.....D.].
-00000c10: 5c02 7d02 7d03 7c03 6a06 6400 7500 7321  \.}.}.|.j.d.u.s!
-00000c20: 7c03 6a07 6400 7500 7223 6402 7d01 7113  |.j.d.u.r#d.}.q.
-00000c30: 7c01 5300 2903 4e54 4629 0872 2800 0000  |.S.).NTF).r(...
-00000c40: da11 7265 6672 6573 685f 6672 6f6d 5f74  ..refresh_from_t
-00000c50: 6f6d 6cda 1067 6574 5f63 616d 6572 615f  oml..get_camera_
-00000c60: 6172 7261 79da 0c63 616d 6572 615f 6172  array..camera_ar
-00000c70: 7261 7972 2e00 0000 723e 0000 005a 066d  rayr....r>...Z.m
-00000c80: 6174 7269 785a 0b64 6973 746f 7274 696f  atrixZ.distortio
-00000c90: 6e73 a904 723b 0000 0072 4a00 0000 7244  ns..r;...rJ...rD
-00000ca0: 0000 0072 4600 0000 7225 0000 0072 2500  ...rF...r%...r%.
-00000cb0: 0000 7226 0000 00da 2169 735f 6578 7472  ..r&....!is_extr
-00000cc0: 696e 7369 635f 6361 6c69 6272 6174 696f  insic_calibratio
-00000cd0: 6e5f 656c 6967 6962 6c65 7300 0000 7310  n_eligibles...s.
-00000ce0: 0000 000a 020c 0104 0114 0114 0104 0102  ................
-00000cf0: 8004 027a 2953 6573 7369 6f6e 2e69 735f  ...z)Session.is_
-00000d00: 6578 7472 696e 7369 635f 6361 6c69 6272  extrinsic_calibr
-00000d10: 6174 696f 6e5f 656c 6967 6962 6c65 6301  ation_eligiblec.
-00000d20: 0000 0000 0000 0000 0000 0004 0000 0007  ................
-00000d30: 0000 0043 0000 0073 8800 0000 7c00 6a00  ...C...s....|.j.
-00000d40: a001 a100 0100 7c00 6a00 a002 a100 7c00  ......|.j.....|.
-00000d50: 5f03 6401 7d01 7404 7c00 6a03 6a05 8301  _.d.}.t.|.j.j...
-00000d60: 6402 6b00 7217 6403 7d01 7c00 6a03 6a05  d.k.r.d.}.|.j.j.
-00000d70: a006 a100 4400 5d1c 5c02 7d02 7d03 7c03  ....D.].\.}.}.|.
-00000d80: 6a07 6404 7500 732b 7c03 6a08 6404 7500  j.d.u.s+|.j.d.u.
-00000d90: 7239 6403 7d01 7409 a00a 6405 7c02 9b00  r9d.}.t...d.|...
-00000da0: 6406 7c03 6a0b 9b00 9d04 a101 0100 711d  d.|.j.........q.
-00000db0: 7409 a00a 6407 7c01 9b00 9d02 a101 0100  t...d.|.........
-00000dc0: 7c01 5300 2908 7afc 0a20 2020 2020 2020  |.S.).z..       
-00000dd0: 2069 6620 616c 6c20 6361 6d65 7261 7320   if all cameras 
-00000de0: 7468 6174 2061 7265 206e 6f74 2069 676e  that are not ign
-00000df0: 6f72 6564 2068 6176 6520 726f 7461 7469  ored have rotati
-00000e00: 6f6e 2061 6e64 2074 7261 6e73 6c61 7469  on and translati
-00000e10: 6f6e 206e 6f74 204e 6f6e 650a 2020 2020  on not None.    
-00000e20: 2020 2020 616e 6420 7468 6572 6520 6973      and there is
-00000e30: 2061 2063 6170 7475 7265 2076 6f6c 756d   a capture volum
-00000e40: 6520 6c6f 6164 6564 2075 702c 2074 6865  e loaded up, the
-00000e50: 6e20 796f 7520 6361 6e20 6c61 756e 6368  n you can launch
-00000e60: 2064 6972 6563 740a 2020 2020 2020 2020   direct.        
-00000e70: 696e 746f 2074 6865 2063 6170 7475 7265  into the capture
-00000e80: 2076 6f6c 756d 6520 7769 6467 6574 2072   volume widget r
-00000e90: 6174 6865 7220 7468 616e 2074 6865 2065  ather than the e
-00000ea0: 7874 7269 6e73 6963 2063 616c 6962 7261  xtrinsic calibra
-00000eb0: 7469 6f6e 2077 6964 6765 740a 2020 2020  tion widget.    
-00000ec0: 2020 2020 54e9 0200 0000 464e 7a30 4661      T.....FNz0Fa
-00000ed0: 696c 6564 2063 6170 7475 7265 2076 6f6c  iled capture vol
-00000ee0: 756d 6520 656c 6967 6962 696c 6974 7920  ume eligibility 
-00000ef0: 6475 6520 746f 2063 616d 6572 6120 7a02  due to camera z.
-00000f00: 3a20 7a45 456c 6967 6962 6c65 2074 6f20  : zEEligible to 
-00000f10: 6c6f 6164 2063 6170 7475 7265 2076 6f6c  load capture vol
-00000f20: 756d 653f 2028 692e 652e 2066 756c 6c79  ume? (i.e. fully
-00000f30: 2063 616c 6962 7261 7465 6420 6578 7472   calibrated extr
-00000f40: 696e 7369 6373 293a 2029 0c72 2800 0000  insics): ).r(...
-00000f50: 724c 0000 0072 4d00 0000 724e 0000 0072  rL...rM...rN...r
-00000f60: 4900 0000 722e 0000 0072 3e00 0000 da08  I...r....r>.....
-00000f70: 726f 7461 7469 6f6e da0b 7472 616e 736c  rotation..transl
-00000f80: 6174 696f 6eda 066c 6f67 6765 72da 0469  ation..logger..i
-00000f90: 6e66 6fda 085f 5f64 6963 745f 5f72 4f00  nfo..__dict__rO.
-00000fa0: 0000 7225 0000 0072 2500 0000 7226 0000  ..r%...r%...r&..
-00000fb0: 00da 1a69 735f 6361 7074 7572 655f 766f  ...is_capture_vo
-00000fc0: 6c75 6d65 5f65 6c69 6769 626c 657e 0000  lume_eligible~..
-00000fd0: 0073 2000 0000 0a08 0c01 0403 1001 0401  .s .............
-00000fe0: 1402 1401 0401 0401 1001 04ff 0280 0404  ................
-00000ff0: 0801 04ff 0404 7a22 5365 7373 696f 6e2e  ......z"Session.
-00001000: 6973 5f63 6170 7475 7265 5f76 6f6c 756d  is_capture_volum
-00001010: 655f 656c 6967 6962 6c65 6301 0000 0000  e_eligiblec.....
-00001020: 0000 0000 0000 0004 0000 0006 0000 0043  ...............C
-00001030: 0000 0073 8c00 0000 7c00 6a00 a001 a100  ...s....|.j.....
-00001040: 0100 7c00 6a00 a002 a100 7c00 5f03 6401  ..|.j.....|._.d.
-00001050: 7d01 7404 7c00 6a03 6a05 8301 6402 6b00  }.t.|.j.j...d.k.
-00001060: 7217 6403 7d01 7c00 6a03 6a05 a006 a100  r.d.}.|.j.j.....
-00001070: 4400 5d1e 5c02 7d02 7d03 7c03 6a07 6403  D.].\.}.}.|.j.d.
-00001080: 6b02 723b 7c03 6a08 6404 7500 7330 7c03  k.r;|.j.d.u.s0|.
-00001090: 6a09 6404 7500 723b 6403 7d01 740a a00b  j.d.u.r;d.}.t...
-000010a0: 6405 7c02 9b00 6406 9d03 a101 0100 711d  d.|...d.......q.
-000010b0: 7c01 7242 6401 7d01 7c01 5300 6403 7d01  |.rBd.}.|.S.d.}.
-000010c0: 7c01 5300 2907 7a44 0a20 2020 2020 2020  |.S.).zD.       
-000010d0: 2055 7365 6420 746f 2064 6574 6572 6d69   Used to determi
-000010e0: 6e65 2069 6620 7468 6520 5265 636f 7264  ne if the Record
-000010f0: 2042 7574 746f 6e20 6973 2065 6e61 626c   Button is enabl
-00001100: 6564 0a0a 2020 2020 2020 2020 5472 5100  ed..        TrQ.
-00001110: 0000 464e 7a34 4361 6d65 7261 2061 7272  ..FNz4Camera arr
-00001120: 6179 2069 7320 6e6f 7420 6675 6c6c 7920  ay is not fully 
-00001130: 6361 6c69 6272 6174 6564 2062 6563 6175  calibrated becau
-00001140: 7365 2063 616d 6572 6120 7a11 206c 6163  se camera z. lac
-00001150: 6b73 2065 7874 7269 6e73 6963 7329 0c72  ks extrinsics).r
-00001160: 2800 0000 724c 0000 0072 4d00 0000 724e  (...rL...rM...rN
-00001170: 0000 0072 4900 0000 722e 0000 0072 3e00  ...rI...r....r>.
-00001180: 0000 da06 6967 6e6f 7265 7252 0000 0072  ....ignorerR...r
-00001190: 5300 0000 7254 0000 0072 5500 0000 2904  S...rT...rU...).
-000011a0: 723b 0000 0072 4a00 0000 7244 0000 005a  r;...rJ...rD...Z
-000011b0: 0663 616d 6572 6172 2500 0000 7225 0000  .camerar%...r%..
-000011c0: 0072 2600 0000 da15 6973 5f72 6563 6f72  .r&.....is_recor
-000011d0: 6469 6e67 5f65 6c69 6769 626c 659b 0000  ding_eligible...
-000011e0: 0073 2a00 0000 0a07 0c01 0403 1001 0401  .s*.............
-000011f0: 1402 0a01 0801 02ff 0801 02ff 0403 0401  ................
-00001200: 0a01 04ff 0280 0403 0401 0404 04fe 0402  ................
-00001210: 7a1d 5365 7373 696f 6e2e 6973 5f72 6563  z.Session.is_rec
-00001220: 6f72 6469 6e67 5f65 6c69 6769 626c 6563  ording_eligiblec
-00001230: 0100 0000 0000 0000 0000 0000 0500 0000  ................
-00001240: 0500 0000 4300 0000 7346 0000 0064 017d  ....C...sF...d.}
-00001250: 017c 006a 00a0 01a1 0044 005d 197d 027c  .|.j.....D.].}.|
-00001260: 02a0 02a1 0072 2074 037c 02a0 0464 02a1  .....r t.|...d..
-00001270: 0183 017d 037c 0264 031b 007d 047c 0372  ...}.|.d...}.|.r
-00001280: 207c 04a0 05a1 0072 2064 047d 0171 077c   |.....r d.}.q.|
-00001290: 0153 0029 057a a60a 2020 2020 2020 2020  .S.).z..        
-000012a0: 506f 7374 2070 726f 6365 7373 696e 6720  Post processing 
-000012b0: 6361 6e20 6f6e 6c79 2062 6520 7065 7266  can only be perf
-000012c0: 6f72 6d65 6420 6966 2072 6563 6f72 6469  ormed if recordi
-000012d0: 6e67 7320 286d 7034 2066 696c 6573 2920  ngs (mp4 files) 
-000012e0: 6578 6973 7420 616e 6420 6578 7472 696e  exist and extrin
-000012f0: 7369 6373 200a 2020 2020 2020 2020 2863  sics .        (c
-00001300: 6f6e 6669 672e 746f 6d6c 2920 6172 6520  onfig.toml) are 
-00001310: 6361 6c69 6272 6174 6564 2069 6e20 7468  calibrated in th
-00001320: 6520 2772 6563 6f72 6427 2064 6972 6563  e 'record' direc
-00001330: 746f 7279 0a20 2020 2020 2020 2046 7a05  tory.        Fz.
-00001340: 2a2e 6d70 347a 0b63 6f6e 6669 672e 746f  *.mp4z.config.to
-00001350: 6d6c 5429 0672 2c00 0000 da07 6974 6572  mlT).r,.....iter
-00001360: 6469 72da 0669 735f 6469 72da 046c 6973  dir..is_dir..lis
-00001370: 74da 0467 6c6f 62da 0665 7869 7374 7329  t..glob..exists)
-00001380: 0572 3b00 0000 724a 0000 00da 0563 6869  .r;...rJ.....chi
-00001390: 6c64 5a09 6d70 345f 6669 6c65 735a 0b63  ldZ.mp4_filesZ.c
-000013a0: 6f6e 6669 675f 6669 6c65 7225 0000 0072  onfig_filer%...r
-000013b0: 2500 0000 7226 0000 00da 1b69 735f 706f  %...r&.....is_po
-000013c0: 7374 5f70 726f 6365 7373 696e 675f 656c  st_processing_el
-000013d0: 6967 6962 6c65 b900 0000 7312 0000 0004  igible....s.....
-000013e0: 060e 0108 010e 0108 010c 0104 0102 8004  ................
-000013f0: 027a 2353 6573 7369 6f6e 2e69 735f 706f  .z#Session.is_po
-00001400: 7374 5f70 726f 6365 7373 696e 675f 656c  st_processing_el
-00001410: 6967 6962 6c65 723a 0000 0063 0200 0000  igibler:...c....
-00001420: 0000 0000 0000 0000 0200 0000 0300 0000  ................
-00001430: 4300 0000 73bc 0100 007c 017c 005f 007c  C...s....|.|._.|
-00001440: 00a0 01a1 0001 007c 006a 0004 0074 026a  .......|.j...t.j
-00001450: 036b 0272 1f01 007c 006a 0472 1d7c 006a  .k.r...|.j.r.|.j
-00001460: 05a0 06a1 0001 007c 00a0 07a1 0001 0064  .......|.......d
-00001470: 0953 0064 0953 0004 0074 026a 086b 0272  .S.d.S...t.j.k.r
-00001480: 3501 007c 006a 0472 337c 006a 05a0 06a1  5..|.j.r3|.j....
-00001490: 0001 007c 00a0 07a1 0001 0064 0953 0064  ...|.......d.S.d
-000014a0: 0953 0004 0074 026a 096b 0272 6201 0074  .S...t.j.k.rb..t
-000014b0: 0a7c 006a 0b83 017c 005f 0c7c 006a 0473  .|.j...|._.|.j.s
-000014c0: 487c 00a0 0da1 0001 007c 006a 05a0 06a1  H|.......|.j....
-000014d0: 0001 007c 00a0 07a1 0001 007c 00a0 0ea1  ...|.......|....
-000014e0: 0001 007c 00a0 0f64 01a1 0101 007c 00a0  ...|...d.....|..
-000014f0: 107c 006a 11a1 0101 0064 0953 0004 0074  .|.j.....d.S...t
-00001500: 026a 126b 0272 8901 0074 0a7c 006a 0b83  .j.k.r...t.|.j..
-00001510: 017c 005f 0c7c 006a 0473 757c 00a0 0da1  .|._.|.j.su|....
-00001520: 0001 007c 00a0 07a1 0001 007c 00a0 0ea1  ...|.......|....
-00001530: 0001 007c 00a0 0f64 01a1 0101 007c 006a  ...|...d.....|.j
-00001540: 05a0 13a1 0001 0064 0953 0004 0074 026a  .......d.S...t.j
-00001550: 146b 0272 9f01 007c 006a 0472 9d7c 00a0  .k.r...|.j.r.|..
-00001560: 07a1 0001 007c 006a 05a0 06a1 0001 0064  .....|.j.......d
-00001570: 0953 0064 0953 0074 026a 156b 0272 dc74  .S.d.S.t.j.k.r.t
-00001580: 16a0 1764 02a1 0101 007c 006a 0473 b474  ...d.....|.j.s.t
-00001590: 16a0 1764 03a1 0101 007c 00a0 0da1 0001  ...d.....|......
-000015a0: 0074 16a0 1764 04a1 0101 007c 00a0 07a1  .t...d.....|....
-000015b0: 0001 0074 16a0 1764 05a1 0101 007c 00a0  ...t...d.....|..
-000015c0: 0f64 06a1 0101 0074 16a0 1764 07a1 0101  .d.....t...d....
-000015d0: 007c 00a0 01a1 0001 0074 16a0 1764 08a1  .|.......t...d..
-000015e0: 0101 007c 006a 05a0 13a1 0001 0064 0953  ...|.j.......d.S
-000015f0: 0064 0953 0029 0a7a af0a 2020 2020 2020  .d.S.).z..      
-00001600: 2020 5669 6120 7468 6973 206d 6574 686f    Via this metho
-00001610: 642c 2074 6865 2066 7261 6d65 2072 6561  d, the frame rea
-00001620: 6469 6e67 2062 6568 6176 696f 7220 7769  ding behavior wi
-00001630: 6c6c 2062 6520 6368 616e 6765 6420 6279  ll be changed by
-00001640: 2074 6865 2047 5549 2e20 4966 2073 6f6d   the GUI. If som
-00001650: 6520 7072 6f70 6572 7469 6573 2061 7265  e properties are
-00001660: 0a20 2020 2020 2020 206e 6f74 2061 7661  .        not ava
-00001670: 696c 6162 6c65 2028 692e 652e 2073 796e  ilable (i.e. syn
-00001680: 6368 726f 6e69 7a65 7229 2074 6865 7920  chronizer) they 
-00001690: 7769 6c6c 2062 6520 6372 6561 7465 640a  will be created.
-000016a0: 2020 2020 2020 2020 547a 2041 7474 656d          Tz Attem
-000016b0: 7074 696e 6720 746f 2073 6574 2072 6563  pting to set rec
-000016c0: 6f72 6469 6e67 206d 6f64 657a 2e53 7472  ording modez.Str
-000016d0: 6561 6d20 746f 6f6c 7320 6e6f 7420 6c6f  eam tools not lo
-000016e0: 6164 6564 2c20 736f 206c 6f61 6469 6e67  aded, so loading
-000016f0: 2074 6865 6d20 7570 2e2e 2e7a 2850 6175   them up...z(Pau
-00001700: 7369 6e67 206d 6f6e 6f63 616c 7320 746f  sing monocals to
-00001710: 2065 6e74 6572 2072 6563 6f72 6469 6e67   enter recording
-00001720: 206d 6f64 657a 2053 746f 7020 7472 6163   modez Stop trac
-00001730: 6b69 6e67 2066 6f72 2072 6563 6f72 6469  king for recordi
-00001740: 6e67 206d 6f64 6546 7a22 5570 6461 7465  ng modeFz"Update
-00001750: 2073 7472 6561 6d20 6670 7320 746f 2072   stream fps to r
-00001760: 6563 6f72 6469 6e67 2066 7073 7a3e 5375  ecording fpsz>Su
-00001770: 6273 6372 6962 6520 7379 6e63 6872 6f6e  bscribe synchron
-00001780: 697a 6572 2074 6f20 7374 7265 616d 7320  izer to streams 
-00001790: 736f 2076 6964 656f 2072 6563 6f72 6465  so video recorde
-000017a0: 7220 6361 6e20 6d61 6e61 6765 4e29 1872  r can manageN).r
-000017b0: 3a00 0000 da12 7570 6461 7465 5f73 7472  :.....update_str
-000017c0: 6561 6d73 5f66 7073 7219 0000 0072 1f00  eams_fpsr....r..
-000017d0: 0000 7231 0000 0072 4100 0000 da18 756e  ..r1...rA.....un
-000017e0: 7375 6273 6372 6962 655f 6672 6f6d 5f73  subscribe_from_s
-000017f0: 7472 6561 6d73 da19 7061 7573 655f 616c  treams..pause_al
-00001800: 6c5f 6d6f 6e6f 6361 6c69 6272 6174 6f72  l_monocalibrator
-00001810: 7372 2400 0000 7220 0000 0072 0900 0000  sr$...r ...r....
-00001820: 7238 0000 0072 3900 0000 da11 6c6f 6164  r8...r9.....load
-00001830: 5f73 7472 6561 6d5f 746f 6f6c 73da 1373  _stream_tools..s
-00001840: 6574 5f73 7472 6561 6d73 5f63 6861 7275  et_streams_charu
-00001850: 636f da14 7365 745f 7374 7265 616d 735f  co..set_streams_
-00001860: 7472 6163 6b69 6e67 da17 6163 7469 7661  tracking..activa
-00001870: 7465 5f6d 6f6e 6f63 616c 6962 7261 746f  te_monocalibrato
-00001880: 7272 3300 0000 7221 0000 00da 1473 7562  rr3...r!.....sub
-00001890: 7363 7269 6265 5f74 6f5f 7374 7265 616d  scribe_to_stream
-000018a0: 7372 2200 0000 7223 0000 0072 5400 0000  sr"...r#...rT...
-000018b0: 7255 0000 0029 0272 3b00 0000 723a 0000  rU...).r;...r:..
-000018c0: 0072 2500 0000 7225 0000 0072 2600 0000  .r%...r%...r&...
-000018d0: da08 7365 745f 6d6f 6465 c900 0000 7362  ..set_mode....sb
-000018e0: 0000 0006 0508 0104 020c 0106 010a 010c  ................
-000018f0: 0104 fe0c 0406 010a 010c 0104 fe0c 040c  ................
-00001900: 0206 0208 010a 0108 0108 010a 0110 010c  ................
-00001910: 020c 0206 0108 0108 0208 010a 010e 020c  ................
-00001920: 0206 0108 010e 0104 fe08 040a 0106 010a  ................
-00001930: 0108 010a 0208 010a 020a 010a 0108 010a  ................
-00001940: 020e 0104 f17a 1053 6573 7369 6f6e 2e73  .....z.Session.s
-00001950: 6574 5f6d 6f64 65da 0a66 7073 5f74 6172  et_mode..fps_tar
-00001960: 6765 7463 0200 0000 0000 0000 0000 0000  getc............
-00001970: 0200 0000 0300 0000 4300 0000 7386 0000  ........C...s...
-00001980: 007c 006a 0004 0074 016a 026b 0272 0901  .|.j...t.j.k.r..
-00001990: 006e 3404 0074 016a 036b 0272 1001 006e  .n4..t.j.k.r...n
-000019a0: 2d04 0074 016a 046b 0272 2001 007c 017c  -..t.j.k.r ..|.|
-000019b0: 005f 057c 006a 06a0 077c 01a1 0101 006e  ._.|.j...|.....n
-000019c0: 1d04 0074 016a 086b 0272 3001 007c 017c  ...t.j.k.r0..|.|
-000019d0: 005f 097c 006a 06a0 0a7c 01a1 0101 006e  ._.|.j...|.....n
-000019e0: 0d74 016a 0b6b 0272 3d7c 017c 005f 0c7c  .t.j.k.r=|.|._.|
-000019f0: 006a 06a0 0d7c 01a1 0101 007c 00a0 0ea1  .j...|.....|....
-00001a00: 0001 0064 0153 0029 027a 780a 2020 2020  ...d.S.).zx.    
-00001a10: 2020 2020 5570 6461 7465 7320 7468 6520      Updates the 
-00001a20: 4650 5320 7573 6564 2062 7920 7468 6520  FPS used by the 
-00001a30: 6375 7272 656e 746c 7920 6163 7469 7665  currently active
-00001a40: 2073 6573 7369 6f6e 206d 6f64 650a 2020   session mode.  
-00001a50: 2020 2020 2020 5468 6973 2075 7064 6174        This updat
-00001a60: 6520 696e 636c 7564 6573 2074 6865 2063  e includes the c
-00001a70: 6f6e 6669 672e 746f 6d6c 0a20 2020 2020  onfig.toml.     
-00001a80: 2020 204e 290f 723a 0000 0072 1900 0000     N).r:...r....
-00001a90: 721f 0000 0072 2400 0000 7220 0000 0072  r....r$...r ...r
-00001aa0: 3600 0000 7228 0000 005a 1e73 6176 655f  6...r(...Z.save_
-00001ab0: 6670 735f 696e 7472 696e 7369 635f 6361  fps_intrinsic_ca
-00001ac0: 6c69 6272 6174 696f 6e72 2100 0000 7235  librationr!...r5
-00001ad0: 0000 005a 1e73 6176 655f 6670 735f 6578  ...Z.save_fps_ex
-00001ae0: 7472 696e 7369 635f 6361 6c69 6272 6174  trinsic_calibrat
-00001af0: 696f 6e72 2300 0000 7234 0000 005a 1273  ionr#...r4...Z.s
-00001b00: 6176 655f 6670 735f 7265 636f 7264 696e  ave_fps_recordin
-00001b10: 6772 6100 0000 2902 723b 0000 0072 6a00  gra...).r;...rj.
-00001b20: 0000 7225 0000 0072 2500 0000 7226 0000  ..r%...r%...r&..
-00001b30: 00da 1373 6574 5f61 6374 6976 655f 6d6f  ...set_active_mo
-00001b40: 6465 5f66 7073 0a01 0000 731e 0000 0004  de_fps....s.....
-00001b50: 050c 0102 010c 0102 010c 0106 010e 010c  ................
-00001b60: 0106 010e 0108 0106 010c 010c 027a 1b53  .............z.S
-00001b70: 6573 7369 6f6e 2e73 6574 5f61 6374 6976  ession.set_activ
-00001b80: 655f 6d6f 6465 5f66 7073 da06 7265 7475  e_mode_fps..retu
-00001b90: 726e 6301 0000 0000 0000 0000 0000 0002  rnc.............
-00001ba0: 0000 0003 0000 0043 0000 0073 6e00 0000  .......C...sn...
-00001bb0: 6400 7d01 7c00 6a00 0400 7401 6a02 6b02  d.}.|.j...t.j.k.
-00001bc0: 720d 0100 0900 7c01 5300 0400 7401 6a03  r.....|.S...t.j.
-00001bd0: 6b02 7216 0100 0900 7c01 5300 0400 7401  k.r.....|.S...t.
-00001be0: 6a04 6b02 7221 0100 7c00 6a05 7d01 7c01  j.k.r!..|.j.}.|.
-00001bf0: 5300 0400 7401 6a06 6b02 722c 0100 7c00  S...t.j.k.r,..|.
-00001c00: 6a07 7d01 7c01 5300 7401 6a08 6b02 7235  j.}.|.S.t.j.k.r5
-00001c10: 7c00 6a09 7d01 7c01 5300 7c01 5300 a901  |.j.}.|.S.|.S...
-00001c20: 4e29 0a72 3a00 0000 7219 0000 0072 1f00  N).r:...r....r..
-00001c30: 0000 7224 0000 0072 2000 0000 7236 0000  ..r$...r ...r6..
-00001c40: 0072 2100 0000 7235 0000 0072 2300 0000  .r!...r5...r#...
-00001c50: 7234 0000 0029 0272 3b00 0000 5a03 6670  r4...).r;...Z.fp
-00001c60: 7372 2500 0000 7225 0000 0072 2600 0000  sr%...r%...r&...
-00001c70: da13 6765 745f 6163 7469 7665 5f6d 6f64  ..get_active_mod
-00001c80: 655f 6670 7320 0100 0073 2200 0000 0401  e_fps ...s".....
-00001c90: 0401 0c01 0201 0409 0cf8 0201 0407 0cfa  ................
-00001ca0: 0601 0405 0cfc 0601 0403 08fe 0601 0801  ................
-00001cb0: 7a1b 5365 7373 696f 6e2e 6765 745f 6163  z.Session.get_ac
-00001cc0: 7469 7665 5f6d 6f64 655f 6670 7363 0100  tive_mode_fpsc..
-00001cd0: 0000 0000 0000 0000 0000 0400 0000 0400  ................
-00001ce0: 0000 4300 0000 7336 0000 007c 00a0 00a1  ..C...s6...|....
-00001cf0: 007d 017c 0164 0075 0172 177c 006a 01a0  .}.|.d.u.r.|.j..
-00001d00: 02a1 0044 005d 0b5c 027d 027d 037c 03a0  ...D.].\.}.}.|..
-00001d10: 037c 01a1 0101 0071 0d64 0053 0064 0053  .|.....q.d.S.d.S
-00001d20: 0072 6d00 0000 2904 726e 0000 0072 2f00  .rm...).rn...r/.
-00001d30: 0000 723e 0000 005a 0e73 6574 5f66 7073  ..r>...Z.set_fps
-00001d40: 5f74 6172 6765 7429 0472 3b00 0000 5a0f  _target).r;...Z.
-00001d50: 6163 7469 7665 5f6d 6f64 655f 6670 7372  active_mode_fpsr
-00001d60: 4400 0000 7245 0000 0072 2500 0000 7225  D...rE...r%...r%
-00001d70: 0000 0072 2600 0000 7261 0000 002f 0100  ...r&...ra.../..
-00001d80: 0073 0c00 0000 0801 0801 1201 0c01 04fe  .s..............
-00001d90: 0401 7a1a 5365 7373 696f 6e2e 7570 6461  ..z.Session.upda
-00001da0: 7465 5f73 7472 6561 6d73 5f66 7073 da0b  te_streams_fps..
-00001db0: 7472 6163 6b69 6e67 5f6f 6e63 0200 0000  tracking_onc....
-00001dc0: 0000 0000 0000 0000 0400 0000 0400 0000  ................
-00001dd0: 4300 0000 7322 0000 007c 006a 00a0 01a1  C...s"...|.j....
-00001de0: 0044 005d 095c 027d 027d 037c 03a0 027c  .D.].\.}.}.|...|
-00001df0: 01a1 0101 0071 0564 0053 0072 6d00 0000  .....q.d.S.rm...
-00001e00: 2903 722f 0000 0072 3e00 0000 5a0f 7365  ).r/...r>...Z.se
-00001e10: 745f 7472 6163 6b69 6e67 5f6f 6e29 0472  t_tracking_on).r
-00001e20: 3b00 0000 726f 0000 0072 4400 0000 7245  ;...ro...rD...rE
-00001e30: 0000 0072 2500 0000 7225 0000 0072 2600  ...r%...r%...r&.
-00001e40: 0000 7266 0000 0035 0100 0073 0600 0000  ..rf...5...s....
-00001e50: 1201 0c01 04ff 7a1c 5365 7373 696f 6e2e  ......z.Session.
-00001e60: 7365 745f 7374 7265 616d 735f 7472 6163  set_streams_trac
-00001e70: 6b69 6e67 6301 0000 0000 0000 0000 0000  kingc...........
-00001e80: 0003 0000 0004 0000 0043 0000 0073 3a00  .........C...s:.
-00001e90: 0000 7400 a001 6401 a101 0100 7402 7c00  ..t...d.....t.|.
-00001ea0: 6a03 8301 7c00 5f04 7c00 6a05 a006 a100  j...|._.|.j.....
-00001eb0: 4400 5d0a 5c02 7d01 7d02 7c02 a007 7c00  D.].\.}.}.|...|.
-00001ec0: 6a04 a101 0100 7110 6400 5300 2902 4e7a  j.....q.d.S.).Nz
-00001ed0: 2275 7064 6174 696e 6720 6368 6172 7563  "updating charuc
-00001ee0: 6f20 696e 2063 6173 6520 6e65 6365 7373  o in case necess
-00001ef0: 6172 7929 0872 5400 0000 7255 0000 0072  ary).rT...rU...r
-00001f00: 0900 0000 7238 0000 0072 3900 0000 722f  ....r8...r9...r/
-00001f10: 0000 0072 3e00 0000 5a0e 7570 6461 7465  ...r>...Z.update
-00001f20: 5f74 7261 636b 6572 2903 723b 0000 0072  _tracker).r;...r
-00001f30: 4400 0000 7245 0000 0072 2500 0000 7225  D...rE...r%...r%
-00001f40: 0000 0072 2600 0000 7265 0000 0039 0100  ...r&...re...9..
-00001f50: 0073 0a00 0000 0a01 0c01 1201 0e01 04ff  .s..............
-00001f60: 7a1b 5365 7373 696f 6e2e 7365 745f 7374  z.Session.set_st
-00001f70: 7265 616d 735f 6368 6172 7563 6f63 0100  reams_charucoc..
-00001f80: 0000 0000 0000 0000 0000 0100 0000 0300  ................
-00001f90: 0000 4300 0000 7318 0000 0074 00a0 0164  ..C...s....t...d
-00001fa0: 01a1 0101 007c 006a 02a0 03a1 0001 0064  .....|.j.......d
-00001fb0: 0053 0029 024e 7a14 7061 7573 696e 6720  .S.).Nz.pausing 
-00001fc0: 7379 6e63 6872 6f6e 697a 6572 2904 7254  synchronizer).rT
-00001fd0: 0000 0072 5500 0000 7241 0000 0072 6200  ...rU...rA...rb.
-00001fe0: 0000 a901 723b 0000 0072 2500 0000 7225  ....r;...r%...r%
-00001ff0: 0000 0072 2600 0000 da12 7061 7573 655f  ...r&.....pause_
-00002000: 7379 6e63 6872 6f6e 697a 6572 3f01 0000  synchronizer?...
-00002010: 7304 0000 000a 010e 017a 1a53 6573 7369  s........z.Sessi
-00002020: 6f6e 2e70 6175 7365 5f73 796e 6368 726f  on.pause_synchro
-00002030: 6e69 7a65 7263 0100 0000 0000 0000 0000  nizerc..........
-00002040: 0000 0100 0000 0300 0000 4300 0000 731e  ..........C...s.
-00002050: 0000 007c 006a 00a0 01a1 0001 007c 006a  ...|.j.......|.j
-00002060: 00a0 027c 006a 006a 03a1 0101 0064 0053  ...|.j.j.....d.S
-00002070: 0072 6d00 0000 2904 7241 0000 0072 6800  .rm...).rA...rh.
-00002080: 0000 5a0e 7365 745f 7374 7265 616d 5f66  ..Z.set_stream_f
-00002090: 7073 726a 0000 0072 7000 0000 7225 0000  psrj...rp...r%..
-000020a0: 0072 2500 0000 7226 0000 00da 1475 6e70  .r%...r&.....unp
-000020b0: 6175 7365 5f73 796e 6368 726f 6e69 7a65  ause_synchronize
-000020c0: 7243 0100 0073 0400 0000 0a01 1401 7a1c  rC...s........z.
-000020d0: 5365 7373 696f 6e2e 756e 7061 7573 655f  Session.unpause_
-000020e0: 7379 6e63 6872 6f6e 697a 6572 6301 0000  synchronizerc...
-000020f0: 0000 0000 0000 0000 0004 0000 0004 0000  ................
-00002100: 0043 0000 0073 3400 0000 6401 7d01 7c00  .C...s4...d.}.|.
-00002110: 6a00 6a01 a002 a100 a003 a100 4400 5d0d  j.j.........D.].
-00002120: 5c02 7d02 7d03 7c02 a004 6402 a101 7217  \.}.}.|...d...r.
-00002130: 7c01 6403 3700 7d01 710a 7c01 5300 2904  |.d.7.}.q.|.S.).
-00002140: 4e72 0100 0000 7246 0000 00e9 0100 0000  Nr....rF........
-00002150: 2905 7228 0000 00da 0464 6963 74da 0463  ).r(.....dict..c
-00002160: 6f70 7972 3e00 0000 da0a 7374 6172 7473  opyr>.....starts
-00002170: 7769 7468 2904 723b 0000 00da 0563 6f75  with).r;.....cou
-00002180: 6e74 da03 6b65 79da 0670 6172 616d 7372  nt..key..paramsr
-00002190: 2500 0000 7225 0000 0072 2600 0000 da1b  %...r%...r&.....
-000021a0: 6765 745f 636f 6e66 6967 7572 6564 5f63  get_configured_c
-000021b0: 616d 6572 615f 636f 756e 7447 0100 0073  amera_countG...s
-000021c0: 0c00 0000 0401 1801 0a01 0801 0280 0401  ................
-000021d0: 7a23 5365 7373 696f 6e2e 6765 745f 636f  z#Session.get_co
-000021e0: 6e66 6967 7572 6564 5f63 616d 6572 615f  nfigured_camera_
-000021f0: 636f 756e 7463 0100 0000 0000 0000 0000  countc..........
-00002200: 0000 0500 0000 0800 0000 0300 0000 738c  ..............s.
-00002210: 0000 0087 0066 0164 0164 0284 087d 0174  .....f.d.d...}.t
-00002220: 0083 008f 1e7d 0274 0164 0374 0283 0244  .....}.t.d.t...D
-00002230: 005d 107d 037c 0388 006a 03a0 04a1 0076  .].}.|...j.....v
-00002240: 0072 1971 0f7c 02a0 057c 017c 03a1 0201  .r.q.|...|.|....
-00002250: 0071 0f57 0064 0404 0004 0083 0301 006e  .q.W.d.........n
-00002260: 0831 0073 2a77 0101 0001 0001 0059 0001  .1.s*w.......Y..
-00002270: 0088 006a 066a 07a0 08a1 00a0 04a1 0044  ...j.j.........D
-00002280: 005d 0c7d 047c 04a0 0964 05a1 0172 4388  .].}.|...d...rC.
-00002290: 006a 066a 077c 043d 0071 3764 0453 0029  .j.j.|.=.q7d.S.)
-000022a0: 067a a30a 2020 2020 2020 2020 4361 6c6c  .z..        Call
-000022b0: 6564 2062 7920 6c6f 6164 5f73 7472 6561  ed by load_strea
-000022c0: 6d73 2069 6e20 7468 6520 6576 656e 7420  ms in the event 
-000022d0: 7468 6174 206e 6f20 6361 6d65 7261 7320  that no cameras 
-000022e0: 6172 6520 7265 7475 726e 6564 2062 7920  are returned by 
-000022f0: 7468 6520 636f 6e66 6967 7572 6174 6f72  the configurator
-00002300: 2e2e 2e0a 2020 2020 2020 2020 5769 6c6c  ....        Will
-00002310: 2070 6f70 756c 6174 6520 7365 6c66 2e63   populate self.c
-00002320: 616d 6572 6173 2075 7369 6e67 206d 756c  ameras using mul
-00002330: 7469 706c 6520 7468 7265 6164 730a 2020  tiple threads.  
-00002340: 2020 2020 2020 6301 0000 0000 0000 0000        c.........
-00002350: 0000 0002 0000 0007 0000 0013 0000 0073  ...............s
-00002360: 8c00 0000 7a37 7400 a001 6401 7c00 9b00  ....z7t...d.|...
-00002370: 9d02 a101 0100 7402 7c00 8301 7d01 7400  ......t.|...}.t.
-00002380: a001 6402 7c00 9b00 9d02 a101 0100 7c01  ..d.|.........|.
-00002390: 8800 6a03 7c00 3c00 8800 6a04 a005 7c01  ..j.|.<...j...|.
-000023a0: a101 0100 7400 a001 6403 7c00 9b00 6404  ....t...d.|...d.
-000023b0: 9d03 a101 0100 7406 7c01 7407 8800 6a08  ......t.|.t...j.
-000023c0: 8301 6405 8d02 8800 6a09 7c00 3c00 5700  ..d.....j.|.<.W.
-000023d0: 6400 5300 0100 0100 0100 7400 a001 6406  d.S.......t...d.
-000023e0: 7c00 9b00 9d02 a101 0100 5900 6400 5300  |.........Y.d.S.
-000023f0: 2907 4e7a 0c54 7279 696e 6720 706f 7274  ).Nz.Trying port
-00002400: 207a 1053 7563 6365 7373 2061 7420 706f   z.Success at po
-00002410: 7274 207a 174c 6f61 6469 6e67 2073 7472  rt z.Loading str
-00002420: 6561 6d20 6174 2070 6f72 7420 7a25 2077  eam at port z% w
-00002430: 6974 6820 6368 6172 7563 6f20 7472 6163  ith charuco trac
-00002440: 6b65 7220 666f 7220 6361 6c69 6272 6174  ker for calibrat
-00002450: 696f 6ea9 015a 0774 7261 636b 6572 7a12  ion..Z.trackerz.
-00002460: 4e6f 2063 616d 6572 6120 6174 2070 6f72  No camera at por
-00002470: 7420 290a 7254 0000 0072 5500 0000 720b  t ).rT...rU...r.
-00002480: 0000 0072 2e00 0000 7228 0000 005a 0b73  ...r....r(...Z.s
-00002490: 6176 655f 6361 6d65 7261 7216 0000 0072  ave_camerar....r
-000024a0: 0900 0000 7238 0000 0072 2f00 0000 2902  ....r8...r/...).
-000024b0: 7244 0000 0072 4600 0000 7270 0000 0072  rD...rF...rp...r
-000024c0: 2500 0000 7226 0000 00da 0761 6464 5f63  %...r&.....add_c
-000024d0: 616d 5401 0000 731c 0000 0002 0110 0108  amT...s.........
-000024e0: 0110 010a 010c 0104 010a 0104 ff02 030a  ................
-000024f0: 0112 ff06 0316 017a 2653 6573 7369 6f6e  .......z&Session
-00002500: 2e5f 6669 6e64 5f63 616d 6572 6173 2e3c  ._find_cameras.<
-00002510: 6c6f 6361 6c73 3e2e 6164 645f 6361 6d72  locals>.add_camr
-00002520: 0100 0000 4e5a 0673 7465 7265 6f29 0a72  ....NZ.stereo).r
-00002530: 0400 0000 da05 7261 6e67 65da 154d 4158  ......range..MAX
-00002540: 5f43 414d 4552 415f 504f 5254 5f43 4845  _CAMERA_PORT_CHE
-00002550: 434b 722e 0000 00da 046b 6579 73da 0673  CKr......keys..s
-00002560: 7562 6d69 7472 2800 0000 7274 0000 0072  ubmitr(...rt...r
-00002570: 7500 0000 7276 0000 0029 0572 3b00 0000  u...rv...).r;...
-00002580: 727c 0000 00da 0865 7865 6375 746f 72da  r|.....executor.
-00002590: 0169 7278 0000 0072 2500 0000 7270 0000  .irx...r%...rp..
-000025a0: 0072 2600 0000 da0d 5f66 696e 645f 6361  .r&....._find_ca
-000025b0: 6d65 7261 734e 0100 0073 1a00 0000 0c06  merasN...s......
-000025c0: 0810 0e01 0e01 0202 0e02 02fb 1cff 1409  ................
-000025d0: 0a01 0a01 0280 04fe 7a15 5365 7373 696f  ........z.Sessio
-000025e0: 6e2e 5f66 696e 645f 6361 6d65 7261 7363  n._find_camerasc
-000025f0: 0100 0000 0000 0000 0000 0000 0300 0000  ................
-00002600: 0500 0000 4300 0000 73da 0000 0064 017c  ....C...s....d.|
-00002610: 005f 007c 006a 01a0 02a1 007c 005f 0374  ._.|.j.....|._.t
-00002620: 047c 006a 0383 0164 026b 0272 147c 00a0  .|.j...d.k.r.|..
-00002630: 05a1 0001 007c 006a 03a0 06a1 0044 005d  .....|.j.....D.]
-00002640: 1e5c 027d 017d 027c 017c 006a 07a0 08a1  .\.}.}.|.|.j....
-00002650: 0076 0072 2571 1974 09a0 0a64 037c 019b  .v.r%q.t...d.|..
-00002660: 009d 02a1 0101 0074 0b7c 027c 006a 0c64  .......t.|.|.j.d
-00002670: 048d 027c 006a 077c 013c 0071 197c 00a0  ...|.j.|.<.q.|..
-00002680: 0da1 0001 007c 00a0 0ea1 0001 0074 0f7c  .....|.......t.|
-00002690: 006a 10a0 08a1 0083 017c 005f 1174 127c  .j.......|._.t.|
-000026a0: 006a 0783 017c 005f 1364 017c 005f 1464  .j...|._.d.|._.d
-000026b0: 057c 005f 0074 09a0 0a64 06a1 0101 007c  .|._.t...d.....|
-000026c0: 00a0 15a1 0001 007c 00a0 16a1 0001 0074  .......|.......t
-000026d0: 09a0 0a64 07a1 0101 007c 006a 17a0 18a1  ...d.....|.j....
-000026e0: 0001 0064 0853 0029 097a ad0a 2020 2020  ...d.S.).z..    
-000026f0: 2020 2020 436f 6e6e 6563 7473 2074 6f20      Connects to 
-00002700: 7374 6f72 6564 2063 616d 6572 6173 2061  stored cameras a
-00002710: 6e64 2063 7265 6174 6573 2073 7472 6561  nd creates strea
-00002720: 6d73 2077 6974 6820 7072 6f76 6964 6564  ms with provided
-00002730: 2074 7261 636b 696e 670a 2020 2020 2020   tracking.      
-00002740: 2020 4265 6361 7573 6520 7468 6573 6520    Because these 
-00002750: 7374 7265 616d 7320 6172 6520 6176 6169  streams are avai
-00002760: 6c61 626c 652c 2074 6865 2073 796e 6368  lable, the synch
-00002770: 726f 6e69 7a65 7220 6361 6e20 7468 656e  ronizer can then
-00002780: 2062 6520 696e 6974 6961 6c69 7a65 640a   be initialized.
-00002790: 2020 2020 2020 2020 5472 0100 0000 7a18          Tr....z.
-000027a0: 4c6f 6164 696e 6720 5374 7265 616d 2066  Loading Stream f
-000027b0: 6f72 2070 6f72 7420 727b 0000 0046 7a33  or port r{...Fz3
-000027c0: 5061 7573 696e 6720 7374 7265 616d 2074  Pausing stream t
-000027d0: 6f6f 6c73 2073 696e 6365 2064 6566 6175  ools since defau
-000027e0: 6c74 206c 6f61 6473 2074 6f20 6368 6172  lt loads to char
-000027f0: 7563 6f7a 2d53 6967 6e61 6c6c 696e 6720  ucoz-Signalling 
-00002800: 7375 6363 6573 7366 756c 206c 6f61 6469  successful loadi
-00002810: 6e67 206f 6620 7374 7265 616d 2074 6f6f  ng of stream too
-00002820: 6c73 4e29 1972 3000 0000 7228 0000 005a  lsN).r0...r(...Z
-00002830: 0b67 6574 5f63 616d 6572 6173 722e 0000  .get_camerasr...
-00002840: 0072 4900 0000 7283 0000 0072 3e00 0000  .rI...r....r>...
-00002850: 722f 0000 0072 7f00 0000 7254 0000 0072  r/...r....rT...r
-00002860: 5500 0000 7216 0000 0072 3900 0000 da13  U...r....r9.....
-00002870: 5f61 646a 7573 745f 7265 736f 6c75 7469  _adjust_resoluti
-00002880: 6f6e 73da 155f 6c6f 6164 5f6d 6f6e 6f63  ons.._load_monoc
-00002890: 616c 6962 7261 746f 7273 da03 6d69 6e72  alibrators..minr
-000028a0: 3200 0000 7233 0000 0072 0c00 0000 7241  2...r3...r....rA
-000028b0: 0000 0072 3100 0000 7263 0000 0072 7100  ...r1...rc...rq.
-000028c0: 0000 da1a 7374 7265 616d 5f74 6f6f 6c73  ....stream_tools
-000028d0: 5f6c 6f61 6465 645f 7369 676e 616c 7243  _loaded_signalrC
-000028e0: 0000 00a9 0372 3b00 0000 7244 0000 0072  .....r;...rD...r
-000028f0: 4600 0000 7225 0000 0072 2500 0000 7226  F...r%...r%...r&
-00002900: 0000 0072 6400 0000 7101 0000 732c 0000  ...rd...q...s,..
-00002910: 0006 050c 020e 0208 0112 020e 0102 0110  ................
-00002920: 0216 0108 0208 0110 0302 0204 0106 ff06  ................
-00002930: 0506 010a 0208 0108 010a 020e 017a 1953  .............z.S
-00002940: 6573 7369 6f6e 2e6c 6f61 645f 7374 7265  ession.load_stre
-00002950: 616d 5f74 6f6f 6c73 6301 0000 0000 0000  am_toolsc.......
-00002960: 0000 0000 0003 0000 0006 0000 0043 0000  .............C..
-00002970: 0073 5e00 0000 7c00 6a00 a001 a100 4400  .s^...|.j.....D.
-00002980: 5d27 5c02 7d01 7d02 7c01 7c00 6a02 a003  ]'\.}.}.|.|.j...
-00002990: a100 7600 721a 7404 a005 6401 7c01 9b00  ..v.r.t...d.|...
-000029a0: 6402 9d03 a101 0100 7105 7404 a005 6403  d.......q.t...d.
-000029b0: 7c01 9b00 9d02 a101 0100 7406 7c00 6a07  |.........t.|.j.
-000029c0: 7c01 1900 8301 7c00 6a02 7c01 3c00 7105  |.....|.j.|.<.q.
-000029d0: 6400 5300 2904 4e7a 2f53 6b69 7070 696e  d.S.).Nz/Skippin
-000029e0: 6720 6f76 6572 206d 6f6e 6f63 616c 6962  g over monocalib
-000029f0: 7261 746f 7220 6372 6561 7469 6f6e 2066  rator creation f
-00002a00: 6f72 2070 6f72 7420 7a1b 2062 6563 6175  or port z. becau
-00002a10: 7365 2069 7420 616c 7265 6164 7920 6578  se it already ex
-00002a20: 6973 7473 2e7a 204c 6f61 6469 6e67 204d  ists.z Loading M
-00002a30: 6f6e 6f63 616c 6962 7261 746f 7220 666f  onocalibrator fo
-00002a40: 7220 706f 7274 2029 0872 2e00 0000 723e  r port ).r....r>
-00002a50: 0000 0072 3200 0000 727f 0000 0072 5400  ...r2...r....rT.
-00002a60: 0000 7255 0000 0072 0a00 0000 722f 0000  ..rU...r....r/..
-00002a70: 0072 8800 0000 7225 0000 0072 2500 0000  .r....r%...r%...
-00002a80: 7226 0000 0072 8500 0000 9901 0000 7312  r&...r........s.
-00002a90: 0000 0012 010e 0104 010a 0104 ff02 0310  ................
-00002aa0: 0216 0104 f87a 1d53 6573 7369 6f6e 2e5f  .....z.Session._
-00002ab0: 6c6f 6164 5f6d 6f6e 6f63 616c 6962 7261  load_monocalibra
-00002ac0: 746f 7273 4eda 0b61 6374 6976 655f 706f  torsN..active_po
-00002ad0: 7274 6302 0000 0000 0000 0000 0000 0002  rtc.............
-00002ae0: 0000 0005 0000 0043 0000 0073 4600 0000  .......C...sF...
-00002af0: 7c01 6401 7501 720f 7400 a001 6402 7c01  |.d.u.r.t...d.|.
-00002b00: 9b00 9d02 a101 0100 7c01 7c00 5f02 7400  ........|.|._.t.
-00002b10: a001 6403 7c00 6a02 9b00 6404 9d03 a101  ..d.|.j...d.....
-00002b20: 0100 7c00 6a03 7c00 6a02 1900 a004 a100  ..|.j.|.j.......
-00002b30: 0100 6401 5300 2905 7a7e 0a20 2020 2020  ..d.S.).z~.     
-00002b40: 2020 2055 7365 6420 746f 206d 616b 6520     Used to make 
-00002b50: 7375 7265 2074 6861 7420 6f6e 6c79 2074  sure that only t
-00002b60: 6865 2061 6374 6976 6520 6361 6d65 7261  he active camera
-00002b70: 2074 6162 2069 7320 7265 6164 696e 6720   tab is reading 
-00002b80: 6672 616d 6573 2064 7572 696e 6720 7468  frames during th
-00002b90: 6520 696e 7472 696e 7369 6320 6361 6c69  e intrinsic cali
-00002ba0: 6272 6174 696f 6e20 7072 6f63 6573 730a  bration process.
-00002bb0: 2020 2020 2020 2020 4e7a 2953 6574 7469          Nz)Setti
-00002bc0: 6e67 2073 6573 7369 6f6e 2061 6374 6976  ng session activ
-00002bd0: 6520 6d6f 6e6f 6361 6c69 6272 6174 6f72  e monocalibrator
-00002be0: 2074 6f20 7a1a 4163 7469 7661 7465 2074   to z.Activate t
-00002bf0: 7261 636b 696e 6720 6f6e 2070 6f72 7420  racking on port 
-00002c00: 7a16 2061 6e64 2064 6561 6374 6976 6174  z. and deactivat
-00002c10: 6520 6f74 6865 7273 2905 7254 0000 0072  e others).rT...r
-00002c20: 5500 0000 7233 0000 0072 3200 0000 5a13  U...r3...r2...Z.
-00002c30: 7375 6273 6372 6962 655f 746f 5f73 7472  subscribe_to_str
-00002c40: 6561 6d29 0272 3b00 0000 7289 0000 0072  eam).r;...r....r
-00002c50: 2500 0000 7225 0000 0072 2600 0000 7267  %...r%...r&...rg
-00002c60: 0000 00a4 0100 0073 0e00 0000 0805 1001  .......s........
-00002c70: 0601 0401 0c01 04ff 1403 7a1f 5365 7373  ..........z.Sess
-00002c80: 696f 6e2e 6163 7469 7661 7465 5f6d 6f6e  ion.activate_mon
-00002c90: 6f63 616c 6962 7261 746f 7263 0100 0000  ocalibratorc....
-00002ca0: 0000 0000 0000 0000 0300 0000 0300 0000  ................
-00002cb0: 4300 0000 732a 0000 0074 00a0 0164 01a1  C...s*...t...d..
-00002cc0: 0101 007c 006a 02a0 03a1 0044 005d 085c  ...|.j.....D.].\
-00002cd0: 027d 017d 027c 02a0 04a1 0001 0071 0a64  .}.}.|.......q.d
-00002ce0: 0253 0029 037a 8b0a 2020 2020 2020 2020  .S.).z..        
-00002cf0: 7573 6564 2077 6865 6e20 6e6f 7420 6163  used when not ac
-00002d00: 7469 7665 6c79 206f 6e20 7468 6520 6361  tively on the ca
-00002d10: 6d65 7261 2063 616c 6962 7261 7469 6f6e  mera calibration
-00002d20: 2074 6162 0a20 2020 2020 2020 206f 7220   tab.        or 
-00002d30: 7768 656e 2073 696c 656e 6369 6e67 2061  when silencing a
-00002d40: 6c6c 2069 6e20 7072 6570 6172 6174 696f  ll in preparatio
-00002d50: 6e20 666f 7220 6163 7469 7661 7469 6e67  n for activating
-00002d60: 206f 6e6c 7920 6f6e 650a 2020 2020 2020   only one.      
-00002d70: 2020 7a25 5061 7573 696e 6720 616c 6c20    z%Pausing all 
-00002d80: 6d6f 6e6f 6361 6c69 6272 6174 6f72 206c  monocalibrator l
-00002d90: 6f6f 7069 6e67 2e2e 2e4e 2905 7254 0000  ooping...N).rT..
-00002da0: 0072 5500 0000 7232 0000 0072 3e00 0000  .rU...r2...r>...
-00002db0: 5a15 756e 7375 6273 6372 6962 655f 746f  Z.unsubscribe_to
-00002dc0: 5f73 7472 6561 6d29 0372 3b00 0000 7244  _stream).r;...rD
-00002dd0: 0000 0072 4700 0000 7225 0000 0072 2500  ...rG...r%...r%.
-00002de0: 0000 7226 0000 0072 6300 0000 b101 0000  ..r&...rc.......
-00002df0: 7308 0000 000a 0512 010a 0104 ff7a 2153  s............z!S
-00002e00: 6573 7369 6f6e 2e70 6175 7365 5f61 6c6c  ession.pause_all
-00002e10: 5f6d 6f6e 6f63 616c 6962 7261 746f 7273  _monocalibrators
-00002e20: 46da 1564 6573 7469 6e61 7469 6f6e 5f64  F..destination_d
-00002e30: 6972 6563 746f 7279 da13 7374 6f72 655f  irectory..store_
-00002e40: 706f 696e 745f 6869 7374 6f72 7963 0300  point_historyc..
-00002e50: 0000 0000 0000 0000 0000 0300 0000 0400  ................
-00002e60: 0000 4300 0000 733e 0000 0074 00a0 0164  ..C...s>...t...d
-00002e70: 01a1 0101 007c 016a 0264 0264 0264 038d  .....|.j.d.d.d..
-00002e80: 0201 0074 037c 006a 0483 017c 005f 057c  ...t.|.j...|._.|
-00002e90: 006a 056a 067c 017c 0264 048d 0201 0064  .j.j.|.|.d.....d
-00002ea0: 027c 005f 0764 0053 0029 054e 7a17 496e  .|._.d.S.).Nz.In
-00002eb0: 6974 6961 7469 6e67 2072 6563 6f72 6469  itiating recordi
-00002ec0: 6e67 2e2e 2e54 2902 da07 7061 7265 6e74  ng...T)...parent
-00002ed0: 73da 0865 7869 7374 5f6f 6b29 0172 8b00  s..exist_ok).r..
-00002ee0: 0000 2908 7254 0000 0072 5500 0000 da05  ..).rT...rU.....
-00002ef0: 6d6b 6469 7272 1700 0000 7241 0000 00da  mkdirr....rA....
-00002f00: 0e76 6964 656f 5f72 6563 6f72 6465 72da  .video_recorder.
-00002f10: 0f73 7461 7274 5f72 6563 6f72 6469 6e67  .start_recording
-00002f20: 7237 0000 0029 0372 3b00 0000 728a 0000  r7...).r;...r...
-00002f30: 0072 8b00 0000 7225 0000 0072 2500 0000  .r....r%...r%...
-00002f40: 7226 0000 0072 9000 0000 ba01 0000 730e  r&...r........s.
-00002f50: 0000 000a 030e 010c 0206 0104 0106 ff0a  ................
-00002f60: 037a 1753 6573 7369 6f6e 2e73 7461 7274  .z.Session.start
-00002f70: 5f72 6563 6f72 6469 6e67 6301 0000 0000  _recordingc.....
-00002f80: 0000 0000 0000 0001 0000 0003 0000 0043  ...............C
-00002f90: 0000 0073 6a00 0000 7400 a001 6401 a101  ...sj...t...d...
-00002fa0: 0100 7c00 6a02 a003 a100 0100 7c00 6a02  ..|.j.......|.j.
-00002fb0: 6a04 721b 7400 a001 6402 a101 0100 7405  j.r.t...d.....t.
-00002fc0: 6403 8301 0100 7c00 6a02 6a04 730e 6404  d.....|.j.j.s.d.
-00002fd0: 7c00 5f06 7400 a001 6405 a101 0100 7c00  |._.t...d.....|.
-00002fe0: 6a07 a008 a100 0100 7c00 a009 a100 7233  j.......|.....r3
-00002ff0: 7c00 6a0a a008 a100 0100 6400 5300 6400  |.j.......d.S.d.
-00003000: 5300 2906 4e7a 1553 746f 7070 696e 6720  S.).Nz.Stopping 
-00003010: 7265 636f 7264 696e 672e 2e2e 7a2e 5761  recording...z.Wa
-00003020: 6974 696e 6720 666f 7220 7669 6465 6f20  iting for video 
-00003030: 7265 636f 7264 6572 2074 6f20 7361 7665  recorder to save
-00003040: 206f 7574 2064 6174 612e 2e2e 6700 0000   out data...g...
-00003050: 0000 00e0 3f46 7a3d 5265 636f 7264 696e  ....?Fz=Recordin
-00003060: 6720 6f66 2066 7261 6d65 7320 6973 2063  g of frames is c
-00003070: 6f6d 706c 6574 652e 2e2e 7369 676e 616c  omplete...signal
-00003080: 6c69 6e67 2063 6861 6e67 6520 696e 2073  ling change in s
-00003090: 7461 7475 7329 0b72 5400 0000 7255 0000  tatus).rT...rU..
-000030a0: 0072 8f00 0000 da0e 7374 6f70 5f72 6563  .r......stop_rec
-000030b0: 6f72 6469 6e67 5a09 7265 636f 7264 696e  ordingZ.recordin
-000030c0: 6772 0600 0000 7237 0000 00da 1972 6563  gr....r7.....rec
-000030d0: 6f72 6469 6e67 5f63 6f6d 706c 6574 655f  ording_complete_
-000030e0: 7369 676e 616c 7243 0000 0072 6000 0000  signalrC...r`...
-000030f0: da15 756e 6c6f 636b 5f70 6f73 7470 726f  ..unlock_postpro
-00003100: 6365 7373 696e 6772 7000 0000 7225 0000  cessingrp...r%..
-00003110: 0072 2500 0000 7226 0000 0072 9100 0000  .r%...r&...r....
-00003120: c601 0000 7318 0000 000a 010a 0108 010a  ....s...........
-00003130: 0108 0108 fe06 040a 020a 0108 020e 0104  ................
-00003140: ff7a 1653 6573 7369 6f6e 2e73 746f 705f  .z.Session.stop_
-00003150: 7265 636f 7264 696e 6763 0100 0000 0000  recordingc......
-00003160: 0000 0000 0000 0400 0000 0800 0000 0300  ................
-00003170: 0000 7354 0000 0087 0066 0164 0164 0284  ..sT.....f.d.d..
-00003180: 087d 0174 0083 008f 177d 0288 006a 01a0  .}.t.....}...j..
-00003190: 02a1 0044 005d 087d 037c 02a0 037c 017c  ...D.].}.|...|.|
-000031a0: 03a1 0201 0071 0f57 0064 0304 0004 0083  .....q.W.d......
-000031b0: 0301 0064 0353 0031 0073 2377 0101 0001  ...d.S.1.s#w....
-000031c0: 0001 0059 0001 0064 0353 0029 047a 8243  ...Y...d.S.).z.C
-000031d0: 6861 6e67 6573 2074 6865 2063 616d 6572  hanges the camer
-000031e0: 6120 7265 736f 6c75 7469 6f6e 2074 6f20  a resolution to 
-000031f0: 7468 6520 7661 6c75 6520 696e 2074 6865  the value in the
-00003200: 2063 6f6e 6669 6775 7261 7469 6f6e 2c20   configuration, 
-00003210: 6173 0a20 2020 2020 2020 206c 6f67 2061  as.        log a
-00003220: 7320 6974 2069 7320 6e6f 7420 636f 6e66  s it is not conf
-00003230: 6967 7572 6564 2066 6f72 2074 6865 2064  igured for the d
-00003240: 6566 6175 6c74 2072 6573 6f6c 7574 696f  efault resolutio
-00003250: 6e63 0100 0000 0000 0000 0000 0000 0400  nc..............
-00003260: 0000 0a00 0000 1300 0000 73b6 0000 0088  ..........s.....
-00003270: 006a 007c 0019 007d 0188 006a 016a 0264  .j.|...}...j.j.d
-00003280: 017c 009b 009d 0219 0064 0219 007d 0288  .|.......d...}..
-00003290: 006a 037c 0019 006a 047d 037c 0264 0319  .j.|...j.}.|.d..
-000032a0: 007c 0364 0319 006b 0373 267c 0264 0419  .|.d...k.s&|.d..
-000032b0: 007c 0364 0419 006b 0372 5974 05a0 0664  .|.d...k.rYt...d
-000032c0: 057c 009b 0064 067c 0364 0364 0785 0219  .|...d.|.d.d....
-000032d0: 009b 0064 087c 0264 0364 0785 0219 009b  ...d.|.d.d......
-000032e0: 009d 06a1 0101 007c 01a0 077c 02a1 0101  .......|...|....
-000032f0: 0074 05a0 0664 097c 009b 0064 067c 0364  .t...d.|...d.|.d
-00003300: 0364 0785 0219 009b 0064 087c 0264 0364  .d.......d.|.d.d
-00003310: 0785 0219 009b 009d 06a1 0101 0064 0053  .............d.S
-00003320: 0064 0053 0029 0a4e 5a04 6361 6d5f da04  .d.S.).NZ.cam_..
-00003330: 7369 7a65 7201 0000 0072 7300 0000 7a27  sizer....rs...z'
-00003340: 4265 6769 6e6e 696e 6720 746f 2063 6861  Beginning to cha
-00003350: 6e67 6520 7265 736f 6c75 7469 6f6e 2061  nge resolution a
-00003360: 7420 706f 7274 207a 0620 6672 6f6d 2072  t port z. from r
-00003370: 5100 0000 7a04 2074 6f20 7a27 436f 6d70  Q...z. to z'Comp
-00003380: 6c65 7465 6420 6368 616e 6765 206f 6620  leted change of 
-00003390: 7265 736f 6c75 7469 6f6e 2061 7420 706f  resolution at po
-000033a0: 7274 2029 0872 2f00 0000 7228 0000 0072  rt ).r/...r(...r
-000033b0: 7400 0000 722e 0000 005a 1264 6566 6175  t...r....Z.defau
-000033c0: 6c74 5f72 6573 6f6c 7574 696f 6e72 5400  lt_resolutionrT.
-000033d0: 0000 7255 0000 005a 1163 6861 6e67 655f  ..rU...Z.change_
-000033e0: 7265 736f 6c75 7469 6f6e 2904 7244 0000  resolution).rD..
-000033f0: 0072 4500 0000 7294 0000 005a 0c64 6566  .rE...r....Z.def
-00003400: 6175 6c74 5f73 697a 6572 7000 0000 7225  ault_sizerp...r%
-00003410: 0000 0072 2600 0000 da11 6164 6a75 7374  ...r&.....adjust
-00003420: 5f72 6573 5f77 6f72 6b65 72d9 0100 0073  _res_worker....s
-00003430: 1800 0000 0a01 1601 0c01 2002 0401 2401  .......... ...$.
-00003440: 04ff 0a03 0401 2401 08ff 04fb 7a36 5365  ......$.....z6Se
-00003450: 7373 696f 6e2e 5f61 646a 7573 745f 7265  ssion._adjust_re
-00003460: 736f 6c75 7469 6f6e 732e 3c6c 6f63 616c  solutions.<local
-00003470: 733e 2e61 646a 7573 745f 7265 735f 776f  s>.adjust_res_wo
-00003480: 726b 6572 4e29 0472 0400 0000 722e 0000  rkerN).r....r...
-00003490: 0072 7f00 0000 7280 0000 0029 0472 3b00  .r....r....).r;.
-000034a0: 0000 7295 0000 0072 8100 0000 7244 0000  ..r....r....rD..
-000034b0: 0072 2500 0000 7270 0000 0072 2600 0000  .r%...rp...r&...
-000034c0: 7284 0000 00d5 0100 0073 0c00 0000 0c04  r........s......
-000034d0: 080e 0e01 0e01 02ff 22ff 7a1b 5365 7373  ........".z.Sess
-000034e0: 696f 6e2e 5f61 646a 7573 745f 7265 736f  ion._adjust_reso
-000034f0: 6c75 7469 6f6e 7363 0100 0000 0000 0000  lutionsc........
-00003500: 0000 0000 0100 0000 0400 0000 4300 0000  ............C...
-00003510: 737a 0000 007c 006a 00a0 01a1 007c 005f  sz...|.j.....|._
-00003520: 027c 006a 00a0 03a1 007c 005f 0474 057c  .|.j.....|._.t.|
-00003530: 006a 047c 006a 0283 027c 005f 067c 006a  .j.|.j...|._.|.j
-00003540: 006a 0764 0119 0064 0219 007c 006a 065f  .j.d...d...|.j._
-00003550: 0864 037c 006a 006a 0764 0119 00a0 09a1  .d.|.j.j.d......
-00003560: 0076 0072 327c 006a 006a 0764 0119 0064  .v.r2|.j.j.d...d
-00003570: 0319 007c 006a 065f 0a74 0b7c 006a 067c  ...|.j._.t.|.j.|
-00003580: 006a 0c64 048d 027c 005f 0d64 0553 0029  .j.d...|._.d.S.)
-00003590: 067a f30a 2020 2020 2020 2020 466f 6c6c  .z..        Foll
-000035a0: 6f77 696e 6720 6361 7074 7572 6520 766f  owing capture vo
-000035b0: 6c75 6d65 206f 7074 696d 697a 6174 696f  lume optimizatio
-000035c0: 6e20 7669 6120 6275 6e64 6c65 2061 646a  n via bundle adj
-000035d0: 7573 746d 656e 742c 206f 7220 616c 7465  ustment, or alte
-000035e0: 7261 7469 6f6e 0a20 2020 2020 2020 2076  ration.        v
-000035f0: 6961 2061 2074 7261 6e73 666f 726d 206f  ia a transform o
-00003600: 6620 7468 6520 6f72 6967 696e 2c20 7468  f the origin, th
-00003610: 6520 656e 7469 7265 2063 6170 7475 7265  e entire capture
-00003620: 2076 6f6c 756d 6520 6361 6e20 6265 2072   volume can be r
-00003630: 656c 6f61 6465 640a 2020 2020 2020 2020  eloaded.        
-00003640: 6672 6f6d 2074 6865 2063 6f6e 6669 6720  from the config 
-00003650: 6461 7461 2077 6974 686f 7574 206e 6565  data without nee
-00003660: 6469 6e67 2074 6f20 676f 2074 6872 6f75  ding to go throu
-00003670: 6768 2074 6865 2073 7465 7073 0a0a 2020  gh the steps..  
-00003680: 2020 2020 2020 da0e 6361 7074 7572 655f        ..capture_
-00003690: 766f 6c75 6d65 da05 7374 6167 65da 116f  volume..stage..o
-000036a0: 7269 6769 6e5f 7379 6e63 5f69 6e64 6578  rigin_sync_index
-000036b0: 2901 7238 0000 004e 290e 7228 0000 0072  ).r8...N).r(...r
-000036c0: 1400 0000 da0f 706f 696e 745f 6573 7469  ......point_esti
-000036d0: 6d61 7465 7372 4d00 0000 724e 0000 0072  matesrM...rN...r
-000036e0: 1100 0000 7296 0000 0072 7400 0000 7297  ....r....rt...r.
-000036f0: 0000 0072 7f00 0000 7298 0000 0072 1200  ...r....r....r..
-00003700: 0000 7238 0000 00da 1271 7561 6c69 7479  ..r8.....quality
-00003710: 5f63 6f6e 7472 6f6c 6c65 7272 7000 0000  _controllerrp...
-00003720: 7225 0000 0072 2500 0000 7226 0000 00da  r%...r%...r&....
-00003730: 1d6c 6f61 645f 6573 7469 6d61 7465 645f  .load_estimated_
-00003740: 6361 7074 7572 655f 766f 6c75 6d65 eb01  capture_volume..
-00003750: 0000 7316 0000 000c 070c 0110 0114 0214  ..s.............
-00003760: 010a 0102 0108 ff02 0508 010c ff7a 2553  .............z%S
-00003770: 6573 7369 6f6e 2e6c 6f61 645f 6573 7469  ession.load_esti
-00003780: 6d61 7465 645f 6361 7074 7572 655f 766f  mated_capture_vo
-00003790: 6c75 6d65 6301 0000 0000 0000 0000 0000  lumec...........
-000037a0: 0002 0000 0005 0000 0043 0000 0073 a600  .........C...s..
-000037b0: 0000 7400 7c00 6a01 6a02 7c00 6a03 8302  ..t.|.j.j.|.j...
-000037c0: 7d01 7c01 6a04 6401 6402 8d01 0100 7405  }.|.j.d.d.....t.
-000037d0: 7c00 6a01 6a02 8301 a006 a100 7c00 5f07  |.j.j.......|._.
-000037e0: 7408 7c00 6a07 7c00 6a03 8302 7c00 5f09  t.|.j.|.j...|._.
-000037f0: 740a 7c00 6a07 7c00 6a09 8302 7c00 5f0b  t.|.j.|.j...|._.
-00003800: 7c00 6a0b a00c a100 0100 740d 7c00 6a0b  |.j.......t.|.j.
-00003810: 7c00 6a0e 8302 7c00 5f0f 7410 a011 6403  |.j...|._.t...d.
-00003820: 7412 6404 1400 9b00 6405 9d03 a101 0100  t.d.....d.......
-00003830: 7c00 6a0f a013 7412 a101 0100 7c00 6a0b  |.j...t.....|.j.
-00003840: a00c a100 0100 7c00 6a01 a014 7c00 6a0b  ......|.j...|.j.
-00003850: a101 0100 6406 5300 2907 7ad7 0a20 2020  ....d.S.).z..   
-00003860: 2020 2020 2054 6869 7320 6973 2077 6865       This is whe
-00003870: 7265 2074 6865 2063 616d 6572 6120 6172  re the camera ar
-00003880: 7261 7920 3620 446f 4620 6973 2073 6574  ray 6 DoF is set
-00003890: 2e20 4d61 6e79 2c20 6d61 6e79 2074 6869  . Many, many thi
-000038a0: 6e67 7320 6172 6520 6861 7070 656e 696e  ngs are happenin
-000038b0: 670a 2020 2020 2020 2020 6865 7265 2c20  g.        here, 
-000038c0: 6275 7420 7468 6579 2061 7265 2061 6c6c  but they are all
-000038d0: 206e 6563 6573 7361 7279 2073 7465 7073   necessary steps
-000038e0: 206f 6620 7468 6520 7072 6f63 6573 7320   of the process 
-000038f0: 736f 2049 2064 6964 6e27 7420 7761 6e74  so I didn't want
-00003900: 2074 6f0a 2020 2020 2020 2020 7472 7920   to.        try 
-00003910: 746f 2065 6e63 6170 7375 6c61 7465 2061  to encapsulate a
-00003920: 6e79 2066 7572 7468 6572 0a20 2020 2020  ny further.     
-00003930: 2020 2072 1800 0000 2901 5a0e 626f 6172     r....).Z.boar
-00003940: 6473 5f73 616d 706c 6564 7a1b 5265 6d6f  ds_sampledz.Remo
-00003950: 7669 6e67 2074 6865 2077 6f72 7374 2066  ving the worst f
-00003960: 6974 7469 6e67 20e9 6400 0000 7a21 2070  itting .d...z! p
-00003970: 6572 6365 6e74 206f 6620 706f 696e 7473  ercent of points
-00003980: 2066 726f 6d20 7468 6520 6d6f 6465 6c4e   from the modelN
-00003990: 2915 720f 0000 0072 2800 0000 5a09 746f  ).r....r(...Z.to
-000039a0: 6d6c 5f70 6174 6872 2d00 0000 5a14 7374  ml_pathr-...Z.st
-000039b0: 6572 656f 5f63 616c 6962 7261 7465 5f61  ereo_calibrate_a
-000039c0: 6c6c 720d 0000 005a 1567 6574 5f62 6573  llr....Z.get_bes
-000039d0: 745f 6361 6d65 7261 5f61 7272 6179 724e  t_camera_arrayrN
-000039e0: 0000 0072 1400 0000 7299 0000 0072 1100  ...r....r....r..
-000039f0: 0000 7296 0000 00da 086f 7074 696d 697a  ..r......optimiz
-00003a00: 6572 1200 0000 7238 0000 0072 9a00 0000  er....r8...r....
-00003a10: 7254 0000 0072 5500 0000 da11 4649 4c54  rT...rU.....FILT
-00003a20: 4552 4544 5f46 5241 4354 494f 4e5a 1666  ERED_FRACTIONZ.f
-00003a30: 696c 7465 725f 706f 696e 745f 6573 7469  ilter_point_esti
-00003a40: 6d61 7465 735a 1373 6176 655f 6361 7074  matesZ.save_capt
-00003a50: 7572 655f 766f 6c75 6d65 2902 723b 0000  ure_volume).r;..
-00003a60: 005a 1073 7465 7265 6f63 616c 6962 7261  .Z.stereocalibra
-00003a70: 746f 7272 2500 0000 7225 0000 0072 2600  torr%...r%...r&.
-00003a80: 0000 da13 6573 7469 6d61 7465 5f65 7874  ....estimate_ext
-00003a90: 7269 6e73 6963 7301 0200 0073 2a00 0000  rinsics....s*...
-00003aa0: 0206 0a01 04ff 0c03 0202 0601 02ff 0402  ................
-00003ab0: 04fe 0204 0801 06ff 1004 0a01 1002 0402  ................
-00003ac0: 0e01 04ff 0c03 0a01 1202 7a1b 5365 7373  ..........z.Sess
-00003ad0: 696f 6e2e 6573 7469 6d61 7465 5f65 7874  ion.estimate_ext
-00003ae0: 7269 6e73 6963 7372 6d00 0000 2901 4629  rinsicsrm...).F)
-00003af0: 2972 1b00 0000 721c 0000 0072 1d00 0000  )r....r....r....
-00003b00: 7203 0000 0072 8700 0000 7242 0000 0072  r....r....rB...r
-00003b10: 9300 0000 7292 0000 0072 1900 0000 5a13  ....r....r....Z.
-00003b20: 6d6f 6465 5f63 6861 6e67 655f 7375 6363  mode_change_succ
-00003b30: 6573 7372 1500 0000 722a 0000 0072 4800  essr....r*...rH.
-00003b40: 0000 724b 0000 0072 5000 0000 7257 0000  ..rK...rP...rW..
-00003b50: 0072 5900 0000 7260 0000 0072 6900 0000  .rY...r`...ri...
-00003b60: da03 696e 7472 6b00 0000 726e 0000 0072  ..intrk...rn...r
-00003b70: 6100 0000 da04 626f 6f6c 7266 0000 0072  a.....boolrf...r
-00003b80: 6500 0000 7271 0000 0072 7200 0000 727a  e...rq...rr...rz
-00003b90: 0000 0072 8300 0000 7264 0000 0072 8500  ...r....rd...r..
-00003ba0: 0000 7267 0000 0072 6300 0000 7205 0000  ..rg...rc...r...
-00003bb0: 0072 9000 0000 7291 0000 0072 8400 0000  .r....r....r....
-00003bc0: 729b 0000 0072 9f00 0000 da0d 5f5f 636c  r....r......__cl
-00003bd0: 6173 7363 656c 6c5f 5f72 2500 0000 7225  asscell__r%...r%
-00003be0: 0000 0072 3c00 0000 7226 0000 0072 2700  ...r<...r&...r'.
-00003bf0: 0000 3000 0000 734a 0000 0008 0006 0106  ..0...sJ........
-00003c00: 0106 0106 0108 0212 0208 2208 1208 0708  ..........".....
-00003c10: 0b08 1d08 1e0e 100e 410e 1608 0f0e 0608  ........A.......
-00003c20: 0408 0608 0408 0408 0708 2308 2810 0b08  ..........#.(...
-00003c30: 0d02 0a04 ff02 0102 ff02 010a ff08 0c08  ................
-00003c40: 0f08 1610 1672 2700 0000 2933 da0d 7079  .....r'...)3..py
-00003c50: 7879 3364 2e6c 6f67 6765 72da 0670 7978  xy3d.logger..pyx
-00003c60: 7933 6472 5400 0000 da03 6765 7472 1b00  y3drT.....getr..
-00003c70: 0000 da0c 5079 5174 362e 5174 436f 7265  ....PyQt6.QtCore
-00003c80: 7202 0000 0072 0300 0000 5a12 636f 6e63  r....r....Z.conc
-00003c90: 7572 7265 6e74 2e66 7574 7572 6573 7204  urrent.futuresr.
-00003ca0: 0000 00da 0770 6174 686c 6962 7205 0000  .....pathlibr...
-00003cb0: 00da 0474 696d 6572 0600 0000 da04 656e  ...timer......en
-00003cc0: 756d 7207 0000 0072 0800 0000 da1f 7079  umr....r......py
-00003cd0: 7879 3364 2e74 7261 636b 6572 732e 6368  xy3d.trackers.ch
-00003ce0: 6172 7563 6f5f 7472 6163 6b65 7272 0900  aruco_trackerr..
-00003cf0: 0000 5a21 7079 7879 3364 2e63 616c 6962  ..Z!pyxy3d.calib
-00003d00: 7261 7469 6f6e 2e6d 6f6e 6f63 616c 6962  ration.monocalib
-00003d10: 7261 746f 7272 0a00 0000 5a15 7079 7879  ratorr....Z.pyxy
-00003d20: 3364 2e63 616d 6572 6173 2e63 616d 6572  3d.cameras.camer
-00003d30: 6172 0b00 0000 5a1b 7079 7879 3364 2e63  ar....Z.pyxy3d.c
-00003d40: 616d 6572 6173 2e73 796e 6368 726f 6e69  ameras.synchroni
-00003d50: 7a65 7272 0c00 0000 5a27 7079 7879 3364  zerr....Z'pyxy3d
-00003d60: 2e63 616d 6572 6173 2e63 616d 6572 615f  .cameras.camera_
-00003d70: 6172 7261 795f 696e 6974 6961 6c69 7a65  array_initialize
-00003d80: 7272 0d00 0000 5a10 7079 7879 3364 2e69  rr....Z.pyxy3d.i
-00003d90: 6e74 6572 6661 6365 720e 0000 005a 2370  nterfacer....Z#p
-00003da0: 7978 7933 642e 6361 6c69 6272 6174 696f  yxy3d.calibratio
-00003db0: 6e2e 7374 6572 656f 6361 6c69 6272 6174  n.stereocalibrat
-00003dc0: 6f72 720f 0000 005a 3170 7978 7933 642e  orr....Z1pyxy3d.
-00003dd0: 6361 6c69 6272 6174 696f 6e2e 6361 7074  calibration.capt
-00003de0: 7572 655f 766f 6c75 6d65 2e70 6f69 6e74  ure_volume.point
-00003df0: 5f65 7374 696d 6174 6573 7210 0000 005a  _estimatesr....Z
-00003e00: 3070 7978 7933 642e 6361 6c69 6272 6174  0pyxy3d.calibrat
-00003e10: 696f 6e2e 6361 7074 7572 655f 766f 6c75  ion.capture_volu
-00003e20: 6d65 2e63 6170 7475 7265 5f76 6f6c 756d  me.capture_volum
-00003e30: 6572 1100 0000 5a34 7079 7879 3364 2e63  er....Z4pyxy3d.c
-00003e40: 616c 6962 7261 7469 6f6e 2e63 6170 7475  alibration.captu
-00003e50: 7265 5f76 6f6c 756d 652e 7175 616c 6974  re_volume.qualit
-00003e60: 795f 636f 6e74 726f 6c6c 6572 7212 0000  y_controllerr...
-00003e70: 005a 1b70 7978 7933 642e 6361 6d65 7261  .Z.pyxy3d.camera
-00003e80: 732e 6361 6d65 7261 5f61 7272 6179 7213  s.camera_arrayr.
-00003e90: 0000 005a 4670 7978 7933 642e 6361 6c69  ...ZFpyxy3d.cali
-00003ea0: 6272 6174 696f 6e2e 6361 7074 7572 655f  bration.capture_
-00003eb0: 766f 6c75 6d65 2e68 656c 7065 725f 6675  volume.helper_fu
-00003ec0: 6e63 7469 6f6e 732e 6765 745f 706f 696e  nctions.get_poin
-00003ed0: 745f 6573 7469 6d61 7465 7372 1400 0000  t_estimatesr....
-00003ee0: da13 7079 7879 3364 2e63 6f6e 6669 6775  ..pyxy3d.configu
-00003ef0: 7261 746f 7272 1500 0000 5a1a 7079 7879  ratorr....Z.pyxy
-00003f00: 3364 2e63 616d 6572 6173 2e6c 6976 655f  3d.cameras.live_
-00003f10: 7374 7265 616d 7216 0000 005a 1f70 7978  streamr....Z.pyx
-00003f20: 7933 642e 7265 636f 7264 696e 672e 7669  y3d.recording.vi
-00003f30: 6465 6f5f 7265 636f 7264 6572 7217 0000  deo_recorderr...
-00003f40: 0072 7e00 0000 729e 0000 0072 1900 0000  .r~...r....r....
-00003f50: 7227 0000 0072 2500 0000 7225 0000 0072  r'...r%...r%...r
-00003f60: 2500 0000 7226 0000 00da 083c 6d6f 6475  %...r&.....<modu
-00003f70: 6c65 3e01 0000 0073 3400 0000 0801 0c02  le>....s4.......
-00003f80: 1002 0c01 0c01 0c01 1001 0c02 0c01 0c01  ................
-00003f90: 0c01 0c01 0c01 0c02 0c01 0c01 0c01 0c02  ................
-00003fa0: 0c01 0c03 0c01 0c01 0403 0401 1003 140b  ................
+00000020: 0004 0000 0040 0000 0073 4e01 0000 6400  .....@...sN...d.
+00000030: 6401 6c00 5a00 6400 6401 6c01 5a02 6502  d.l.Z.d.d.l.Z.e.
+00000040: 6a03 a004 6505 a101 5a03 6400 6402 6c06  j...e...Z.d.d.l.
+00000050: 6d07 5a07 6d08 5a08 0100 6400 6403 6c09  m.Z.m.Z...d.d.l.
+00000060: 6d0a 5a0a 0100 6400 6404 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
+00000070: 0100 6400 6405 6c0d 6d0e 5a0e 0100 6400  ..d.d.l.m.Z...d.
+00000080: 6406 6c0f 6d10 5a10 6d11 5a11 0100 6400  d.l.m.Z.m.Z...d.
+00000090: 6407 6c12 6d13 5a13 0100 6400 6408 6c14  d.l.m.Z...d.d.l.
+000000a0: 6d15 5a15 0100 6400 6409 6c16 6d17 5a17  m.Z...d.d.l.m.Z.
+000000b0: 0100 6400 640a 6c18 6d19 5a19 0100 6400  ..d.d.l.m.Z...d.
+000000c0: 640b 6c1a 6d1b 5a1b 0100 6400 640c 6c1c  d.l.m.Z...d.d.l.
+000000d0: 6d1d 5a1d 0100 6400 640d 6c1e 6d1f 5a1f  m.Z...d.d.l.m.Z.
+000000e0: 0100 6400 640e 6c20 6d21 5a21 0100 6400  ..d.d.l m!Z!..d.
+000000f0: 640f 6c22 6d23 5a23 0100 6400 6410 6c24  d.l"m#Z#..d.d.l$
+00000100: 6d25 5a25 0100 6400 6411 6c26 6d27 5a27  m%Z%..d.d.l&m'Z'
+00000110: 0100 6400 6412 6c28 6d29 5a29 0100 6400  ..d.d.l(m)Z)..d.
+00000120: 6413 6c2a 6d2b 5a2b 0100 6400 6414 6c2c  d.l*m+Z+..d.d.l,
+00000130: 6d2d 5a2d 0100 6400 6415 6c2e 6d2f 5a2f  m-Z-..d.d.l.m/Z/
+00000140: 0100 6416 5a30 6417 5a31 4700 6418 6419  ..d.Z0d.Z1G.d.d.
+00000150: 8400 6419 6510 8303 5a32 4700 641a 641b  ..d.e...Z2G.d.d.
+00000160: 8400 641b 6507 8303 5a33 4700 641c 641d  ..d.e...Z3G.d.d.
+00000170: 8400 641d 8302 5a34 6401 5300 291e e900  ..d...Z4d.S.)...
+00000180: 0000 004e 2902 da07 514f 626a 6563 74da  ...N)...QObject.
+00000190: 0a70 7971 7453 6967 6e61 6c29 01da 1254  .pyqtSignal)...T
+000001a0: 6872 6561 6450 6f6f 6c45 7865 6375 746f  hreadPoolExecuto
+000001b0: 7229 01da 0450 6174 6829 01da 0573 6c65  r)...Path)...sle
+000001c0: 6570 2902 da04 456e 756d da04 6175 746f  ep)...Enum..auto
+000001d0: 2901 da0e 4368 6172 7563 6f54 7261 636b  )...CharucoTrack
+000001e0: 6572 2901 da0e 4d6f 6e6f 4361 6c69 6272  er)...MonoCalibr
+000001f0: 6174 6f72 2901 da06 4361 6d65 7261 2901  ator)...Camera).
+00000200: da0c 5379 6e63 6872 6f6e 697a 6572 2901  ..Synchronizer).
+00000210: da16 4361 6d65 7261 4172 7261 7949 6e69  ..CameraArrayIni
+00000220: 7469 616c 697a 6572 2901 da07 5472 6163  tializer)...Trac
+00000230: 6b65 7229 01da 1053 7465 7265 6f43 616c  ker)...StereoCal
+00000240: 6962 7261 746f 7229 01da 0e50 6f69 6e74  ibrator)...Point
+00000250: 4573 7469 6d61 7465 7329 01da 0d43 6170  Estimates)...Cap
+00000260: 7475 7265 566f 6c75 6d65 2901 da11 5175  tureVolume)...Qu
+00000270: 616c 6974 7943 6f6e 7472 6f6c 6c65 7229  alityController)
+00000280: 01da 0b43 616d 6572 6141 7272 6179 2901  ...CameraArray).
+00000290: da13 6765 745f 706f 696e 745f 6573 7469  ..get_point_esti
+000002a0: 6d61 7465 7329 01da 0c43 6f6e 6669 6775  mates)...Configu
+000002b0: 7261 746f 7229 01da 0a4c 6976 6553 7472  rator)...LiveStr
+000002c0: 6561 6d29 01da 0d56 6964 656f 5265 636f  eam)...VideoReco
+000002d0: 7264 6572 e90a 0000 0067 9a99 9999 9999  rder.....g......
+000002e0: a93f 6300 0000 0000 0000 0000 0000 0000  .?c.............
+000002f0: 0000 0001 0000 0040 0000 0073 3400 0000  .......@...s4...
+00000300: 6500 5a01 6400 5a02 6401 5a03 6504 8300  e.Z.d.Z.d.Z.e...
+00000310: 5a05 6504 8300 5a06 6504 8300 5a07 6504  Z.e...Z.e...Z.e.
+00000320: 8300 5a08 6504 8300 5a09 6504 8300 5a0a  ..Z.e...Z.e...Z.
+00000330: 6402 5300 2903 da0b 5365 7373 696f 6e4d  d.S.)...SessionM
+00000340: 6f64 65fa 0120 4e29 0bda 085f 5f6e 616d  ode.. N)...__nam
+00000350: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
+00000360: 0c5f 5f71 7561 6c6e 616d 655f 5fda 075f  .__qualname__.._
+00000370: 5f64 6f63 5f5f 7208 0000 00da 0743 6861  _doc__r......Cha
+00000380: 7275 636f da14 496e 7472 696e 7369 6343  ruco..IntrinsicC
+00000390: 616c 6962 7261 7469 6f6e da14 4578 7472  alibration..Extr
+000003a0: 696e 7369 6343 616c 6962 7261 7469 6f6e  insicCalibration
+000003b0: da13 4361 7074 7572 6556 6f6c 756d 654f  ..CaptureVolumeO
+000003c0: 7269 6769 6eda 0952 6563 6f72 6469 6e67  rigin..Recording
+000003d0: da0e 506f 7374 5072 6f63 6573 7369 6e67  ..PostProcessing
+000003e0: a900 7225 0000 0072 2500 0000 fa3a 433a  ..r%...r%....:C:
+000003f0: 5c55 7365 7273 5c4d 6163 2050 7269 626c  \Users\Mac Pribl
+00000400: 655c 7265 706f 735c 7079 7879 3364 5c70  e\repos\pyxy3d\p
+00000410: 7978 7933 645c 7365 7373 696f 6e5c 7365  yxy3d\session\se
+00000420: 7373 696f 6e2e 7079 7219 0000 0026 0000  ssion.pyr....&..
+00000430: 0073 1000 0000 0800 0401 0602 0601 0601  .s..............
+00000440: 0601 0601 0a01 7219 0000 0063 0000 0000  ......r....c....
+00000450: 0000 0000 0000 0000 0000 0000 0400 0000  ................
+00000460: 0000 0000 733e 0000 0065 005a 0164 005a  ....s>...e.Z.d.Z
+00000470: 0265 0383 005a 0465 0383 005a 0565 0383  .e...Z.e...Z.e..
+00000480: 005a 0665 0383 005a 0765 0365 0883 015a  .Z.e...Z.e.e...Z
+00000490: 0964 0587 0066 0164 0364 0484 0c5a 0a87  .d...f.d.d...Z..
+000004a0: 0004 005a 0b53 0029 06da 0a51 7453 6967  ...Z.S.)...QtSig
+000004b0: 6e61 6c65 72da 0672 6574 7572 6e4e 6301  naler..returnNc.
+000004c0: 0000 0000 0000 0000 0000 0001 0000 0003  ................
+000004d0: 0000 0003 0000 0073 1200 0000 7400 7401  .......s....t.t.
+000004e0: 7c00 8302 a002 a100 0100 6400 5300 a901  |.........d.S...
+000004f0: 4e29 03da 0573 7570 6572 7227 0000 00da  N)...superr'....
+00000500: 085f 5f69 6e69 745f 5fa9 01da 0473 656c  .__init__....sel
+00000510: 66a9 01da 095f 5f63 6c61 7373 5f5f 7225  f....__class__r%
+00000520: 0000 0072 2600 0000 722b 0000 0037 0000  ...r&...r+...7..
+00000530: 0073 0200 0000 1201 7a13 5174 5369 676e  .s......z.QtSign
+00000540: 616c 6572 2e5f 5f69 6e69 745f 5f29 0272  aler.__init__).r
+00000550: 2800 0000 4e29 0c72 1b00 0000 721c 0000  (...N).r....r...
+00000560: 0072 1d00 0000 7203 0000 00da 1a73 7472  .r....r......str
+00000570: 6561 6d5f 746f 6f6c 735f 6c6f 6164 6564  eam_tools_loaded
+00000580: 5f73 6967 6e61 6cda 2073 7472 6561 6d5f  _signal. stream_
+00000590: 746f 6f6c 735f 6469 7363 6f6e 6e65 6374  tools_disconnect
+000005a0: 6564 5f73 6967 6e61 6cda 1575 6e6c 6f63  ed_signal..unloc
+000005b0: 6b5f 706f 7374 7072 6f63 6573 7369 6e67  k_postprocessing
+000005c0: da19 7265 636f 7264 696e 675f 636f 6d70  ..recording_comp
+000005d0: 6c65 7465 5f73 6967 6e61 6c72 1900 0000  lete_signalr....
+000005e0: 5a13 6d6f 6465 5f63 6861 6e67 655f 7375  Z.mode_change_su
+000005f0: 6363 6573 7372 2b00 0000 da0d 5f5f 636c  ccessr+.....__cl
+00000600: 6173 7363 656c 6c5f 5f72 2500 0000 7225  asscell__r%...r%
+00000610: 0000 0072 2e00 0000 7226 0000 0072 2700  ...r....r&...r'.
+00000620: 0000 3000 0000 730e 0000 0008 0006 0106  ..0...s.........
+00000630: 0106 0106 0108 0116 0272 2700 0000 6300  .........r'...c.
+00000640: 0000 0000 0000 0000 0000 0000 0000 0005  ................
+00000650: 0000 0040 0000 0073 1001 0000 6500 5a01  ...@...s....e.Z.
+00000660: 6400 5a02 6401 6503 6602 6402 6403 8404  d.Z.d.e.f.d.d...
+00000670: 5a04 6404 6405 8400 5a05 6406 6407 8400  Z.d.d...Z.d.d...
+00000680: 5a06 6408 6409 8400 5a07 640a 640b 8400  Z.d.d...Z.d.d...
+00000690: 5a08 640c 640d 8400 5a09 640e 640f 8400  Z.d.d...Z.d.d...
+000006a0: 5a0a 6410 650b 6602 6411 6412 8404 5a0c  Z.d.e.f.d.d...Z.
+000006b0: 6413 650d 6602 6414 6415 8404 5a0e 6416  d.e.f.d.d...Z.d.
+000006c0: 650d 6602 6417 6418 8404 5a0f 6419 641a  e.f.d.d...Z.d.d.
+000006d0: 8400 5a10 641b 6511 6602 641c 641d 8404  ..Z.d.e.f.d.d...
+000006e0: 5a12 641e 641f 8400 5a13 6420 6421 8400  Z.d.d...Z.d d!..
+000006f0: 5a14 6422 6423 8400 5a15 6424 6425 8400  Z.d"d#..Z.d$d%..
+00000700: 5a16 6426 6427 8400 5a17 6428 6429 8400  Z.d&d'..Z.d(d)..
+00000710: 5a18 642a 642b 8400 5a19 643f 642d 650d  Z.d*d+..Z.d?d-e.
+00000720: 6602 642e 642f 8405 5a1a 6430 6431 8400  f.d.d/..Z.d0d1..
+00000730: 5a1b 0932 6440 6433 651c 6434 6511 6604  Z..2d@d3e.d4e.f.
+00000740: 6435 6436 8405 5a1d 6437 6438 8400 5a1e  d5d6..Z.d7d8..Z.
+00000750: 6439 643a 8400 5a1f 643b 643c 8400 5a20  d9d:..Z.d;d<..Z 
+00000760: 643d 643e 8400 5a21 642c 5300 2941 da07  d=d>..Z!d,S.)A..
+00000770: 5365 7373 696f 6eda 0663 6f6e 6669 6763  Session..configc
+00000780: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+00000790: 0500 0000 4300 0000 73b4 0000 0074 0083  ....C...s....t..
+000007a0: 007c 005f 017c 017c 005f 027c 006a 026a  .|._.|.|._.|.j.j
+000007b0: 037c 005f 0474 057c 006a 0464 0164 0264  .|._.t.|.j.d.d.d
+000007c0: 0383 047c 005f 0669 007c 005f 0769 007c  ...|._.i.|._.i.|
+000007d0: 005f 0864 047c 005f 0964 047c 005f 0a69  ._.d.|._.d.|._.i
+000007e0: 007c 005f 0b64 007c 005f 0c7c 006a 02a0  .|._.d.|._.|.j..
+000007f0: 0da1 007c 005f 0e7c 006a 02a0 0fa1 007c  ...|._.|.j.....|
+00000800: 005f 107c 006a 02a0 11a1 007c 005f 127c  ._.|.j.....|._.|
+00000810: 006a 02a0 13a1 007c 005f 147c 006a 02a0  .j.....|._.|.j..
+00000820: 15a1 007c 005f 1664 047c 005f 177c 006a  ...|._.d.|._.|.j
+00000830: 02a0 18a1 007c 005f 1974 1a7c 006a 1983  .....|._.t.|.j..
+00000840: 017c 005f 1b74 1c6a 1d7c 005f 1e64 0053  .|._.t.j.|._.d.S
+00000850: 0029 054e 5a0b 6361 6c69 6272 6174 696f  .).NZ.calibratio
+00000860: 6e5a 0965 7874 7269 6e73 6963 7a06 7879  nZ.extrinsicz.xy
+00000870: 2e63 7376 4629 1f72 2700 0000 da0b 7174  .csvF).r'.....qt
+00000880: 5f73 6967 6e61 6c65 7272 3600 0000 da0c  _signalerr6.....
+00000890: 7365 7373 696f 6e5f 7061 7468 da04 7061  session_path..pa
+000008a0: 7468 7205 0000 00da 1865 7874 7269 6e73  thr......extrins
+000008b0: 6963 5f63 616c 6962 7261 7469 6f6e 5f78  ic_calibration_x
+000008c0: 79da 0763 616d 6572 6173 da07 7374 7265  y..cameras..stre
+000008d0: 616d 73da 1773 7472 6561 6d5f 746f 6f6c  ams..stream_tool
+000008e0: 735f 696e 5f70 726f 6365 7373 da13 7374  s_in_process..st
+000008f0: 7265 616d 5f74 6f6f 6c73 5f6c 6f61 6465  ream_tools_loade
+00000900: 64da 0f6d 6f6e 6f63 616c 6962 7261 746f  d..monocalibrato
+00000910: 7273 da15 6163 7469 7665 5f6d 6f6e 6f63  rs..active_monoc
+00000920: 616c 6962 7261 746f 725a 1167 6574 5f66  alibratorZ.get_f
+00000930: 7073 5f72 6563 6f72 6469 6e67 da0d 6670  ps_recording..fp
+00000940: 735f 7265 636f 7264 696e 675a 1d67 6574  s_recordingZ.get
+00000950: 5f66 7073 5f65 7874 7269 6e73 6963 5f63  _fps_extrinsic_c
+00000960: 616c 6962 7261 7469 6f6e da19 6670 735f  alibration..fps_
+00000970: 6578 7472 696e 7369 635f 6361 6c69 6272  extrinsic_calibr
+00000980: 6174 696f 6e5a 1d67 6574 5f66 7073 5f69  ationZ.get_fps_i
+00000990: 6e74 7269 6e73 6963 5f63 616c 6962 7261  ntrinsic_calibra
+000009a0: 7469 6f6e da19 6670 735f 696e 7472 696e  tion..fps_intrin
+000009b0: 7369 635f 6361 6c69 6272 6174 696f 6e5a  sic_calibrationZ
+000009c0: 1767 6574 5f65 7874 7269 6e73 6963 5f77  .get_extrinsic_w
+000009d0: 6169 745f 7469 6d65 5a13 7761 6974 5f74  ait_timeZ.wait_t
+000009e0: 696d 655f 6578 7472 696e 7369 635a 1767  ime_extrinsicZ.g
+000009f0: 6574 5f69 6e74 7269 6e73 6963 5f77 6169  et_intrinsic_wai
+00000a00: 745f 7469 6d65 5a13 7761 6974 5f74 696d  t_timeZ.wait_tim
+00000a10: 655f 696e 7472 696e 7369 63da 0c69 735f  e_intrinsic..is_
+00000a20: 7265 636f 7264 696e 675a 0b67 6574 5f63  recordingZ.get_c
+00000a30: 6861 7275 636f da07 6368 6172 7563 6f72  haruco..charucor
+00000a40: 0900 0000 da0f 6368 6172 7563 6f5f 7472  ......charuco_tr
+00000a50: 6163 6b65 7272 1900 0000 721f 0000 00da  ackerr....r.....
+00000a60: 046d 6f64 6529 0272 2d00 0000 7236 0000  .mode).r-...r6..
+00000a70: 0072 2500 0000 7225 0000 0072 2600 0000  .r%...r%...r&...
+00000a80: 722b 0000 003c 0000 0073 2a00 0000 0802  r+...<...s*.....
+00000a90: 0602 0a02 0204 0a01 06ff 0605 0601 0601  ................
+00000aa0: 0601 0602 0601 0c03 0c01 0c01 0c01 0c01  ................
+00000ab0: 0602 0c02 0c01 0c01 7a10 5365 7373 696f  ........z.Sessio
+00000ac0: 6e2e 5f5f 696e 6974 5f5f 6301 0000 0000  n.__init__c.....
+00000ad0: 0000 0000 0000 0005 0000 0003 0000 0043  ...............C
+00000ae0: 0000 0073 8c00 0000 7c00 6a00 a001 a100  ...s....|.j.....
+00000af0: 4400 5d09 5c02 7d01 7d02 7c02 6a02 a003  D.].\.}.}.|.j...
+00000b00: a100 0100 7105 6900 7c00 5f00 7c00 6a04  ....q.i.|._.|.j.
+00000b10: a001 a100 4400 5d08 5c02 7d01 7d03 7c03  ....D.].\.}.}.|.
+00000b20: a005 a100 0100 7117 6900 7c00 5f04 7c00  ......q.i.|._.|.
+00000b30: 6a06 a001 a100 4400 5d09 5c02 7d01 7d04  j.....D.].\.}.}.
+00000b40: 7c04 6a02 a003 a100 0100 7128 6900 7c00  |.j.......q(i.|.
+00000b50: 5f06 7c00 6a07 6a02 a003 a100 0100 6401  _.|.j.j.......d.
+00000b60: 7c00 5f07 7c00 6a08 6a09 a00a a100 0100  |._.|.j.j.......
+00000b70: 6401 5300 2902 7a72 0a20 2020 2020 2020  d.S.).zr.       
+00000b80: 2053 6875 7420 646f 776e 2074 6865 2073   Shut down the s
+00000b90: 7472 6561 6d73 2c20 636c 6f73 6520 7468  treams, close th
+00000ba0: 6520 6361 6d65 7261 2063 6170 7475 7265  e camera capture
+00000bb0: 7320 616e 6420 6465 6c65 7465 2074 6865  s and delete the
+00000bc0: 206d 6f6e 6f63 616c 6962 7261 746f 7273   monocalibrators
+00000bd0: 2061 6e64 2073 796e 6368 726f 6e69 7a65   and synchronize
+00000be0: 720a 2020 2020 2020 2020 4e29 0b72 3c00  r.        N).r<.
+00000bf0: 0000 da05 6974 656d 735a 0a73 746f 705f  ....itemsZ.stop_
+00000c00: 6576 656e 74da 0373 6574 723b 0000 00da  event..setr;....
+00000c10: 0a64 6973 636f 6e6e 6563 7472 3f00 0000  .disconnectr?...
+00000c20: da0c 7379 6e63 6872 6f6e 697a 6572 7237  ..synchronizerr7
+00000c30: 0000 0072 3100 0000 da04 656d 6974 2905  ...r1.....emit).
+00000c40: 722d 0000 00da 0470 6f72 74da 0673 7472  r-.....port..str
+00000c50: 6561 6dda 0363 616d da07 6d6f 6e6f 6361  eam..cam..monoca
+00000c60: 6c72 2500 0000 7225 0000 0072 2600 0000  lr%...r%...r&...
+00000c70: da12 6469 7363 6f6e 6e65 6374 5f63 616d  ..disconnect_cam
+00000c80: 6572 6173 6000 0000 7318 0000 0012 040c  eras`...s.......
+00000c90: 0106 0112 010a 0106 0112 010c 0106 010c  ................
+00000ca0: 0106 0110 027a 1a53 6573 7369 6f6e 2e64  .....z.Session.d
+00000cb0: 6973 636f 6e6e 6563 745f 6361 6d65 7261  isconnect_camera
+00000cc0: 7363 0100 0000 0000 0000 0000 0000 0200  sc..............
+00000cd0: 0000 0200 0000 4300 0000 731e 0000 0074  ......C...s....t
+00000ce0: 007c 006a 0183 0164 016b 0472 0b64 027d  .|.j...d.k.r.d.}
+00000cf0: 017c 0153 0064 037d 017c 0153 0029 044e  .|.S.d.}.|.S.).N
+00000d00: 7201 0000 0054 4629 02da 036c 656e 723b  r....TF)...lenr;
+00000d10: 0000 0029 0272 2d00 0000 da08 656c 6967  ...).r-.....elig
+00000d20: 6962 6c65 7225 0000 0072 2500 0000 7226  ibler%...r%...r&
+00000d30: 0000 00da 1869 735f 6361 6d65 7261 5f73  .....is_camera_s
+00000d40: 6574 7570 5f65 6c69 6769 626c 6572 0000  etup_eligibler..
+00000d50: 0073 0a00 0000 0e01 0401 0403 04ff 0401  .s..............
+00000d60: 7a20 5365 7373 696f 6e2e 6973 5f63 616d  z Session.is_cam
+00000d70: 6572 615f 7365 7475 705f 656c 6967 6962  era_setup_eligib
+00000d80: 6c65 6301 0000 0000 0000 0000 0000 0004  lec.............
+00000d90: 0000 0003 0000 0043 0000 0073 4c00 0000  .......C...sL...
+00000da0: 7c00 6a00 a001 a100 0100 7c00 6a00 a002  |.j.......|.j...
+00000db0: a100 7c00 5f03 6401 7d01 7c00 6a03 6a04  ..|._.d.}.|.j.j.
+00000dc0: a005 a100 4400 5d10 5c02 7d02 7d03 7c03  ....D.].\.}.}.|.
+00000dd0: 6a06 6400 7500 7321 7c03 6a07 6400 7500  j.d.u.s!|.j.d.u.
+00000de0: 7223 6402 7d01 7113 7c01 5300 2903 4e54  r#d.}.q.|.S.).NT
+00000df0: 4629 0872 3600 0000 da11 7265 6672 6573  F).r6.....refres
+00000e00: 685f 6672 6f6d 5f74 6f6d 6cda 1067 6574  h_from_toml..get
+00000e10: 5f63 616d 6572 615f 6172 7261 79da 0c63  _camera_array..c
+00000e20: 616d 6572 615f 6172 7261 7972 3b00 0000  amera_arrayr;...
+00000e30: 7248 0000 00da 066d 6174 7269 785a 0b64  rH.....matrixZ.d
+00000e40: 6973 746f 7274 696f 6e73 a904 722d 0000  istortions..r-..
+00000e50: 0072 5300 0000 724d 0000 0072 4f00 0000  .rS...rM...rO...
+00000e60: 7225 0000 0072 2500 0000 7226 0000 00da  r%...r%...r&....
+00000e70: 2169 735f 6578 7472 696e 7369 635f 6361  !is_extrinsic_ca
+00000e80: 6c69 6272 6174 696f 6e5f 656c 6967 6962  libration_eligib
+00000e90: 6c65 7900 0000 7310 0000 000a 020c 0104  ley...s.........
+00000ea0: 0114 0114 0104 0102 8004 027a 2953 6573  ...........z)Ses
+00000eb0: 7369 6f6e 2e69 735f 6578 7472 696e 7369  sion.is_extrinsi
+00000ec0: 635f 6361 6c69 6272 6174 696f 6e5f 656c  c_calibration_el
+00000ed0: 6967 6962 6c65 6301 0000 0000 0000 0000  igiblec.........
+00000ee0: 0000 0004 0000 0007 0000 0043 0000 0073  ...........C...s
+00000ef0: 8800 0000 7c00 6a00 a001 a100 0100 7c00  ....|.j.......|.
+00000f00: 6a00 a002 a100 7c00 5f03 6401 7d01 7404  j.....|._.d.}.t.
+00000f10: 7c00 6a03 6a05 8301 6402 6b00 7217 6403  |.j.j...d.k.r.d.
+00000f20: 7d01 7c00 6a03 6a05 a006 a100 4400 5d1c  }.|.j.j.....D.].
+00000f30: 5c02 7d02 7d03 7c03 6a07 6404 7500 732b  \.}.}.|.j.d.u.s+
+00000f40: 7c03 6a08 6404 7500 7239 6403 7d01 7409  |.j.d.u.r9d.}.t.
+00000f50: a00a 6405 7c02 9b00 6406 7c03 6a0b 9b00  ..d.|...d.|.j...
+00000f60: 9d04 a101 0100 711d 7409 a00a 6407 7c01  ......q.t...d.|.
+00000f70: 9b00 9d02 a101 0100 7c01 5300 2908 7afc  ........|.S.).z.
+00000f80: 0a20 2020 2020 2020 2069 6620 616c 6c20  .        if all 
+00000f90: 6361 6d65 7261 7320 7468 6174 2061 7265  cameras that are
+00000fa0: 206e 6f74 2069 676e 6f72 6564 2068 6176   not ignored hav
+00000fb0: 6520 726f 7461 7469 6f6e 2061 6e64 2074  e rotation and t
+00000fc0: 7261 6e73 6c61 7469 6f6e 206e 6f74 204e  ranslation not N
+00000fd0: 6f6e 650a 2020 2020 2020 2020 616e 6420  one.        and 
+00000fe0: 7468 6572 6520 6973 2061 2063 6170 7475  there is a captu
+00000ff0: 7265 2076 6f6c 756d 6520 6c6f 6164 6564  re volume loaded
+00001000: 2075 702c 2074 6865 6e20 796f 7520 6361   up, then you ca
+00001010: 6e20 6c61 756e 6368 2064 6972 6563 740a  n launch direct.
+00001020: 2020 2020 2020 2020 696e 746f 2074 6865          into the
+00001030: 2063 6170 7475 7265 2076 6f6c 756d 6520   capture volume 
+00001040: 7769 6467 6574 2072 6174 6865 7220 7468  widget rather th
+00001050: 616e 2074 6865 2065 7874 7269 6e73 6963  an the extrinsic
+00001060: 2063 616c 6962 7261 7469 6f6e 2077 6964   calibration wid
+00001070: 6765 740a 2020 2020 2020 2020 54e9 0200  get.        T...
+00001080: 0000 464e 7a30 4661 696c 6564 2063 6170  ..FNz0Failed cap
+00001090: 7475 7265 2076 6f6c 756d 6520 656c 6967  ture volume elig
+000010a0: 6962 696c 6974 7920 6475 6520 746f 2063  ibility due to c
+000010b0: 616d 6572 6120 7a02 3a20 7a45 456c 6967  amera z.: zEElig
+000010c0: 6962 6c65 2074 6f20 6c6f 6164 2063 6170  ible to load cap
+000010d0: 7475 7265 2076 6f6c 756d 653f 2028 692e  ture volume? (i.
+000010e0: 652e 2066 756c 6c79 2063 616c 6962 7261  e. fully calibra
+000010f0: 7465 6420 6578 7472 696e 7369 6373 293a  ted extrinsics):
+00001100: 2029 0c72 3600 0000 7255 0000 0072 5600   ).r6...rU...rV.
+00001110: 0000 7257 0000 0072 5200 0000 723b 0000  ..rW...rR...r;..
+00001120: 0072 4800 0000 da08 726f 7461 7469 6f6e  .rH.....rotation
+00001130: da0b 7472 616e 736c 6174 696f 6eda 066c  ..translation..l
+00001140: 6f67 6765 72da 0469 6e66 6fda 085f 5f64  ogger..info..__d
+00001150: 6963 745f 5f72 5900 0000 7225 0000 0072  ict__rY...r%...r
+00001160: 2500 0000 7226 0000 00da 1a69 735f 6361  %...r&.....is_ca
+00001170: 7074 7572 655f 766f 6c75 6d65 5f65 6c69  pture_volume_eli
+00001180: 6769 626c 6584 0000 0073 2000 0000 0a08  gible....s .....
+00001190: 0c01 0403 1001 0401 1402 1401 0401 0401  ................
+000011a0: 1001 04ff 0280 0404 0801 04ff 0404 7a22  ..............z"
+000011b0: 5365 7373 696f 6e2e 6973 5f63 6170 7475  Session.is_captu
+000011c0: 7265 5f76 6f6c 756d 655f 656c 6967 6962  re_volume_eligib
+000011d0: 6c65 6301 0000 0000 0000 0000 0000 0004  lec.............
+000011e0: 0000 0006 0000 0043 0000 0073 8c00 0000  .......C...s....
+000011f0: 7c00 6a00 a001 a100 0100 7c00 6a00 a002  |.j.......|.j...
+00001200: a100 7c00 5f03 6401 7d01 7404 7c00 6a03  ..|._.d.}.t.|.j.
+00001210: 6a05 8301 6402 6b00 7217 6403 7d01 7c00  j...d.k.r.d.}.|.
+00001220: 6a03 6a05 a006 a100 4400 5d1e 5c02 7d02  j.j.....D.].\.}.
+00001230: 7d03 7c03 6a07 6403 6b02 723b 7c03 6a08  }.|.j.d.k.r;|.j.
+00001240: 6404 7500 7330 7c03 6a09 6404 7500 723b  d.u.s0|.j.d.u.r;
+00001250: 6403 7d01 740a a00b 6405 7c02 9b00 6406  d.}.t...d.|...d.
+00001260: 9d03 a101 0100 711d 7c01 7242 6401 7d01  ......q.|.rBd.}.
+00001270: 7c01 5300 6403 7d01 7c01 5300 2907 7a44  |.S.d.}.|.S.).zD
+00001280: 0a20 2020 2020 2020 2055 7365 6420 746f  .        Used to
+00001290: 2064 6574 6572 6d69 6e65 2069 6620 7468   determine if th
+000012a0: 6520 5265 636f 7264 2042 7574 746f 6e20  e Record Button 
+000012b0: 6973 2065 6e61 626c 6564 0a0a 2020 2020  is enabled..    
+000012c0: 2020 2020 5472 5b00 0000 464e 7a34 4361      Tr[...FNz4Ca
+000012d0: 6d65 7261 2061 7272 6179 2069 7320 6e6f  mera array is no
+000012e0: 7420 6675 6c6c 7920 6361 6c69 6272 6174  t fully calibrat
+000012f0: 6564 2062 6563 6175 7365 2063 616d 6572  ed because camer
+00001300: 6120 7a11 206c 6163 6b73 2065 7874 7269  a z. lacks extri
+00001310: 6e73 6963 7329 0c72 3600 0000 7255 0000  nsics).r6...rU..
+00001320: 0072 5600 0000 7257 0000 0072 5200 0000  .rV...rW...rR...
+00001330: 723b 0000 0072 4800 0000 da06 6967 6e6f  r;...rH.....igno
+00001340: 7265 725c 0000 0072 5d00 0000 725e 0000  rer\...r]...r^..
+00001350: 0072 5f00 0000 2904 722d 0000 0072 5300  .r_...).r-...rS.
+00001360: 0000 724d 0000 00da 0663 616d 6572 6172  ..rM.....camerar
+00001370: 2500 0000 7225 0000 0072 2600 0000 da15  %...r%...r&.....
+00001380: 6973 5f72 6563 6f72 6469 6e67 5f65 6c69  is_recording_eli
+00001390: 6769 626c 65a1 0000 0073 2400 0000 0a07  gible....s$.....
+000013a0: 0c01 0403 1001 0401 1402 0a01 1401 0402  ................
+000013b0: 0401 0a01 04ff 0280 0403 0401 0404 04fe  ................
+000013c0: 0402 7a1d 5365 7373 696f 6e2e 6973 5f72  ..z.Session.is_r
+000013d0: 6563 6f72 6469 6e67 5f65 6c69 6769 626c  ecording_eligibl
+000013e0: 6563 0100 0000 0000 0000 0000 0000 0500  ec..............
+000013f0: 0000 0500 0000 4300 0000 7346 0000 0064  ......C...sF...d
+00001400: 017d 017c 006a 00a0 01a1 0044 005d 197d  .}.|.j.....D.].}
+00001410: 027c 02a0 02a1 0072 2074 037c 02a0 0464  .|.....r t.|...d
+00001420: 02a1 0183 017d 037c 0264 031b 007d 047c  .....}.|.d...}.|
+00001430: 0372 207c 04a0 05a1 0072 2064 047d 0171  .r |.....r d.}.q
+00001440: 077c 0153 0029 057a a60a 2020 2020 2020  .|.S.).z..      
+00001450: 2020 506f 7374 2070 726f 6365 7373 696e    Post processin
+00001460: 6720 6361 6e20 6f6e 6c79 2062 6520 7065  g can only be pe
+00001470: 7266 6f72 6d65 6420 6966 2072 6563 6f72  rformed if recor
+00001480: 6469 6e67 7320 286d 7034 2066 696c 6573  dings (mp4 files
+00001490: 2920 6578 6973 7420 616e 6420 6578 7472  ) exist and extr
+000014a0: 696e 7369 6373 200a 2020 2020 2020 2020  insics .        
+000014b0: 2863 6f6e 6669 672e 746f 6d6c 2920 6172  (config.toml) ar
+000014c0: 6520 6361 6c69 6272 6174 6564 2069 6e20  e calibrated in 
+000014d0: 7468 6520 2772 6563 6f72 6427 2064 6972  the 'record' dir
+000014e0: 6563 746f 7279 0a20 2020 2020 2020 2046  ectory.        F
+000014f0: 7a05 2a2e 6d70 347a 0b63 6f6e 6669 672e  z.*.mp4z.config.
+00001500: 746f 6d6c 5429 0672 3900 0000 da07 6974  tomlT).r9.....it
+00001510: 6572 6469 72da 0669 735f 6469 72da 046c  erdir..is_dir..l
+00001520: 6973 74da 0467 6c6f 62da 0665 7869 7374  ist..glob..exist
+00001530: 7329 0572 2d00 0000 7253 0000 00da 0563  s).r-...rS.....c
+00001540: 6869 6c64 5a09 6d70 345f 6669 6c65 735a  hildZ.mp4_filesZ
+00001550: 0b63 6f6e 6669 675f 6669 6c65 7225 0000  .config_filer%..
+00001560: 0072 2500 0000 7226 0000 00da 1b69 735f  .r%...r&.....is_
+00001570: 706f 7374 5f70 726f 6365 7373 696e 675f  post_processing_
+00001580: 656c 6967 6962 6c65 bf00 0000 7312 0000  eligible....s...
+00001590: 0004 060e 0108 010e 0108 010c 0104 0102  ................
+000015a0: 8004 027a 2353 6573 7369 6f6e 2e69 735f  ...z#Session.is_
+000015b0: 706f 7374 5f70 726f 6365 7373 696e 675f  post_processing_
+000015c0: 656c 6967 6962 6c65 7247 0000 0063 0200  eligiblerG...c..
+000015d0: 0000 0000 0000 0000 0000 0200 0000 0300  ................
+000015e0: 0000 4300 0000 73bc 0100 007c 017c 005f  ..C...s....|.|._
+000015f0: 007c 00a0 01a1 0001 007c 006a 0004 0074  .|.......|.j...t
+00001600: 026a 036b 0272 1f01 007c 006a 0472 1d7c  .j.k.r...|.j.r.|
+00001610: 006a 05a0 06a1 0001 007c 00a0 07a1 0001  .j.......|......
+00001620: 0064 0953 0064 0953 0004 0074 026a 086b  .d.S.d.S...t.j.k
+00001630: 0272 3501 007c 006a 0472 337c 006a 05a0  .r5..|.j.r3|.j..
+00001640: 06a1 0001 007c 00a0 07a1 0001 0064 0953  .....|.......d.S
+00001650: 0064 0953 0004 0074 026a 096b 0272 6201  .d.S...t.j.k.rb.
+00001660: 0074 0a7c 006a 0b83 017c 005f 0c7c 006a  .t.|.j...|._.|.j
+00001670: 0473 487c 00a0 0da1 0001 007c 006a 05a0  .sH|.......|.j..
+00001680: 06a1 0001 007c 00a0 07a1 0001 007c 00a0  .....|.......|..
+00001690: 0ea1 0001 007c 00a0 0f64 01a1 0101 007c  .....|...d.....|
+000016a0: 00a0 107c 006a 11a1 0101 0064 0953 0004  ...|.j.....d.S..
+000016b0: 0074 026a 126b 0272 8901 0074 0a7c 006a  .t.j.k.r...t.|.j
+000016c0: 0b83 017c 005f 0c7c 006a 0473 757c 00a0  ...|._.|.j.su|..
+000016d0: 0da1 0001 007c 00a0 07a1 0001 007c 00a0  .....|.......|..
+000016e0: 0ea1 0001 007c 00a0 0f64 01a1 0101 007c  .....|...d.....|
+000016f0: 006a 05a0 13a1 0001 0064 0953 0004 0074  .j.......d.S...t
+00001700: 026a 146b 0272 9f01 007c 006a 0472 9d7c  .j.k.r...|.j.r.|
+00001710: 00a0 07a1 0001 007c 006a 05a0 06a1 0001  .......|.j......
+00001720: 0064 0953 0064 0953 0074 026a 156b 0272  .d.S.d.S.t.j.k.r
+00001730: dc74 16a0 1764 02a1 0101 007c 006a 0473  .t...d.....|.j.s
+00001740: b474 16a0 1764 03a1 0101 007c 00a0 0da1  .t...d.....|....
+00001750: 0001 0074 16a0 1764 04a1 0101 007c 00a0  ...t...d.....|..
+00001760: 07a1 0001 0074 16a0 1764 05a1 0101 007c  .....t...d.....|
+00001770: 00a0 0f64 06a1 0101 0074 16a0 1764 07a1  ...d.....t...d..
+00001780: 0101 007c 00a0 01a1 0001 0074 16a0 1764  ...|.......t...d
+00001790: 08a1 0101 007c 006a 05a0 13a1 0001 0064  .....|.j.......d
+000017a0: 0953 0064 0953 0029 0a7a af0a 2020 2020  .S.d.S.).z..    
+000017b0: 2020 2020 5669 6120 7468 6973 206d 6574      Via this met
+000017c0: 686f 642c 2074 6865 2066 7261 6d65 2072  hod, the frame r
+000017d0: 6561 6469 6e67 2062 6568 6176 696f 7220  eading behavior 
+000017e0: 7769 6c6c 2062 6520 6368 616e 6765 6420  will be changed 
+000017f0: 6279 2074 6865 2047 5549 2e20 4966 2073  by the GUI. If s
+00001800: 6f6d 6520 7072 6f70 6572 7469 6573 2061  ome properties a
+00001810: 7265 0a20 2020 2020 2020 206e 6f74 2061  re.        not a
+00001820: 7661 696c 6162 6c65 2028 692e 652e 2073  vailable (i.e. s
+00001830: 796e 6368 726f 6e69 7a65 7229 2074 6865  ynchronizer) the
+00001840: 7920 7769 6c6c 2062 6520 6372 6561 7465  y will be create
+00001850: 640a 2020 2020 2020 2020 547a 2041 7474  d.        Tz Att
+00001860: 656d 7074 696e 6720 746f 2073 6574 2072  empting to set r
+00001870: 6563 6f72 6469 6e67 206d 6f64 657a 2e53  ecording modez.S
+00001880: 7472 6561 6d20 746f 6f6c 7320 6e6f 7420  tream tools not 
+00001890: 6c6f 6164 6564 2c20 736f 206c 6f61 6469  loaded, so loadi
+000018a0: 6e67 2074 6865 6d20 7570 2e2e 2e7a 2850  ng them up...z(P
+000018b0: 6175 7369 6e67 206d 6f6e 6f63 616c 7320  ausing monocals 
+000018c0: 746f 2065 6e74 6572 2072 6563 6f72 6469  to enter recordi
+000018d0: 6e67 206d 6f64 657a 2053 746f 7020 7472  ng modez Stop tr
+000018e0: 6163 6b69 6e67 2066 6f72 2072 6563 6f72  acking for recor
+000018f0: 6469 6e67 206d 6f64 6546 7a22 5570 6461  ding modeFz"Upda
+00001900: 7465 2073 7472 6561 6d20 6670 7320 746f  te stream fps to
+00001910: 2072 6563 6f72 6469 6e67 2066 7073 7a3e   recording fpsz>
+00001920: 5375 6273 6372 6962 6520 7379 6e63 6872  Subscribe synchr
+00001930: 6f6e 697a 6572 2074 6f20 7374 7265 616d  onizer to stream
+00001940: 7320 736f 2076 6964 656f 2072 6563 6f72  s so video recor
+00001950: 6465 7220 6361 6e20 6d61 6e61 6765 4e29  der can manageN)
+00001960: 1872 4700 0000 da12 7570 6461 7465 5f73  .rG.....update_s
+00001970: 7472 6561 6d73 5f66 7073 7219 0000 0072  treams_fpsr....r
+00001980: 1f00 0000 723e 0000 0072 4b00 0000 da18  ....r>...rK.....
+00001990: 756e 7375 6273 6372 6962 655f 6672 6f6d  unsubscribe_from
+000019a0: 5f73 7472 6561 6d73 da19 7061 7573 655f  _streams..pause_
+000019b0: 616c 6c5f 6d6f 6e6f 6361 6c69 6272 6174  all_monocalibrat
+000019c0: 6f72 7372 2400 0000 7220 0000 0072 0900  orsr$...r ...r..
+000019d0: 0000 7245 0000 0072 4600 0000 da11 6c6f  ..rE...rF.....lo
+000019e0: 6164 5f73 7472 6561 6d5f 746f 6f6c 73da  ad_stream_tools.
+000019f0: 1373 6574 5f73 7472 6561 6d73 5f63 6861  .set_streams_cha
+00001a00: 7275 636f da14 7365 745f 7374 7265 616d  ruco..set_stream
+00001a10: 735f 7472 6163 6b69 6e67 da17 6163 7469  s_tracking..acti
+00001a20: 7661 7465 5f6d 6f6e 6f63 616c 6962 7261  vate_monocalibra
+00001a30: 746f 7272 4000 0000 7221 0000 00da 1473  torr@...r!.....s
+00001a40: 7562 7363 7269 6265 5f74 6f5f 7374 7265  ubscribe_to_stre
+00001a50: 616d 7372 2200 0000 7223 0000 0072 5e00  amsr"...r#...r^.
+00001a60: 0000 725f 0000 0029 0272 2d00 0000 7247  ..r_...).r-...rG
+00001a70: 0000 0072 2500 0000 7225 0000 0072 2600  ...r%...r%...r&.
+00001a80: 0000 da08 7365 745f 6d6f 6465 cf00 0000  ....set_mode....
+00001a90: 7362 0000 0006 0508 0104 020c 0106 010a  sb..............
+00001aa0: 010c 0104 fe0c 0406 010a 010c 0104 fe0c  ................
+00001ab0: 040c 0206 0208 010a 0108 0108 010a 0110  ................
+00001ac0: 010c 020c 0206 0108 0108 0208 010a 010e  ................
+00001ad0: 020c 0206 0108 010e 0104 fe08 040a 0106  ................
+00001ae0: 010a 0108 010a 0208 010a 020a 010a 0108  ................
+00001af0: 010a 020e 0104 f17a 1053 6573 7369 6f6e  .......z.Session
+00001b00: 2e73 6574 5f6d 6f64 65da 0a66 7073 5f74  .set_mode..fps_t
+00001b10: 6172 6765 7463 0200 0000 0000 0000 0000  argetc..........
+00001b20: 0000 0200 0000 0300 0000 4300 0000 7386  ..........C...s.
+00001b30: 0000 007c 006a 0004 0074 016a 026b 0272  ...|.j...t.j.k.r
+00001b40: 0901 006e 3404 0074 016a 036b 0272 1001  ...n4..t.j.k.r..
+00001b50: 006e 2d04 0074 016a 046b 0272 2001 007c  .n-..t.j.k.r ..|
+00001b60: 017c 005f 057c 006a 06a0 077c 01a1 0101  .|._.|.j...|....
+00001b70: 006e 1d04 0074 016a 086b 0272 3001 007c  .n...t.j.k.r0..|
+00001b80: 017c 005f 097c 006a 06a0 0a7c 01a1 0101  .|._.|.j...|....
+00001b90: 006e 0d74 016a 0b6b 0272 3d7c 017c 005f  .n.t.j.k.r=|.|._
+00001ba0: 0c7c 006a 06a0 0d7c 01a1 0101 007c 00a0  .|.j...|.....|..
+00001bb0: 0ea1 0001 0064 0153 0029 027a 780a 2020  .....d.S.).zx.  
+00001bc0: 2020 2020 2020 5570 6461 7465 7320 7468        Updates th
+00001bd0: 6520 4650 5320 7573 6564 2062 7920 7468  e FPS used by th
+00001be0: 6520 6375 7272 656e 746c 7920 6163 7469  e currently acti
+00001bf0: 7665 2073 6573 7369 6f6e 206d 6f64 650a  ve session mode.
+00001c00: 2020 2020 2020 2020 5468 6973 2075 7064          This upd
+00001c10: 6174 6520 696e 636c 7564 6573 2074 6865  ate includes the
+00001c20: 2063 6f6e 6669 672e 746f 6d6c 0a20 2020   config.toml.   
+00001c30: 2020 2020 204e 290f 7247 0000 0072 1900       N).rG...r..
+00001c40: 0000 721f 0000 0072 2400 0000 7220 0000  ..r....r$...r ..
+00001c50: 0072 4300 0000 7236 0000 005a 1e73 6176  .rC...r6...Z.sav
+00001c60: 655f 6670 735f 696e 7472 696e 7369 635f  e_fps_intrinsic_
+00001c70: 6361 6c69 6272 6174 696f 6e72 2100 0000  calibrationr!...
+00001c80: 7242 0000 005a 1e73 6176 655f 6670 735f  rB...Z.save_fps_
+00001c90: 6578 7472 696e 7369 635f 6361 6c69 6272  extrinsic_calibr
+00001ca0: 6174 696f 6e72 2300 0000 7241 0000 005a  ationr#...rA...Z
+00001cb0: 1273 6176 655f 6670 735f 7265 636f 7264  .save_fps_record
+00001cc0: 696e 6772 6c00 0000 2902 722d 0000 0072  ingrl...).r-...r
+00001cd0: 7500 0000 7225 0000 0072 2500 0000 7226  u...r%...r%...r&
+00001ce0: 0000 00da 1373 6574 5f61 6374 6976 655f  .....set_active_
+00001cf0: 6d6f 6465 5f66 7073 1001 0000 731e 0000  mode_fps....s...
+00001d00: 0004 050c 0102 010c 0102 010c 0106 010e  ................
+00001d10: 010c 0106 010e 0108 0106 010c 010c 027a  ...............z
+00001d20: 1b53 6573 7369 6f6e 2e73 6574 5f61 6374  .Session.set_act
+00001d30: 6976 655f 6d6f 6465 5f66 7073 7228 0000  ive_mode_fpsr(..
+00001d40: 0063 0100 0000 0000 0000 0000 0000 0200  .c..............
+00001d50: 0000 0300 0000 4300 0000 736e 0000 0064  ......C...sn...d
+00001d60: 007d 017c 006a 0004 0074 016a 026b 0272  .}.|.j...t.j.k.r
+00001d70: 0d01 0009 007c 0153 0004 0074 016a 036b  .....|.S...t.j.k
+00001d80: 0272 1601 0009 007c 0153 0004 0074 016a  .r.....|.S...t.j
+00001d90: 046b 0272 2101 007c 006a 057d 017c 0153  .k.r!..|.j.}.|.S
+00001da0: 0004 0074 016a 066b 0272 2c01 007c 006a  ...t.j.k.r,..|.j
+00001db0: 077d 017c 0153 0074 016a 086b 0272 357c  .}.|.S.t.j.k.r5|
+00001dc0: 006a 097d 017c 0153 007c 0153 0072 2900  .j.}.|.S.|.S.r).
+00001dd0: 0000 290a 7247 0000 0072 1900 0000 721f  ..).rG...r....r.
+00001de0: 0000 0072 2400 0000 7220 0000 0072 4300  ...r$...r ...rC.
+00001df0: 0000 7221 0000 0072 4200 0000 7223 0000  ..r!...rB...r#..
+00001e00: 0072 4100 0000 2902 722d 0000 005a 0366  .rA...).r-...Z.f
+00001e10: 7073 7225 0000 0072 2500 0000 7226 0000  psr%...r%...r&..
+00001e20: 00da 1367 6574 5f61 6374 6976 655f 6d6f  ...get_active_mo
+00001e30: 6465 5f66 7073 2601 0000 7322 0000 0004  de_fps&...s"....
+00001e40: 0104 010c 0102 0104 090c f802 0104 070c  ................
+00001e50: fa06 0104 050c fc06 0104 0308 fe06 0108  ................
+00001e60: 017a 1b53 6573 7369 6f6e 2e67 6574 5f61  .z.Session.get_a
+00001e70: 6374 6976 655f 6d6f 6465 5f66 7073 6301  ctive_mode_fpsc.
+00001e80: 0000 0000 0000 0000 0000 0004 0000 0004  ................
+00001e90: 0000 0043 0000 0073 3600 0000 7c00 a000  ...C...s6...|...
+00001ea0: a100 7d01 7c01 6400 7501 7217 7c00 6a01  ..}.|.d.u.r.|.j.
+00001eb0: a002 a100 4400 5d0b 5c02 7d02 7d03 7c03  ....D.].\.}.}.|.
+00001ec0: a003 7c01 a101 0100 710d 6400 5300 6400  ..|.....q.d.S.d.
+00001ed0: 5300 7229 0000 0029 0472 7700 0000 723c  S.r)...).rw...r<
+00001ee0: 0000 0072 4800 0000 5a0e 7365 745f 6670  ...rH...Z.set_fp
+00001ef0: 735f 7461 7267 6574 2904 722d 0000 005a  s_target).r-...Z
+00001f00: 0f61 6374 6976 655f 6d6f 6465 5f66 7073  .active_mode_fps
+00001f10: 724d 0000 0072 4e00 0000 7225 0000 0072  rM...rN...r%...r
+00001f20: 2500 0000 7226 0000 0072 6c00 0000 3501  %...r&...rl...5.
+00001f30: 0000 730c 0000 0008 0108 0112 010c 0104  ..s.............
+00001f40: fe04 017a 1a53 6573 7369 6f6e 2e75 7064  ...z.Session.upd
+00001f50: 6174 655f 7374 7265 616d 735f 6670 73da  ate_streams_fps.
+00001f60: 0b74 7261 636b 696e 675f 6f6e 6302 0000  .tracking_onc...
+00001f70: 0000 0000 0000 0000 0004 0000 0004 0000  ................
+00001f80: 0043 0000 0073 2200 0000 7c00 6a00 a001  .C...s"...|.j...
+00001f90: a100 4400 5d09 5c02 7d02 7d03 7c03 a002  ..D.].\.}.}.|...
+00001fa0: 7c01 a101 0100 7105 6400 5300 7229 0000  |.....q.d.S.r)..
+00001fb0: 0029 0372 3c00 0000 7248 0000 005a 0f73  .).r<...rH...Z.s
+00001fc0: 6574 5f74 7261 636b 696e 675f 6f6e 2904  et_tracking_on).
+00001fd0: 722d 0000 0072 7800 0000 724d 0000 0072  r-...rx...rM...r
+00001fe0: 4e00 0000 7225 0000 0072 2500 0000 7226  N...r%...r%...r&
+00001ff0: 0000 0072 7100 0000 3b01 0000 7306 0000  ...rq...;...s...
+00002000: 0012 010c 0104 ff7a 1c53 6573 7369 6f6e  .......z.Session
+00002010: 2e73 6574 5f73 7472 6561 6d73 5f74 7261  .set_streams_tra
+00002020: 636b 696e 6763 0100 0000 0000 0000 0000  ckingc..........
+00002030: 0000 0300 0000 0400 0000 4300 0000 733a  ..........C...s:
+00002040: 0000 0074 00a0 0164 01a1 0101 0074 027c  ...t...d.....t.|
+00002050: 006a 0383 017c 005f 047c 006a 05a0 06a1  .j...|._.|.j....
+00002060: 0044 005d 0a5c 027d 017d 027c 02a0 077c  .D.].\.}.}.|...|
+00002070: 006a 04a1 0101 0071 1064 0053 0029 024e  .j.....q.d.S.).N
+00002080: 7a22 7570 6461 7469 6e67 2063 6861 7275  z"updating charu
+00002090: 636f 2069 6e20 6361 7365 206e 6563 6573  co in case neces
+000020a0: 7361 7279 2908 725e 0000 0072 5f00 0000  sary).r^...r_...
+000020b0: 7209 0000 0072 4500 0000 7246 0000 0072  r....rE...rF...r
+000020c0: 3c00 0000 7248 0000 005a 0e75 7064 6174  <...rH...Z.updat
+000020d0: 655f 7472 6163 6b65 7229 0372 2d00 0000  e_tracker).r-...
+000020e0: 724d 0000 0072 4e00 0000 7225 0000 0072  rM...rN...r%...r
+000020f0: 2500 0000 7226 0000 0072 7000 0000 3f01  %...r&...rp...?.
+00002100: 0000 730a 0000 000a 010c 0112 010e 0104  ..s.............
+00002110: ff7a 1b53 6573 7369 6f6e 2e73 6574 5f73  .z.Session.set_s
+00002120: 7472 6561 6d73 5f63 6861 7275 636f 6301  treams_charucoc.
+00002130: 0000 0000 0000 0000 0000 0001 0000 0003  ................
+00002140: 0000 0043 0000 0073 1800 0000 7400 a001  ...C...s....t...
+00002150: 6401 a101 0100 7c00 6a02 a003 a100 0100  d.....|.j.......
+00002160: 6400 5300 2902 4e7a 1470 6175 7369 6e67  d.S.).Nz.pausing
+00002170: 2073 796e 6368 726f 6e69 7a65 7229 0472   synchronizer).r
+00002180: 5e00 0000 725f 0000 0072 4b00 0000 726d  ^...r_...rK...rm
+00002190: 0000 0072 2c00 0000 7225 0000 0072 2500  ...r,...r%...r%.
+000021a0: 0000 7226 0000 00da 1270 6175 7365 5f73  ..r&.....pause_s
+000021b0: 796e 6368 726f 6e69 7a65 7245 0100 0073  ynchronizerE...s
+000021c0: 0400 0000 0a01 0e01 7a1a 5365 7373 696f  ........z.Sessio
+000021d0: 6e2e 7061 7573 655f 7379 6e63 6872 6f6e  n.pause_synchron
+000021e0: 697a 6572 6301 0000 0000 0000 0000 0000  izerc...........
+000021f0: 0001 0000 0003 0000 0043 0000 0073 1e00  .........C...s..
+00002200: 0000 7c00 6a00 a001 a100 0100 7c00 6a00  ..|.j.......|.j.
+00002210: a002 7c00 6a00 6a03 a101 0100 6400 5300  ..|.j.j.....d.S.
+00002220: 7229 0000 0029 0472 4b00 0000 7273 0000  r)...).rK...rs..
+00002230: 005a 0e73 6574 5f73 7472 6561 6d5f 6670  .Z.set_stream_fp
+00002240: 7372 7500 0000 722c 0000 0072 2500 0000  sru...r,...r%...
+00002250: 7225 0000 0072 2600 0000 da14 756e 7061  r%...r&.....unpa
+00002260: 7573 655f 7379 6e63 6872 6f6e 697a 6572  use_synchronizer
+00002270: 4901 0000 7304 0000 000a 0114 017a 1c53  I...s........z.S
+00002280: 6573 7369 6f6e 2e75 6e70 6175 7365 5f73  ession.unpause_s
+00002290: 796e 6368 726f 6e69 7a65 7263 0100 0000  ynchronizerc....
+000022a0: 0000 0000 0000 0000 0400 0000 0400 0000  ................
+000022b0: 4300 0000 7334 0000 0064 017d 017c 006a  C...s4...d.}.|.j
+000022c0: 006a 01a0 02a1 00a0 03a1 0044 005d 0d5c  .j.........D.].\
+000022d0: 027d 027d 037c 02a0 0464 02a1 0172 177c  .}.}.|...d...r.|
+000022e0: 0164 0337 007d 0171 0a7c 0153 0029 044e  .d.7.}.q.|.S.).N
+000022f0: 7201 0000 0072 4f00 0000 e901 0000 0029  r....rO........)
+00002300: 0572 3600 0000 da04 6469 6374 da04 636f  .r6.....dict..co
+00002310: 7079 7248 0000 00da 0a73 7461 7274 7377  pyrH.....startsw
+00002320: 6974 6829 0472 2d00 0000 da05 636f 756e  ith).r-.....coun
+00002330: 74da 036b 6579 da06 7061 7261 6d73 7225  t..key..paramsr%
+00002340: 0000 0072 2500 0000 7226 0000 00da 1b67  ...r%...r&.....g
+00002350: 6574 5f63 6f6e 6669 6775 7265 645f 6361  et_configured_ca
+00002360: 6d65 7261 5f63 6f75 6e74 4d01 0000 730c  mera_countM...s.
+00002370: 0000 0004 0118 010a 0108 0102 8004 017a  ...............z
+00002380: 2353 6573 7369 6f6e 2e67 6574 5f63 6f6e  #Session.get_con
+00002390: 6669 6775 7265 645f 6361 6d65 7261 5f63  figured_camera_c
+000023a0: 6f75 6e74 6301 0000 0000 0000 0000 0000  ountc...........
+000023b0: 0005 0000 0008 0000 0003 0000 0073 8c00  .............s..
+000023c0: 0000 8700 6601 6401 6402 8408 7d01 7400  ....f.d.d...}.t.
+000023d0: 8300 8f1e 7d02 7401 6403 7402 8302 4400  ....}.t.d.t...D.
+000023e0: 5d10 7d03 7c03 8800 6a03 a004 a100 7600  ].}.|...j.....v.
+000023f0: 7219 710f 7c02 a005 7c01 7c03 a102 0100  r.q.|...|.|.....
+00002400: 710f 5700 6404 0400 0400 8303 0100 6e08  q.W.d.........n.
+00002410: 3100 732a 7701 0100 0100 0100 5900 0100  1.s*w.......Y...
+00002420: 8800 6a06 6a07 a008 a100 a004 a100 4400  ..j.j.........D.
+00002430: 5d0c 7d04 7c04 a009 6405 a101 7243 8800  ].}.|...d...rC..
+00002440: 6a06 6a07 7c04 3d00 7137 6404 5300 2906  j.j.|.=.q7d.S.).
+00002450: 7aa3 0a20 2020 2020 2020 2043 616c 6c65  z..        Calle
+00002460: 6420 6279 206c 6f61 645f 7374 7265 616d  d by load_stream
+00002470: 7320 696e 2074 6865 2065 7665 6e74 2074  s in the event t
+00002480: 6861 7420 6e6f 2063 616d 6572 6173 2061  hat no cameras a
+00002490: 7265 2072 6574 7572 6e65 6420 6279 2074  re returned by t
+000024a0: 6865 2063 6f6e 6669 6775 7261 746f 722e  he configurator.
+000024b0: 2e2e 0a20 2020 2020 2020 2057 696c 6c20  ...        Will 
+000024c0: 706f 7075 6c61 7465 2073 656c 662e 6361  populate self.ca
+000024d0: 6d65 7261 7320 7573 696e 6720 6d75 6c74  meras using mult
+000024e0: 6970 6c65 2074 6872 6561 6473 0a20 2020  iple threads.   
+000024f0: 2020 2020 2063 0100 0000 0000 0000 0000       c..........
+00002500: 0000 0200 0000 0700 0000 1300 0000 738c  ..............s.
+00002510: 0000 007a 3774 00a0 0164 017c 009b 009d  ...z7t...d.|....
+00002520: 02a1 0101 0074 027c 0083 017d 0174 00a0  .....t.|...}.t..
+00002530: 0164 027c 009b 009d 02a1 0101 007c 0188  .d.|.........|..
+00002540: 006a 037c 003c 0088 006a 04a0 057c 01a1  .j.|.<...j...|..
+00002550: 0101 0074 00a0 0164 037c 009b 0064 049d  ...t...d.|...d..
+00002560: 03a1 0101 0074 067c 0174 0788 006a 0883  .....t.|.t...j..
+00002570: 0164 058d 0288 006a 097c 003c 0057 0064  .d.....j.|.<.W.d
+00002580: 0053 0001 0001 0001 0074 00a0 0164 067c  .S.......t...d.|
+00002590: 009b 009d 02a1 0101 0059 0064 0053 0029  .........Y.d.S.)
+000025a0: 074e 7a0c 5472 7969 6e67 2070 6f72 7420  .Nz.Trying port 
+000025b0: 7a10 5375 6363 6573 7320 6174 2070 6f72  z.Success at por
+000025c0: 7420 7a17 4c6f 6164 696e 6720 7374 7265  t z.Loading stre
+000025d0: 616d 2061 7420 706f 7274 207a 2520 7769  am at port z% wi
+000025e0: 7468 2063 6861 7275 636f 2074 7261 636b  th charuco track
+000025f0: 6572 2066 6f72 2063 616c 6962 7261 7469  er for calibrati
+00002600: 6f6e a901 5a07 7472 6163 6b65 727a 124e  on..Z.trackerz.N
+00002610: 6f20 6361 6d65 7261 2061 7420 706f 7274  o camera at port
+00002620: 2029 0a72 5e00 0000 725f 0000 0072 0b00   ).r^...r_...r..
+00002630: 0000 723b 0000 0072 3600 0000 5a0b 7361  ..r;...r6...Z.sa
+00002640: 7665 5f63 616d 6572 6172 1600 0000 7209  ve_camerar....r.
+00002650: 0000 0072 4500 0000 723c 0000 0029 0272  ...rE...r<...).r
+00002660: 4d00 0000 724f 0000 0072 2c00 0000 7225  M...rO...r,...r%
+00002670: 0000 0072 2600 0000 da07 6164 645f 6361  ...r&.....add_ca
+00002680: 6d5a 0100 0073 1c00 0000 0201 1001 0801  mZ...s..........
+00002690: 1001 0a01 0c01 0401 0a01 04ff 0203 0a01  ................
+000026a0: 12ff 0603 1601 7a26 5365 7373 696f 6e2e  ......z&Session.
+000026b0: 5f66 696e 645f 6361 6d65 7261 732e 3c6c  _find_cameras.<l
+000026c0: 6f63 616c 733e 2e61 6464 5f63 616d 7201  ocals>.add_camr.
+000026d0: 0000 004e da06 7374 6572 656f 290a 7204  ...N..stereo).r.
+000026e0: 0000 00da 0572 616e 6765 da15 4d41 585f  .....range..MAX_
+000026f0: 4341 4d45 5241 5f50 4f52 545f 4348 4543  CAMERA_PORT_CHEC
+00002700: 4b72 3b00 0000 da04 6b65 7973 da06 7375  Kr;.....keys..su
+00002710: 626d 6974 7236 0000 0072 7c00 0000 727d  bmitr6...r|...r}
+00002720: 0000 0072 7e00 0000 2905 722d 0000 0072  ...r~...).r-...r
+00002730: 8400 0000 da08 6578 6563 7574 6f72 da01  ......executor..
+00002740: 6972 8000 0000 7225 0000 0072 2c00 0000  ir....r%...r,...
+00002750: 7226 0000 00da 0d5f 6669 6e64 5f63 616d  r&....._find_cam
+00002760: 6572 6173 5401 0000 731a 0000 000c 0608  erasT...s.......
+00002770: 100e 010e 0102 020e 0202 fb1c ff14 090a  ................
+00002780: 010a 0102 8004 fe7a 1553 6573 7369 6f6e  .......z.Session
+00002790: 2e5f 6669 6e64 5f63 616d 6572 6173 6301  ._find_camerasc.
+000027a0: 0000 0000 0000 0000 0000 0003 0000 0005  ................
+000027b0: 0000 0043 0000 0073 dc00 0000 6401 7c00  ...C...s....d.|.
+000027c0: 5f00 7c00 6a01 a002 a100 7c00 5f03 7404  _.|.j.....|._.t.
+000027d0: 7c00 6a03 8301 6402 6b02 7214 7c00 a005  |.j...d.k.r.|...
+000027e0: a100 0100 7c00 6a03 a006 a100 4400 5d1e  ....|.j.....D.].
+000027f0: 5c02 7d01 7d02 7c01 7c00 6a07 a008 a100  \.}.}.|.|.j.....
+00002800: 7600 7225 7119 7409 a00a 6403 7c01 9b00  v.r%q.t...d.|...
+00002810: 9d02 a101 0100 740b 7c02 7c00 6a0c 6404  ......t.|.|.j.d.
+00002820: 8d02 7c00 6a07 7c01 3c00 7119 7c00 a00d  ..|.j.|.<.q.|...
+00002830: a100 0100 7c00 a00e a100 0100 740f 7c00  ....|.......t.|.
+00002840: 6a10 a008 a100 8301 7c00 5f11 7412 7c00  j.......|._.t.|.
+00002850: 6a07 8301 7c00 5f13 6401 7c00 5f14 6405  j...|._.d.|._.d.
+00002860: 7c00 5f00 7409 a00a 6406 a101 0100 7c00  |._.t...d.....|.
+00002870: a015 a100 0100 7c00 a016 a100 0100 7409  ......|.......t.
+00002880: a00a 6407 a101 0100 7c00 6a17 6a18 a019  ..d.....|.j.j...
+00002890: a100 0100 6408 5300 2909 7aad 0a20 2020  ....d.S.).z..   
+000028a0: 2020 2020 2043 6f6e 6e65 6374 7320 746f       Connects to
+000028b0: 2073 746f 7265 6420 6361 6d65 7261 7320   stored cameras 
+000028c0: 616e 6420 6372 6561 7465 7320 7374 7265  and creates stre
+000028d0: 616d 7320 7769 7468 2070 726f 7669 6465  ams with provide
+000028e0: 6420 7472 6163 6b69 6e67 0a20 2020 2020  d tracking.     
+000028f0: 2020 2042 6563 6175 7365 2074 6865 7365     Because these
+00002900: 2073 7472 6561 6d73 2061 7265 2061 7661   streams are ava
+00002910: 696c 6162 6c65 2c20 7468 6520 7379 6e63  ilable, the sync
+00002920: 6872 6f6e 697a 6572 2063 616e 2074 6865  hronizer can the
+00002930: 6e20 6265 2069 6e69 7469 616c 697a 6564  n be initialized
+00002940: 0a20 2020 2020 2020 2054 7201 0000 007a  .        Tr....z
+00002950: 184c 6f61 6469 6e67 2053 7472 6561 6d20  .Loading Stream 
+00002960: 666f 7220 706f 7274 2072 8300 0000 467a  for port r....Fz
+00002970: 3350 6175 7369 6e67 2073 7472 6561 6d20  3Pausing stream 
+00002980: 746f 6f6c 7320 7369 6e63 6520 6465 6661  tools since defa
+00002990: 756c 7420 6c6f 6164 7320 746f 2063 6861  ult loads to cha
+000029a0: 7275 636f 7a2d 5369 676e 616c 6c69 6e67  rucoz-Signalling
+000029b0: 2073 7563 6365 7373 6675 6c20 6c6f 6164   successful load
+000029c0: 696e 6720 6f66 2073 7472 6561 6d20 746f  ing of stream to
+000029d0: 6f6c 734e 291a 723d 0000 0072 3600 0000  olsN).r=...r6...
+000029e0: 5a0b 6765 745f 6361 6d65 7261 7372 3b00  Z.get_camerasr;.
+000029f0: 0000 7252 0000 0072 8c00 0000 7248 0000  ..rR...r....rH..
+00002a00: 0072 3c00 0000 7288 0000 0072 5e00 0000  .r<...r....r^...
+00002a10: 725f 0000 0072 1600 0000 7246 0000 00da  r_...r....rF....
+00002a20: 135f 6164 6a75 7374 5f72 6573 6f6c 7574  ._adjust_resolut
+00002a30: 696f 6e73 da15 5f6c 6f61 645f 6d6f 6e6f  ions.._load_mono
+00002a40: 6361 6c69 6272 6174 6f72 73da 036d 696e  calibrators..min
+00002a50: 723f 0000 0072 4000 0000 720c 0000 0072  r?...r@...r....r
+00002a60: 4b00 0000 723e 0000 0072 6e00 0000 7279  K...r>...rn...ry
+00002a70: 0000 0072 3700 0000 7230 0000 0072 4c00  ...r7...r0...rL.
+00002a80: 0000 a903 722d 0000 0072 4d00 0000 724f  ....r-...rM...rO
+00002a90: 0000 0072 2500 0000 7225 0000 0072 2600  ...r%...r%...r&.
+00002aa0: 0000 726f 0000 0077 0100 0073 2c00 0000  ..ro...w...s,...
+00002ab0: 0605 0c02 0e02 0801 1202 0e01 0201 1002  ................
+00002ac0: 1601 0802 0801 1003 0202 0401 06ff 0605  ................
+00002ad0: 0601 0a02 0801 0801 0a02 1001 7a19 5365  ............z.Se
+00002ae0: 7373 696f 6e2e 6c6f 6164 5f73 7472 6561  ssion.load_strea
+00002af0: 6d5f 746f 6f6c 7363 0100 0000 0000 0000  m_toolsc........
+00002b00: 0000 0000 0300 0000 0600 0000 4300 0000  ............C...
+00002b10: 735e 0000 007c 006a 00a0 01a1 0044 005d  s^...|.j.....D.]
+00002b20: 275c 027d 017d 027c 017c 006a 02a0 03a1  '\.}.}.|.|.j....
+00002b30: 0076 0072 1a74 04a0 0564 017c 019b 0064  .v.r.t...d.|...d
+00002b40: 029d 03a1 0101 0071 0574 04a0 0564 037c  .......q.t...d.|
+00002b50: 019b 009d 02a1 0101 0074 067c 006a 077c  .........t.|.j.|
+00002b60: 0119 0083 017c 006a 027c 013c 0071 0564  .....|.j.|.<.q.d
+00002b70: 0053 0029 044e 7a2f 536b 6970 7069 6e67  .S.).Nz/Skipping
+00002b80: 206f 7665 7220 6d6f 6e6f 6361 6c69 6272   over monocalibr
+00002b90: 6174 6f72 2063 7265 6174 696f 6e20 666f  ator creation fo
+00002ba0: 7220 706f 7274 207a 1b20 6265 6361 7573  r port z. becaus
+00002bb0: 6520 6974 2061 6c72 6561 6479 2065 7869  e it already exi
+00002bc0: 7374 732e 7a20 4c6f 6164 696e 6720 4d6f  sts.z Loading Mo
+00002bd0: 6e6f 6361 6c69 6272 6174 6f72 2066 6f72  nocalibrator for
+00002be0: 2070 6f72 7420 2908 723b 0000 0072 4800   port ).r;...rH.
+00002bf0: 0000 723f 0000 0072 8800 0000 725e 0000  ..r?...r....r^..
+00002c00: 0072 5f00 0000 720a 0000 0072 3c00 0000  .r_...r....r<...
+00002c10: 7290 0000 0072 2500 0000 7225 0000 0072  r....r%...r%...r
+00002c20: 2600 0000 728e 0000 009f 0100 0073 1200  &...r........s..
+00002c30: 0000 1201 0e01 0401 0a01 04ff 0203 1002  ................
+00002c40: 1601 04f8 7a1d 5365 7373 696f 6e2e 5f6c  ....z.Session._l
+00002c50: 6f61 645f 6d6f 6e6f 6361 6c69 6272 6174  oad_monocalibrat
+00002c60: 6f72 734e da0b 6163 7469 7665 5f70 6f72  orsN..active_por
+00002c70: 7463 0200 0000 0000 0000 0000 0000 0200  tc..............
+00002c80: 0000 0500 0000 4300 0000 7346 0000 007c  ......C...sF...|
+00002c90: 0164 0175 0172 0f74 00a0 0164 027c 019b  .d.u.r.t...d.|..
+00002ca0: 009d 02a1 0101 007c 017c 005f 0274 00a0  .......|.|._.t..
+00002cb0: 0164 037c 006a 029b 0064 049d 03a1 0101  .d.|.j...d......
+00002cc0: 007c 006a 037c 006a 0219 00a0 04a1 0001  .|.j.|.j........
+00002cd0: 0064 0153 0029 057a 7e0a 2020 2020 2020  .d.S.).z~.      
+00002ce0: 2020 5573 6564 2074 6f20 6d61 6b65 2073    Used to make s
+00002cf0: 7572 6520 7468 6174 206f 6e6c 7920 7468  ure that only th
+00002d00: 6520 6163 7469 7665 2063 616d 6572 6120  e active camera 
+00002d10: 7461 6220 6973 2072 6561 6469 6e67 2066  tab is reading f
+00002d20: 7261 6d65 7320 6475 7269 6e67 2074 6865  rames during the
+00002d30: 2069 6e74 7269 6e73 6963 2063 616c 6962   intrinsic calib
+00002d40: 7261 7469 6f6e 2070 726f 6365 7373 0a20  ration process. 
+00002d50: 2020 2020 2020 204e 7a29 5365 7474 696e         Nz)Settin
+00002d60: 6720 7365 7373 696f 6e20 6163 7469 7665  g session active
+00002d70: 206d 6f6e 6f63 616c 6962 7261 746f 7220   monocalibrator 
+00002d80: 746f 207a 1a41 6374 6976 6174 6520 7472  to z.Activate tr
+00002d90: 6163 6b69 6e67 206f 6e20 706f 7274 207a  acking on port z
+00002da0: 1620 616e 6420 6465 6163 7469 7661 7465  . and deactivate
+00002db0: 206f 7468 6572 7329 0572 5e00 0000 725f   others).r^...r_
+00002dc0: 0000 0072 4000 0000 723f 0000 005a 1373  ...r@...r?...Z.s
+00002dd0: 7562 7363 7269 6265 5f74 6f5f 7374 7265  ubscribe_to_stre
+00002de0: 616d 2902 722d 0000 0072 9100 0000 7225  am).r-...r....r%
+00002df0: 0000 0072 2500 0000 7226 0000 0072 7200  ...r%...r&...rr.
+00002e00: 0000 aa01 0000 730e 0000 0008 0510 0106  ......s.........
+00002e10: 0104 010c 0104 ff14 037a 1f53 6573 7369  .........z.Sessi
+00002e20: 6f6e 2e61 6374 6976 6174 655f 6d6f 6e6f  on.activate_mono
+00002e30: 6361 6c69 6272 6174 6f72 6301 0000 0000  calibratorc.....
+00002e40: 0000 0000 0000 0003 0000 0003 0000 0043  ...............C
+00002e50: 0000 0073 2a00 0000 7400 a001 6401 a101  ...s*...t...d...
+00002e60: 0100 7c00 6a02 a003 a100 4400 5d08 5c02  ..|.j.....D.].\.
+00002e70: 7d01 7d02 7c02 a004 a100 0100 710a 6402  }.}.|.......q.d.
+00002e80: 5300 2903 7a8b 0a20 2020 2020 2020 2075  S.).z..        u
+00002e90: 7365 6420 7768 656e 206e 6f74 2061 6374  sed when not act
+00002ea0: 6976 656c 7920 6f6e 2074 6865 2063 616d  ively on the cam
+00002eb0: 6572 6120 6361 6c69 6272 6174 696f 6e20  era calibration 
+00002ec0: 7461 620a 2020 2020 2020 2020 6f72 2077  tab.        or w
+00002ed0: 6865 6e20 7369 6c65 6e63 696e 6720 616c  hen silencing al
+00002ee0: 6c20 696e 2070 7265 7061 7261 7469 6f6e  l in preparation
+00002ef0: 2066 6f72 2061 6374 6976 6174 696e 6720   for activating 
+00002f00: 6f6e 6c79 206f 6e65 0a20 2020 2020 2020  only one.       
+00002f10: 207a 2550 6175 7369 6e67 2061 6c6c 206d   z%Pausing all m
+00002f20: 6f6e 6f63 616c 6962 7261 746f 7220 6c6f  onocalibrator lo
+00002f30: 6f70 696e 672e 2e2e 4e29 0572 5e00 0000  oping...N).r^...
+00002f40: 725f 0000 0072 3f00 0000 7248 0000 005a  r_...r?...rH...Z
+00002f50: 1575 6e73 7562 7363 7269 6265 5f74 6f5f  .unsubscribe_to_
+00002f60: 7374 7265 616d 2903 722d 0000 0072 4d00  stream).r-...rM.
+00002f70: 0000 7250 0000 0072 2500 0000 7225 0000  ..rP...r%...r%..
+00002f80: 0072 2600 0000 726e 0000 00b7 0100 0073  .r&...rn.......s
+00002f90: 0800 0000 0a05 1201 0a01 04ff 7a21 5365  ............z!Se
+00002fa0: 7373 696f 6e2e 7061 7573 655f 616c 6c5f  ssion.pause_all_
+00002fb0: 6d6f 6e6f 6361 6c69 6272 6174 6f72 7346  monocalibratorsF
+00002fc0: da15 6465 7374 696e 6174 696f 6e5f 6469  ..destination_di
+00002fd0: 7265 6374 6f72 79da 1373 746f 7265 5f70  rectory..store_p
+00002fe0: 6f69 6e74 5f68 6973 746f 7279 6303 0000  oint_historyc...
+00002ff0: 0000 0000 0000 0000 0003 0000 0004 0000  ................
+00003000: 0043 0000 0073 3e00 0000 7400 a001 6401  .C...s>...t...d.
+00003010: a101 0100 7c01 6a02 6402 6402 6403 8d02  ....|.j.d.d.d...
+00003020: 0100 7403 7c00 6a04 8301 7c00 5f05 7c00  ..t.|.j...|._.|.
+00003030: 6a05 6a06 7c01 7c02 6404 8d02 0100 6402  j.j.|.|.d.....d.
+00003040: 7c00 5f07 6400 5300 2905 4e7a 1749 6e69  |._.d.S.).Nz.Ini
+00003050: 7469 6174 696e 6720 7265 636f 7264 696e  tiating recordin
+00003060: 672e 2e2e 5429 02da 0770 6172 656e 7473  g...T)...parents
+00003070: da08 6578 6973 745f 6f6b 2901 7293 0000  ..exist_ok).r...
+00003080: 0029 0872 5e00 0000 725f 0000 00da 056d  .).r^...r_.....m
+00003090: 6b64 6972 7217 0000 0072 4b00 0000 da0e  kdirr....rK.....
+000030a0: 7669 6465 6f5f 7265 636f 7264 6572 da0f  video_recorder..
+000030b0: 7374 6172 745f 7265 636f 7264 696e 6772  start_recordingr
+000030c0: 4400 0000 2903 722d 0000 0072 9200 0000  D...).r-...r....
+000030d0: 7293 0000 0072 2500 0000 7225 0000 0072  r....r%...r%...r
+000030e0: 2600 0000 7298 0000 00c0 0100 0073 0e00  &...r........s..
+000030f0: 0000 0a03 0e01 0c02 0601 0401 06ff 0a03  ................
+00003100: 7a17 5365 7373 696f 6e2e 7374 6172 745f  z.Session.start_
+00003110: 7265 636f 7264 696e 6763 0100 0000 0000  recordingc......
+00003120: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
+00003130: 0000 736e 0000 0074 00a0 0164 01a1 0101  ..sn...t...d....
+00003140: 007c 006a 02a0 03a1 0001 007c 006a 026a  .|.j.......|.j.j
+00003150: 0472 1b74 00a0 0164 02a1 0101 0074 0564  .r.t...d.....t.d
+00003160: 0383 0101 007c 006a 026a 0473 0e64 047c  .....|.j.j.s.d.|
+00003170: 005f 0674 00a0 0164 05a1 0101 007c 006a  ._.t...d.....|.j
+00003180: 076a 08a0 09a1 0001 007c 00a0 0aa1 0072  .j.......|.....r
+00003190: 357c 006a 076a 0ba0 09a1 0001 0064 0053  5|.j.j.......d.S
+000031a0: 0064 0053 0029 064e 7a15 5374 6f70 7069  .d.S.).Nz.Stoppi
+000031b0: 6e67 2072 6563 6f72 6469 6e67 2e2e 2e7a  ng recording...z
+000031c0: 2e57 6169 7469 6e67 2066 6f72 2076 6964  .Waiting for vid
+000031d0: 656f 2072 6563 6f72 6465 7220 746f 2073  eo recorder to s
+000031e0: 6176 6520 6f75 7420 6461 7461 2e2e 2e67  ave out data...g
+000031f0: 0000 0000 0000 e03f 467a 3d52 6563 6f72  .......?Fz=Recor
+00003200: 6469 6e67 206f 6620 6672 616d 6573 2069  ding of frames i
+00003210: 7320 636f 6d70 6c65 7465 2e2e 2e73 6967  s complete...sig
+00003220: 6e61 6c6c 696e 6720 6368 616e 6765 2069  nalling change i
+00003230: 6e20 7374 6174 7573 290c 725e 0000 0072  n status).r^...r
+00003240: 5f00 0000 7297 0000 00da 0e73 746f 705f  _...r......stop_
+00003250: 7265 636f 7264 696e 675a 0972 6563 6f72  recordingZ.recor
+00003260: 6469 6e67 7206 0000 0072 4400 0000 7237  dingr....rD...r7
+00003270: 0000 0072 3300 0000 724c 0000 0072 6b00  ...r3...rL...rk.
+00003280: 0000 7232 0000 0072 2c00 0000 7225 0000  ..r2...r,...r%..
+00003290: 0072 2500 0000 7226 0000 0072 9900 0000  .r%...r&...r....
+000032a0: cc01 0000 7318 0000 000a 010a 0108 010a  ....s...........
+000032b0: 0108 0108 fe06 040a 020c 0108 0210 0104  ................
+000032c0: ff7a 1653 6573 7369 6f6e 2e73 746f 705f  .z.Session.stop_
+000032d0: 7265 636f 7264 696e 6763 0100 0000 0000  recordingc......
+000032e0: 0000 0000 0000 0400 0000 0800 0000 0300  ................
+000032f0: 0000 7354 0000 0087 0066 0164 0164 0284  ..sT.....f.d.d..
+00003300: 087d 0174 0083 008f 177d 0288 006a 01a0  .}.t.....}...j..
+00003310: 02a1 0044 005d 087d 037c 02a0 037c 017c  ...D.].}.|...|.|
+00003320: 03a1 0201 0071 0f57 0064 0304 0004 0083  .....q.W.d......
+00003330: 0301 0064 0353 0031 0073 2377 0101 0001  ...d.S.1.s#w....
+00003340: 0001 0059 0001 0064 0353 0029 047a 8243  ...Y...d.S.).z.C
+00003350: 6861 6e67 6573 2074 6865 2063 616d 6572  hanges the camer
+00003360: 6120 7265 736f 6c75 7469 6f6e 2074 6f20  a resolution to 
+00003370: 7468 6520 7661 6c75 6520 696e 2074 6865  the value in the
+00003380: 2063 6f6e 6669 6775 7261 7469 6f6e 2c20   configuration, 
+00003390: 6173 0a20 2020 2020 2020 206c 6f67 2061  as.        log a
+000033a0: 7320 6974 2069 7320 6e6f 7420 636f 6e66  s it is not conf
+000033b0: 6967 7572 6564 2066 6f72 2074 6865 2064  igured for the d
+000033c0: 6566 6175 6c74 2072 6573 6f6c 7574 696f  efault resolutio
+000033d0: 6e63 0100 0000 0000 0000 0000 0000 0400  nc..............
+000033e0: 0000 0a00 0000 1300 0000 73b6 0000 0088  ..........s.....
+000033f0: 006a 007c 0019 007d 0188 006a 016a 0264  .j.|...}...j.j.d
+00003400: 017c 009b 009d 0219 0064 0219 007d 0288  .|.......d...}..
+00003410: 006a 037c 0019 006a 047d 037c 0264 0319  .j.|...j.}.|.d..
+00003420: 007c 0364 0319 006b 0373 267c 0264 0419  .|.d...k.s&|.d..
+00003430: 007c 0364 0419 006b 0372 5974 05a0 0664  .|.d...k.rYt...d
+00003440: 057c 009b 0064 067c 0364 0364 0785 0219  .|...d.|.d.d....
+00003450: 009b 0064 087c 0264 0364 0785 0219 009b  ...d.|.d.d......
+00003460: 009d 06a1 0101 007c 01a0 077c 02a1 0101  .......|...|....
+00003470: 0074 05a0 0664 097c 009b 0064 067c 0364  .t...d.|...d.|.d
+00003480: 0364 0785 0219 009b 0064 087c 0264 0364  .d.......d.|.d.d
+00003490: 0785 0219 009b 009d 06a1 0101 0064 0053  .............d.S
+000034a0: 0064 0053 0029 0a4e 5a04 6361 6d5f da04  .d.S.).NZ.cam_..
+000034b0: 7369 7a65 7201 0000 0072 7b00 0000 7a27  sizer....r{...z'
+000034c0: 4265 6769 6e6e 696e 6720 746f 2063 6861  Beginning to cha
+000034d0: 6e67 6520 7265 736f 6c75 7469 6f6e 2061  nge resolution a
+000034e0: 7420 706f 7274 207a 0620 6672 6f6d 2072  t port z. from r
+000034f0: 5b00 0000 7a04 2074 6f20 7a27 436f 6d70  [...z. to z'Comp
+00003500: 6c65 7465 6420 6368 616e 6765 206f 6620  leted change of 
+00003510: 7265 736f 6c75 7469 6f6e 2061 7420 706f  resolution at po
+00003520: 7274 2029 0872 3c00 0000 7236 0000 0072  rt ).r<...r6...r
+00003530: 7c00 0000 723b 0000 005a 1264 6566 6175  |...r;...Z.defau
+00003540: 6c74 5f72 6573 6f6c 7574 696f 6e72 5e00  lt_resolutionr^.
+00003550: 0000 725f 0000 005a 1163 6861 6e67 655f  ..r_...Z.change_
+00003560: 7265 736f 6c75 7469 6f6e 2904 724d 0000  resolution).rM..
+00003570: 0072 4e00 0000 729a 0000 005a 0c64 6566  .rN...r....Z.def
+00003580: 6175 6c74 5f73 697a 6572 2c00 0000 7225  ault_sizer,...r%
+00003590: 0000 0072 2600 0000 da11 6164 6a75 7374  ...r&.....adjust
+000035a0: 5f72 6573 5f77 6f72 6b65 72df 0100 0073  _res_worker....s
+000035b0: 1800 0000 0a01 1601 0c01 2002 0401 2401  .......... ...$.
+000035c0: 04ff 0a03 0401 2401 08ff 04fb 7a36 5365  ......$.....z6Se
+000035d0: 7373 696f 6e2e 5f61 646a 7573 745f 7265  ssion._adjust_re
+000035e0: 736f 6c75 7469 6f6e 732e 3c6c 6f63 616c  solutions.<local
+000035f0: 733e 2e61 646a 7573 745f 7265 735f 776f  s>.adjust_res_wo
+00003600: 726b 6572 4e29 0472 0400 0000 723b 0000  rkerN).r....r;..
+00003610: 0072 8800 0000 7289 0000 0029 0472 2d00  .r....r....).r-.
+00003620: 0000 729b 0000 0072 8a00 0000 724d 0000  ..r....r....rM..
+00003630: 0072 2500 0000 722c 0000 0072 2600 0000  .r%...r,...r&...
+00003640: 728d 0000 00db 0100 0073 0c00 0000 0c04  r........s......
+00003650: 080e 0e01 0e01 02ff 22ff 7a1b 5365 7373  ........".z.Sess
+00003660: 696f 6e2e 5f61 646a 7573 745f 7265 736f  ion._adjust_reso
+00003670: 6c75 7469 6f6e 7363 0100 0000 0000 0000  lutionsc........
+00003680: 0000 0000 0100 0000 0400 0000 4300 0000  ............C...
+00003690: 737a 0000 007c 006a 00a0 01a1 007c 005f  sz...|.j.....|._
+000036a0: 027c 006a 00a0 03a1 007c 005f 0474 057c  .|.j.....|._.t.|
+000036b0: 006a 047c 006a 0283 027c 005f 067c 006a  .j.|.j...|._.|.j
+000036c0: 006a 0764 0119 0064 0219 007c 006a 065f  .j.d...d...|.j._
+000036d0: 0864 037c 006a 006a 0764 0119 00a0 09a1  .d.|.j.j.d......
+000036e0: 0076 0072 327c 006a 006a 0764 0119 0064  .v.r2|.j.j.d...d
+000036f0: 0319 007c 006a 065f 0a74 0b7c 006a 067c  ...|.j._.t.|.j.|
+00003700: 006a 0c64 048d 027c 005f 0d64 0553 0029  .j.d...|._.d.S.)
+00003710: 067a f30a 2020 2020 2020 2020 466f 6c6c  .z..        Foll
+00003720: 6f77 696e 6720 6361 7074 7572 6520 766f  owing capture vo
+00003730: 6c75 6d65 206f 7074 696d 697a 6174 696f  lume optimizatio
+00003740: 6e20 7669 6120 6275 6e64 6c65 2061 646a  n via bundle adj
+00003750: 7573 746d 656e 742c 206f 7220 616c 7465  ustment, or alte
+00003760: 7261 7469 6f6e 0a20 2020 2020 2020 2076  ration.        v
+00003770: 6961 2061 2074 7261 6e73 666f 726d 206f  ia a transform o
+00003780: 6620 7468 6520 6f72 6967 696e 2c20 7468  f the origin, th
+00003790: 6520 656e 7469 7265 2063 6170 7475 7265  e entire capture
+000037a0: 2076 6f6c 756d 6520 6361 6e20 6265 2072   volume can be r
+000037b0: 656c 6f61 6465 640a 2020 2020 2020 2020  eloaded.        
+000037c0: 6672 6f6d 2074 6865 2063 6f6e 6669 6720  from the config 
+000037d0: 6461 7461 2077 6974 686f 7574 206e 6565  data without nee
+000037e0: 6469 6e67 2074 6f20 676f 2074 6872 6f75  ding to go throu
+000037f0: 6768 2074 6865 2073 7465 7073 0a0a 2020  gh the steps..  
+00003800: 2020 2020 2020 da0e 6361 7074 7572 655f        ..capture_
+00003810: 766f 6c75 6d65 da05 7374 6167 65da 116f  volume..stage..o
+00003820: 7269 6769 6e5f 7379 6e63 5f69 6e64 6578  rigin_sync_index
+00003830: 2901 7245 0000 004e 290e 7236 0000 0072  ).rE...N).r6...r
+00003840: 1400 0000 da0f 706f 696e 745f 6573 7469  ......point_esti
+00003850: 6d61 7465 7372 5600 0000 7257 0000 0072  matesrV...rW...r
+00003860: 1100 0000 729c 0000 0072 7c00 0000 729d  ....r....r|...r.
+00003870: 0000 0072 8800 0000 729e 0000 0072 1200  ...r....r....r..
+00003880: 0000 7245 0000 00da 1271 7561 6c69 7479  ..rE.....quality
+00003890: 5f63 6f6e 7472 6f6c 6c65 7272 2c00 0000  _controllerr,...
+000038a0: 7225 0000 0072 2500 0000 7226 0000 00da  r%...r%...r&....
+000038b0: 1d6c 6f61 645f 6573 7469 6d61 7465 645f  .load_estimated_
+000038c0: 6361 7074 7572 655f 766f 6c75 6d65 f101  capture_volume..
+000038d0: 0000 7316 0000 000c 070c 0110 0114 0214  ..s.............
+000038e0: 010a 0102 0108 ff02 0508 010c ff7a 2553  .............z%S
+000038f0: 6573 7369 6f6e 2e6c 6f61 645f 6573 7469  ession.load_esti
+00003900: 6d61 7465 645f 6361 7074 7572 655f 766f  mated_capture_vo
+00003910: 6c75 6d65 6301 0000 0000 0000 0000 0000  lumec...........
+00003920: 0002 0000 0005 0000 0043 0000 0073 a600  .........C...s..
+00003930: 0000 7400 7c00 6a01 6a02 7c00 6a03 8302  ..t.|.j.j.|.j...
+00003940: 7d01 7c01 6a04 6401 6402 8d01 0100 7405  }.|.j.d.d.....t.
+00003950: 7c00 6a01 6a02 8301 a006 a100 7c00 5f07  |.j.j.......|._.
+00003960: 7408 7c00 6a07 7c00 6a03 8302 7c00 5f09  t.|.j.|.j...|._.
+00003970: 740a 7c00 6a07 7c00 6a09 8302 7c00 5f0b  t.|.j.|.j...|._.
+00003980: 7c00 6a0b a00c a100 0100 740d 7c00 6a0b  |.j.......t.|.j.
+00003990: 7c00 6a0e 8302 7c00 5f0f 7410 a011 6403  |.j...|._.t...d.
+000039a0: 7412 6404 1400 9b00 6405 9d03 a101 0100  t.d.....d.......
+000039b0: 7c00 6a0f a013 7412 a101 0100 7c00 6a0b  |.j...t.....|.j.
+000039c0: a00c a100 0100 7c00 6a01 a014 7c00 6a0b  ......|.j...|.j.
+000039d0: a101 0100 6406 5300 2907 7ad7 0a20 2020  ....d.S.).z..   
+000039e0: 2020 2020 2054 6869 7320 6973 2077 6865       This is whe
+000039f0: 7265 2074 6865 2063 616d 6572 6120 6172  re the camera ar
+00003a00: 7261 7920 3620 446f 4620 6973 2073 6574  ray 6 DoF is set
+00003a10: 2e20 4d61 6e79 2c20 6d61 6e79 2074 6869  . Many, many thi
+00003a20: 6e67 7320 6172 6520 6861 7070 656e 696e  ngs are happenin
+00003a30: 670a 2020 2020 2020 2020 6865 7265 2c20  g.        here, 
+00003a40: 6275 7420 7468 6579 2061 7265 2061 6c6c  but they are all
+00003a50: 206e 6563 6573 7361 7279 2073 7465 7073   necessary steps
+00003a60: 206f 6620 7468 6520 7072 6f63 6573 7320   of the process 
+00003a70: 736f 2049 2064 6964 6e27 7420 7761 6e74  so I didn't want
+00003a80: 2074 6f0a 2020 2020 2020 2020 7472 7920   to.        try 
+00003a90: 746f 2065 6e63 6170 7375 6c61 7465 2061  to encapsulate a
+00003aa0: 6e79 2066 7572 7468 6572 0a20 2020 2020  ny further.     
+00003ab0: 2020 2072 1800 0000 2901 5a0e 626f 6172     r....).Z.boar
+00003ac0: 6473 5f73 616d 706c 6564 7a1b 5265 6d6f  ds_sampledz.Remo
+00003ad0: 7669 6e67 2074 6865 2077 6f72 7374 2066  ving the worst f
+00003ae0: 6974 7469 6e67 20e9 6400 0000 7a21 2070  itting .d...z! p
+00003af0: 6572 6365 6e74 206f 6620 706f 696e 7473  ercent of points
+00003b00: 2066 726f 6d20 7468 6520 6d6f 6465 6c4e   from the modelN
+00003b10: 2915 720f 0000 0072 3600 0000 5a09 746f  ).r....r6...Z.to
+00003b20: 6d6c 5f70 6174 6872 3a00 0000 5a14 7374  ml_pathr:...Z.st
+00003b30: 6572 656f 5f63 616c 6962 7261 7465 5f61  ereo_calibrate_a
+00003b40: 6c6c 720d 0000 005a 1567 6574 5f62 6573  llr....Z.get_bes
+00003b50: 745f 6361 6d65 7261 5f61 7272 6179 7257  t_camera_arrayrW
+00003b60: 0000 0072 1400 0000 729f 0000 0072 1100  ...r....r....r..
+00003b70: 0000 729c 0000 00da 086f 7074 696d 697a  ..r......optimiz
+00003b80: 6572 1200 0000 7245 0000 0072 a000 0000  er....rE...r....
+00003b90: 725e 0000 0072 5f00 0000 da11 4649 4c54  r^...r_.....FILT
+00003ba0: 4552 4544 5f46 5241 4354 494f 4e5a 1666  ERED_FRACTIONZ.f
+00003bb0: 696c 7465 725f 706f 696e 745f 6573 7469  ilter_point_esti
+00003bc0: 6d61 7465 735a 1373 6176 655f 6361 7074  matesZ.save_capt
+00003bd0: 7572 655f 766f 6c75 6d65 2902 722d 0000  ure_volume).r-..
+00003be0: 005a 1073 7465 7265 6f63 616c 6962 7261  .Z.stereocalibra
+00003bf0: 746f 7272 2500 0000 7225 0000 0072 2600  torr%...r%...r&.
+00003c00: 0000 da13 6573 7469 6d61 7465 5f65 7874  ....estimate_ext
+00003c10: 7269 6e73 6963 7307 0200 0073 2a00 0000  rinsics....s*...
+00003c20: 0206 0a01 04ff 0c03 0202 0601 02ff 0402  ................
+00003c30: 04fe 0204 0801 06ff 1004 0a01 1002 0402  ................
+00003c40: 0e01 04ff 0c03 0a01 1202 7a1b 5365 7373  ..........z.Sess
+00003c50: 696f 6e2e 6573 7469 6d61 7465 5f65 7874  ion.estimate_ext
+00003c60: 7269 6e73 6963 7372 2900 0000 2901 4629  rinsicsr)...).F)
+00003c70: 2272 1b00 0000 721c 0000 0072 1d00 0000  "r....r....r....
+00003c80: 7215 0000 0072 2b00 0000 7251 0000 0072  r....r+...rQ...r
+00003c90: 5400 0000 725a 0000 0072 6100 0000 7264  T...rZ...ra...rd
+00003ca0: 0000 0072 6b00 0000 7219 0000 0072 7400  ...rk...r....rt.
+00003cb0: 0000 da03 696e 7472 7600 0000 7277 0000  ....intrv...rw..
+00003cc0: 0072 6c00 0000 da04 626f 6f6c 7271 0000  .rl.....boolrq..
+00003cd0: 0072 7000 0000 7279 0000 0072 7a00 0000  .rp...ry...rz...
+00003ce0: 7282 0000 0072 8c00 0000 726f 0000 0072  r....r....ro...r
+00003cf0: 8e00 0000 7272 0000 0072 6e00 0000 7205  ....rr...rn...r.
+00003d00: 0000 0072 9800 0000 7299 0000 0072 8d00  ...r....r....r..
+00003d10: 0000 72a1 0000 0072 a500 0000 7225 0000  ..r....r....r%..
+00003d20: 0072 2500 0000 7225 0000 0072 2600 0000  .r%...r%...r&...
+00003d30: 7235 0000 003b 0000 0073 4000 0000 0800  r5...;...s@.....
+00003d40: 0e01 0824 0812 0807 080b 081d 081e 0e10  ...$............
+00003d50: 0e41 0e16 080f 0e06 0804 0806 0804 0804  .A..............
+00003d60: 0807 0823 0828 100b 080d 020a 04ff 0201  ...#.(..........
+00003d70: 02ff 0201 0aff 080c 080f 0816 0c16 7235  ..............r5
+00003d80: 0000 0029 35da 0674 7970 696e 67da 0d70  ...)5..typing..p
+00003d90: 7978 7933 642e 6c6f 6767 6572 da06 7079  yxy3d.logger..py
+00003da0: 7879 3364 725e 0000 00da 0367 6574 721b  xy3dr^.....getr.
+00003db0: 0000 00da 0c50 7951 7436 2e51 7443 6f72  .....PyQt6.QtCor
+00003dc0: 6572 0200 0000 7203 0000 005a 1263 6f6e  er....r....Z.con
+00003dd0: 6375 7272 656e 742e 6675 7475 7265 7372  current.futuresr
+00003de0: 0400 0000 da07 7061 7468 6c69 6272 0500  ......pathlibr..
+00003df0: 0000 da04 7469 6d65 7206 0000 00da 0465  ....timer......e
+00003e00: 6e75 6d72 0700 0000 7208 0000 005a 1f70  numr....r....Z.p
+00003e10: 7978 7933 642e 7472 6163 6b65 7273 2e63  yxy3d.trackers.c
+00003e20: 6861 7275 636f 5f74 7261 636b 6572 7209  haruco_trackerr.
+00003e30: 0000 005a 2170 7978 7933 642e 6361 6c69  ...Z!pyxy3d.cali
+00003e40: 6272 6174 696f 6e2e 6d6f 6e6f 6361 6c69  bration.monocali
+00003e50: 6272 6174 6f72 720a 0000 005a 1570 7978  bratorr....Z.pyx
+00003e60: 7933 642e 6361 6d65 7261 732e 6361 6d65  y3d.cameras.came
+00003e70: 7261 720b 0000 00da 1b70 7978 7933 642e  rar......pyxy3d.
+00003e80: 6361 6d65 7261 732e 7379 6e63 6872 6f6e  cameras.synchron
+00003e90: 697a 6572 720c 0000 005a 2770 7978 7933  izerr....Z'pyxy3
+00003ea0: 642e 6361 6d65 7261 732e 6361 6d65 7261  d.cameras.camera
+00003eb0: 5f61 7272 6179 5f69 6e69 7469 616c 697a  _array_initializ
+00003ec0: 6572 720d 0000 005a 1070 7978 7933 642e  err....Z.pyxy3d.
+00003ed0: 696e 7465 7266 6163 6572 0e00 0000 5a23  interfacer....Z#
+00003ee0: 7079 7879 3364 2e63 616c 6962 7261 7469  pyxy3d.calibrati
+00003ef0: 6f6e 2e73 7465 7265 6f63 616c 6962 7261  on.stereocalibra
+00003f00: 746f 7272 0f00 0000 5a31 7079 7879 3364  torr....Z1pyxy3d
+00003f10: 2e63 616c 6962 7261 7469 6f6e 2e63 6170  .calibration.cap
+00003f20: 7475 7265 5f76 6f6c 756d 652e 706f 696e  ture_volume.poin
+00003f30: 745f 6573 7469 6d61 7465 7372 1000 0000  t_estimatesr....
+00003f40: 5a30 7079 7879 3364 2e63 616c 6962 7261  Z0pyxy3d.calibra
+00003f50: 7469 6f6e 2e63 6170 7475 7265 5f76 6f6c  tion.capture_vol
+00003f60: 756d 652e 6361 7074 7572 655f 766f 6c75  ume.capture_volu
+00003f70: 6d65 7211 0000 005a 3470 7978 7933 642e  mer....Z4pyxy3d.
+00003f80: 6361 6c69 6272 6174 696f 6e2e 6361 7074  calibration.capt
+00003f90: 7572 655f 766f 6c75 6d65 2e71 7561 6c69  ure_volume.quali
+00003fa0: 7479 5f63 6f6e 7472 6f6c 6c65 7272 1200  ty_controllerr..
+00003fb0: 0000 5a1b 7079 7879 3364 2e63 616d 6572  ..Z.pyxy3d.camer
+00003fc0: 6173 2e63 616d 6572 615f 6172 7261 7972  as.camera_arrayr
+00003fd0: 1300 0000 5a46 7079 7879 3364 2e63 616c  ....ZFpyxy3d.cal
+00003fe0: 6962 7261 7469 6f6e 2e63 6170 7475 7265  ibration.capture
+00003ff0: 5f76 6f6c 756d 652e 6865 6c70 6572 5f66  _volume.helper_f
+00004000: 756e 6374 696f 6e73 2e67 6574 5f70 6f69  unctions.get_poi
+00004010: 6e74 5f65 7374 696d 6174 6573 7214 0000  nt_estimatesr...
+00004020: 00da 1370 7978 7933 642e 636f 6e66 6967  ...pyxy3d.config
+00004030: 7572 6174 6f72 7215 0000 005a 1a70 7978  uratorr....Z.pyx
+00004040: 7933 642e 6361 6d65 7261 732e 6c69 7665  y3d.cameras.live
+00004050: 5f73 7472 6561 6d72 1600 0000 da1f 7079  _streamr......py
+00004060: 7879 3364 2e72 6563 6f72 6469 6e67 2e76  xy3d.recording.v
+00004070: 6964 656f 5f72 6563 6f72 6465 7272 1700  ideo_recorderr..
+00004080: 0000 7287 0000 0072 a400 0000 7219 0000  ..r....r....r...
+00004090: 0072 2700 0000 7235 0000 0072 2500 0000  .r'...r5...r%...
+000040a0: 7225 0000 0072 2500 0000 7226 0000 00da  r%...r%...r&....
+000040b0: 083c 6d6f 6475 6c65 3e01 0000 0073 3800  .<module>....s8.
+000040c0: 0000 0801 0801 0c02 1002 0c01 0c01 0c01  ................
+000040d0: 1001 0c02 0c01 0c01 0c01 0c01 0c01 0c02  ................
+000040e0: 0c01 0c01 0c01 0c02 0c01 0c03 0c01 0c01  ................
+000040f0: 0403 0401 1003 100a 120b                 ..........
```

### Comparing `pyxy3d-0.1.3/pyxy3d/session/session.py` & `pyxy3d-0.1.4/pyxy3d/session/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Environment for managing all created objects and the primary interface for the GUI.
+import typing
 import pyxy3d.logger
 
 logger = pyxy3d.logger.get(__name__)
 
 from PyQt6.QtCore import QObject, pyqtSignal
 from concurrent.futures import ThreadPoolExecutor
 from pathlib import Path
@@ -40,25 +41,30 @@
     Charuco = auto()
     IntrinsicCalibration = auto()
     ExtrinsicCalibration = auto()
     CaptureVolumeOrigin = auto()
     Recording = auto()
     PostProcessing = auto()
 
-
-class Session(QObject):
+class QtSignaler(QObject):
     stream_tools_loaded_signal = pyqtSignal()
     stream_tools_disconnected_signal = pyqtSignal()
     unlock_postprocessing = pyqtSignal()
     recording_complete_signal = pyqtSignal()        
-
     mode_change_success = pyqtSignal(SessionMode)
 
+    def __init__(self) -> None:
+        super(QtSignaler, self).__init__()
+
+        
+class Session:
     def __init__(self, config: Configurator):
-        super(Session, self).__init__()
+        # need a way to let the GUI know when certain actions have been completed
+        self.qt_signaler = QtSignaler()
+
         self.config = config
         # self.folder = PurePath(directory).name
         self.path = self.config.session_path
 
         # this will not have anything to start, but the path
         # will be set
         self.extrinsic_calibration_xy = Path(
@@ -99,15 +105,15 @@
         self.cameras = {}
         for port, monocal in self.monocalibrators.items():
             monocal.stop_event.set()
         self.monocalibrators = {}
         self.synchronizer.stop_event.set()
         self.synchronizer = None
 
-        self.stream_tools_disconnected_signal.emit()
+        self.qt_signaler.stream_tools_disconnected_signal.emit()
 
     def is_camera_setup_eligible(self):
         if len(self.cameras) > 0:
             eligible = True
         else:
             eligible = False
         return eligible
@@ -400,15 +406,15 @@
         self.stream_tools_in_process = False
 
         logger.info("Pausing stream tools since default loads to charuco")
         self.pause_all_monocalibrators()
         self.pause_synchronizer()
         
         logger.info(f"Signalling successful loading of stream tools")
-        self.stream_tools_loaded_signal.emit()
+        self.qt_signaler.stream_tools_loaded_signal.emit()
 
     def _load_monocalibrators(self):
         for port, cam in self.cameras.items():
             if port in self.monocalibrators.keys():
                 logger.info(
                     f"Skipping over monocalibrator creation for port {port} because it already exists."
                 )
@@ -457,18 +463,18 @@
         while self.video_recorder.recording:
             logger.info("Waiting for video recorder to save out data...")
             sleep(0.5)
 
         self.is_recording = False
 
         logger.info(f"Recording of frames is complete...signalling change in status")
-        self.recording_complete_signal.emit()
+        self.qt_signaler.recording_complete_signal.emit()
 
         if self.is_post_processing_eligible():
-            self.unlock_postprocessing.emit()
+            self.qt_signaler.unlock_postprocessing.emit()
 
     def _adjust_resolutions(self):
         """Changes the camera resolution to the value in the configuration, as
         log as it is not configured for the default resolution"""
 
         def adjust_res_worker(port):
             stream = self.streams[port]
```

### Comparing `pyxy3d-0.1.3/pyxy3d/trackers/__pycache__/charuco_tracker.cpython-310.pyc` & `pyxy3d-0.1.4/pyxy3d/trackers/__pycache__/charuco_tracker.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/trackers/__pycache__/hand_tracker.cpython-310.pyc` & `pyxy3d-0.1.4/pyxy3d/trackers/__pycache__/hand_tracker.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/trackers/__pycache__/helper.cpython-310.pyc` & `pyxy3d-0.1.4/pyxy3d/trackers/__pycache__/helper.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/trackers/__pycache__/holistic_opensim_tracker.cpython-310.pyc` & `pyxy3d-0.1.4/pyxy3d/trackers/__pycache__/holistic_opensim_tracker.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/trackers/__pycache__/holistic_tracker.cpython-310.pyc` & `pyxy3d-0.1.4/pyxy3d/trackers/__pycache__/holistic_tracker.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/trackers/__pycache__/pose_tracker.cpython-310.pyc` & `pyxy3d-0.1.4/pyxy3d/trackers/__pycache__/pose_tracker.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/trackers/__pycache__/threaded_hand_tracker.cpython-310.pyc` & `pyxy3d-0.1.4/pyxy3d/trackers/__pycache__/threaded_hand_tracker.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/trackers/__pycache__/tracker_enum.cpython-310.pyc` & `pyxy3d-0.1.4/pyxy3d/trackers/__pycache__/tracker_enum.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/trackers/charuco_tracker.py` & `pyxy3d-0.1.4/pyxy3d/trackers/charuco_tracker.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/trackers/hand_tracker.py` & `pyxy3d-0.1.4/pyxy3d/trackers/hand_tracker.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/trackers/helper.py` & `pyxy3d-0.1.4/pyxy3d/trackers/helper.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/trackers/holistic_opensim_tracker.py` & `pyxy3d-0.1.4/pyxy3d/trackers/holistic_opensim_tracker.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/trackers/holistic_tracker.py` & `pyxy3d-0.1.4/pyxy3d/trackers/holistic_tracker.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/trackers/pose_tracker.py` & `pyxy3d-0.1.4/pyxy3d/trackers/pose_tracker.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/trackers/tracker_enum.py` & `pyxy3d-0.1.4/pyxy3d/trackers/tracker_enum.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/array_stereo_triangulator.cpython-310.pyc` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/array_stereo_triangulator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/array_stereo_triangulator.cpython-38.pyc` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/array_stereo_triangulator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/helper.cpython-310.pyc` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/helper.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.cpython-310.pyc` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.cpython-38.pyc` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.1.nbc` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.2.nbc` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.2.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.nbi` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py310.1.nbc` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py310.nbi` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py38.1.nbc` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py38.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py38.nbi` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py38.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-138.py310.1.nbc` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-138.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-138.py310.nbi` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-138.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-139.py310.1.nbc` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-139.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-139.py310.nbi` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-139.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-86.py38.1.nbc` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-86.py38.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-86.py38.nbi` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-86.py38.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-88.py38.1.nbc` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-88.py38.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-88.py38.nbi` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-88.py38.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.unique_with_counts-118.py310.1.nbc` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.unique_with_counts-118.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.unique_with_counts-118.py310.nbi` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.unique_with_counts-118.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/stereo_points_builder.cpython-310.pyc` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/stereo_points_builder.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/stereo_points_builder.cpython-38.pyc` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/stereo_points_builder.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.cpython-310.pyc` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.1.nbc` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.2.nbc` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.2.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.3.nbc` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.3.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.nbi` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-170.py310.1.nbc` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-170.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-170.py310.nbi` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-170.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-186.py310.1.nbc` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-186.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-186.py310.nbi` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-186.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.1.nbc` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.2.nbc` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.2.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.3.nbc` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.3.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.nbi` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.1.nbc` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.2.nbc` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.2.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.3.nbc` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.3.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.nbi` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.1.nbc` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.2.nbc` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.2.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.3.nbc` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.3.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.nbi` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-195.py310.1.nbc` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-195.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-195.py310.nbi` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-195.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.1.nbc` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.2.nbc` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.2.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.nbi` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.1.nbc` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.2.nbc` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.2.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.nbi` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-170.py310.1.nbc` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-170.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-170.py310.nbi` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-170.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.1.nbc` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.2.nbc` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.2.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.nbi` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.1.nbc` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.2.nbc` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.2.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.nbi` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.1.nbc` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.2.nbc` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.2.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.nbi` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-179.py310.1.nbc` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-179.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-179.py310.nbi` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-179.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/triangulator.cpython-38.pyc` & `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/triangulator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/array_stereo_triangulator.py` & `pyxy3d-0.1.4/pyxy3d/triangulate/array_stereo_triangulator.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/stereo_points_builder.py` & `pyxy3d-0.1.4/pyxy3d/triangulate/stereo_points_builder.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/pyxy3d/triangulate/sync_packet_triangulator.py` & `pyxy3d-0.1.4/pyxy3d/triangulate/sync_packet_triangulator.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.3/README.md` & `pyxy3d-0.1.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,65 +1,75 @@
 
 
 <div align="center"><img src = "pyxy3d/gui/icons/pyxy_logo.svg" width = "150"></div>
 
+<div align="center">
 
-[Introduction](#introduction)
+[Quick Start](#quick-start) | [Key Features](#key-features) | [Limitations](#limitations) | [Known Issues](#known-issues)
 
-[Quick Start](#quick-start)
+</div>
 
-[Key Features](#key-features)
-
-[Limitations](#limitations)
 
 ---
 ## About
 
 Pyxy3D (*pixie-3d*) is an open-source **Py**thon package for converting 2D **(x,y)** point data to **3D** estimates. It is intended to serve as the calibration and triangulation workhorse of a low-cost DIY motion capture studio. It's core functionality includes: 
 
 - the estimation of intrinsic (focal length/optical center/distortion) and extrinsic (rotation and translation) camera parameters via a GUI
 - API for slotting various tracking solutions into the data pipeline
 - triangulation of tracked points
 
 The package comes included with a sample tracker using Google's Mediapipe which illustrates how to use the tracker API. The camera management backend allows for recording of synchronized frames from connected webcams, though the frame rate/resolution/number of cameras will be limited by the bandwidth of the current system.
 
+The gif below gives a quick demo of the following steps:
+1. Single Camera Calibration
+2. Multicamera Calibratoin
+3. Synchronized Recording
+4. Post-processing with Mediapipe Holistic
+5. Visualization of triangulated results
+
 ![Quick_Demo](https://github.com/mprib/pyxy3d/assets/31831778/5fc8e15e-ca64-447b-86b8-69c64601199c)
 
 ## Quick Start
 
+This package has only been successfully tested on Windows 10 and MacOS 12 Ventura. Limited testing on Linx (Ubuntu) has failed due to issues loading PyQt6.
+
 From a terminal (the code below is using Powershell), do the following:
 
 1. Create a new project folder
 ```powershell
 mkdir pyxy3d_demo
 ```
 2. Navigate into that directory
 ```powershell
 cd pyxy3d_demo
 ```
 3. Create a virtual environment with [Python 3.10](https://www.python.org/downloads/release/python-3100/) or later:
 ```powershell
-C:\Python310\python.exe -m venv .venv
+python3.10 -m venv .venv
 ```
 4. Activate the environment
 ```powershell
 .\.venv\Scripts\activate
 ```
 
 5. Install Pyxy3D
 ```powershell
 pip install pyxy3d
 ```
-Note that this will also install dependencies into the virtual environment, so complete download and installation may take several minutes..
+Note that this will also install dependencies into the virtual environment, some of which are large (OpenCV, SciPy and Numpy are among the core dependencies). Complete download and installation may take several minutes. 
 
 6. Launch Pyxy3D    
 ```powershell
 pyxy3d
 ```
-At this point, an application window should launch. It may take several seconds for this to load. Refer to the [Quick Start Video Walkthrough](https://youtu.be/QHQKkLCE0e4) to see how to calibrate, record and process data
+
+
+At this point, an application window should launch, though be aware that it may take several seconds for this to load. 
+Refer to the [Quick Start Video Walkthrough](https://youtu.be/QHQKkLCE0e4) to see how to calibrate, record and process data
 
 ## Key Features
 
 The project leans heavily upon OpenCV, SciPy, and PyQt to provide the following **key features**:
 
 - User-friendly graphical user interface (GUI)
 - Easy creation and modification of the charuco calibration board
@@ -73,20 +83,21 @@
 - Triangulation of tracked landmarks
 - Visualization of triangulated points for quick confirmation of output quality
 - Currently exporting to `.csv` and `.trc` file formats
 
 ## Limitations
 
 Please note that the system currently has the following **limitations**:
-- MediaPipe is only configured to run on Windows
-    - while the camera calibration will likely work on other systems, the included sample markerless tracking will not (currently)
 - It does not support anything other than standard webcams at the moment 
 - The frame capture backend presents a primary bottleneck that will limit the number of cameras/resolution/frame rates that can be used, which ultimately limits the size and precision of the capture volume.
 - Data export is currently limited to .csv, and .trc files. Use in 3D animation tools like Blender, which require character rigging, will require additional processing.
 
+## Known Issues
+### Seg Faults on Windows 10
+[June 23, 2023] The most recent version of the package on PyPI (0.1.3) has been updated to allow it to run on MacOS 12. This update did not change any code, but did change which versions of the underlying dependencies were configured to install. Segmentation faults during recording emerged after this update and are currently being addressed as a top priority.
 
 ## Reporting Issues and Requesting Features
 
 To report a bug or request a feature, please [open an issue](https://github.com/mprib/pyxy3d/issues). Please keep in mind that this is an open-source project supported by volunteer effort, so your patience is appreciated.
 
 ## General Questions and Conversation
```

### Comparing `pyxy3d-0.1.3/PKG-INFO` & `pyxy3d-0.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: pyxy3d
-Version: 0.1.3
+Version: 0.1.4
 Summary: A package for calibrating standard webcams to enable 3d motion tracking
 License: AGPL-3.0-only
 Author: Mac Prible
 Author-email: prible@gmail.com
-Requires-Python: >=3.10,<3.12
+Requires-Python: >=3.10,<3.10.11
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyOpenGL (>=3.1.6,<4.0.0)
 Requires-Dist: PyQt6 (>=6.4.0,<7.0.0)
 Requires-Dist: mediapipe (==0.10.1)
 Requires-Dist: numba (>=0.56.4,<0.57.0)
 Requires-Dist: opencv-contrib-python (>=4.7,<5.0)
 Requires-Dist: pandas (>=1.5.0,<2.0.0)
 Requires-Dist: pyqtgraph (>=0.13.2,<0.14.0)
@@ -22,68 +21,78 @@
 Project-URL: repository, https://github.com/mprib/pyxy3d
 Description-Content-Type: text/markdown
 
 
 
 <div align="center"><img src = "pyxy3d/gui/icons/pyxy_logo.svg" width = "150"></div>
 
+<div align="center">
 
-[Introduction](#introduction)
+[Quick Start](#quick-start) | [Key Features](#key-features) | [Limitations](#limitations) | [Known Issues](#known-issues)
 
-[Quick Start](#quick-start)
+</div>
 
-[Key Features](#key-features)
-
-[Limitations](#limitations)
 
 ---
 ## About
 
 Pyxy3D (*pixie-3d*) is an open-source **Py**thon package for converting 2D **(x,y)** point data to **3D** estimates. It is intended to serve as the calibration and triangulation workhorse of a low-cost DIY motion capture studio. It's core functionality includes: 
 
 - the estimation of intrinsic (focal length/optical center/distortion) and extrinsic (rotation and translation) camera parameters via a GUI
 - API for slotting various tracking solutions into the data pipeline
 - triangulation of tracked points
 
 The package comes included with a sample tracker using Google's Mediapipe which illustrates how to use the tracker API. The camera management backend allows for recording of synchronized frames from connected webcams, though the frame rate/resolution/number of cameras will be limited by the bandwidth of the current system.
 
+The gif below gives a quick demo of the following steps:
+1. Single Camera Calibration
+2. Multicamera Calibratoin
+3. Synchronized Recording
+4. Post-processing with Mediapipe Holistic
+5. Visualization of triangulated results
+
 ![Quick_Demo](https://github.com/mprib/pyxy3d/assets/31831778/5fc8e15e-ca64-447b-86b8-69c64601199c)
 
 ## Quick Start
 
+This package has only been successfully tested on Windows 10 and MacOS 12 Ventura. Limited testing on Linx (Ubuntu) has failed due to issues loading PyQt6.
+
 From a terminal (the code below is using Powershell), do the following:
 
 1. Create a new project folder
 ```powershell
 mkdir pyxy3d_demo
 ```
 2. Navigate into that directory
 ```powershell
 cd pyxy3d_demo
 ```
 3. Create a virtual environment with [Python 3.10](https://www.python.org/downloads/release/python-3100/) or later:
 ```powershell
-C:\Python310\python.exe -m venv .venv
+python3.10 -m venv .venv
 ```
 4. Activate the environment
 ```powershell
 .\.venv\Scripts\activate
 ```
 
 5. Install Pyxy3D
 ```powershell
 pip install pyxy3d
 ```
-Note that this will also install dependencies into the virtual environment, so complete download and installation may take several minutes..
+Note that this will also install dependencies into the virtual environment, some of which are large (OpenCV, SciPy and Numpy are among the core dependencies). Complete download and installation may take several minutes. 
 
 6. Launch Pyxy3D    
 ```powershell
 pyxy3d
 ```
-At this point, an application window should launch. It may take several seconds for this to load. Refer to the [Quick Start Video Walkthrough](https://youtu.be/QHQKkLCE0e4) to see how to calibrate, record and process data
+
+
+At this point, an application window should launch, though be aware that it may take several seconds for this to load. 
+Refer to the [Quick Start Video Walkthrough](https://youtu.be/QHQKkLCE0e4) to see how to calibrate, record and process data
 
 ## Key Features
 
 The project leans heavily upon OpenCV, SciPy, and PyQt to provide the following **key features**:
 
 - User-friendly graphical user interface (GUI)
 - Easy creation and modification of the charuco calibration board
@@ -97,20 +106,21 @@
 - Triangulation of tracked landmarks
 - Visualization of triangulated points for quick confirmation of output quality
 - Currently exporting to `.csv` and `.trc` file formats
 
 ## Limitations
 
 Please note that the system currently has the following **limitations**:
-- MediaPipe is only configured to run on Windows
-    - while the camera calibration will likely work on other systems, the included sample markerless tracking will not (currently)
 - It does not support anything other than standard webcams at the moment 
 - The frame capture backend presents a primary bottleneck that will limit the number of cameras/resolution/frame rates that can be used, which ultimately limits the size and precision of the capture volume.
 - Data export is currently limited to .csv, and .trc files. Use in 3D animation tools like Blender, which require character rigging, will require additional processing.
 
+## Known Issues
+### Seg Faults on Windows 10
+[June 23, 2023] The most recent version of the package on PyPI (0.1.3) has been updated to allow it to run on MacOS 12. This update did not change any code, but did change which versions of the underlying dependencies were configured to install. Segmentation faults during recording emerged after this update and are currently being addressed as a top priority.
 
 ## Reporting Issues and Requesting Features
 
 To report a bug or request a feature, please [open an issue](https://github.com/mprib/pyxy3d/issues). Please keep in mind that this is an open-source project supported by volunteer effort, so your patience is appreciated.
 
 ## General Questions and Conversation
```

