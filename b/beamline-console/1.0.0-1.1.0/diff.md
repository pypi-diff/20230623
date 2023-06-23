# Comparing `tmp/beamline_console-1.0.0.tar.gz` & `tmp/beamline_console-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/beamline_console-1.0.0.tar", last modified: Wed Feb 22 10:30:28 2023, max compression
+gzip compressed data, was "beamline_console-1.1.0.tar", last modified: Fri Jun 23 08:05:53 2023, max compression
```

## Comparing `beamline_console-1.0.0.tar` & `beamline_console-1.1.0.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-02-22 10:30:28.000000 beamline_console-1.0.0/
--rw-r--r--   0 matveyev (30593) irc         (39)    35143 2023-02-10 11:18:51.000000 beamline_console-1.0.0/LICENSE.txt
--rw-r--r--   0 matveyev (30593) irc         (39)      238 2023-02-22 10:19:46.000000 beamline_console-1.0.0/MANIFEST.in
--rw-r--r--   0 matveyev (30593) irc         (39)      732 2023-02-22 10:30:28.000000 beamline_console-1.0.0/PKG-INFO
-drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-02-22 10:30:28.000000 beamline_console-1.0.0/beamline_console/
--rw-r--r--   0 matveyev (30593) irc         (39)     4493 2023-02-22 10:06:27.000000 beamline_console-1.0.0/beamline_console/__init__.py
--rw-r--r--   0 matveyev (30593) irc         (39)     1016 2023-02-08 16:43:16.000000 beamline_console-1.0.0/beamline_console/base_widget.py
--rw-r--r--   0 matveyev (30593) irc         (39)      157 2023-02-22 10:28:48.000000 beamline_console-1.0.0/beamline_console/beamline_console.desktop
--rwxr-xr-x   0 matveyev (30593) irc         (39)       65 2023-02-22 10:13:56.000000 beamline_console-1.0.0/beamline_console/beamline_console.sh
--rw-r--r--   0 matveyev (30593) irc         (39)    13467 2023-02-21 12:57:49.000000 beamline_console-1.0.0/beamline_console/beamlinehal.py
--rw-r--r--   0 matveyev (30593) irc         (39)      795 2023-02-20 08:50:32.000000 beamline_console-1.0.0/beamline_console/constants.py
-drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-02-22 10:30:28.000000 beamline_console-1.0.0/beamline_console/default_config/
--rw-r--r--   0 matveyev (30593) irc         (39)        0 2022-09-29 13:24:55.000000 beamline_console-1.0.0/beamline_console/default_config/__init__.py
--rw-r--r--   0 matveyev (30593) irc         (39)      209 2023-02-22 10:06:27.000000 beamline_console-1.0.0/beamline_console/default_config/devices.xml
--rw-r--r--   0 matveyev (30593) irc         (39)      603 2023-02-22 10:06:27.000000 beamline_console-1.0.0/beamline_console/default_config/main.cfg
-drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-02-22 10:30:28.000000 beamline_console-1.0.0/beamline_console/devicecontrol/
--rw-r--r--   0 matveyev (30593) irc         (39)        0 2022-09-29 13:24:55.000000 beamline_console-1.0.0/beamline_console/devicecontrol/__init__.py
--rw-r--r--   0 matveyev (30593) irc         (39)     3230 2023-02-20 08:51:13.000000 beamline_console-1.0.0/beamline_console/devicecontrol/beamlinegraphicsscene.py
--rw-r--r--   0 matveyev (30593) irc         (39)     4431 2023-02-20 15:49:19.000000 beamline_console-1.0.0/beamline_console/devicecontrol/beamlinewidget.py
--rw-r--r--   0 matveyev (30593) irc         (39)     1268 2023-02-20 08:52:41.000000 beamline_console-1.0.0/beamline_console/devicecontrol/devicehistorydialog.py
-drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-02-22 10:30:28.000000 beamline_console-1.0.0/beamline_console/devicecontrol/deviceitem/
--rw-r--r--   0 matveyev (30593) irc         (39)        0 2022-09-29 13:24:55.000000 beamline_console-1.0.0/beamline_console/devicecontrol/deviceitem/__init__.py
--rw-r--r--   0 matveyev (30593) irc         (39)     2236 2023-02-08 16:37:34.000000 beamline_console-1.0.0/beamline_console/devicecontrol/deviceitem/devicegraphicsitem.py
--rw-r--r--   0 matveyev (30593) irc         (39)     1947 2023-02-07 16:40:40.000000 beamline_console-1.0.0/beamline_console/devicecontrol/deviceitem/frameitem.py
--rw-r--r--   0 matveyev (30593) irc         (39)     3762 2023-02-08 15:40:07.000000 beamline_console-1.0.0/beamline_console/devicecontrol/deviceitem/statusitem.py
--rw-r--r--   0 matveyev (30593) irc         (39)      902 2023-02-10 14:43:44.000000 beamline_console-1.0.0/beamline_console/devicecontrol/deviceitem/titleitem.py
--rw-r--r--   0 matveyev (30593) irc         (39)     4613 2023-02-20 16:30:02.000000 beamline_console-1.0.0/beamline_console/devicecontrol/devicewidget.py
--rw-r--r--   0 matveyev (30593) irc         (39)    11471 2023-02-21 16:49:02.000000 beamline_console-1.0.0/beamline_console/devicecontrol/motoritemwidget.py
--rw-r--r--   0 matveyev (30593) irc         (39)     9570 2023-02-20 15:11:50.000000 beamline_console-1.0.0/beamline_console/devicecontrol/motorpropsdialog.py
-drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-02-22 10:30:28.000000 beamline_console-1.0.0/beamline_console/devices/
--rw-r--r--   0 matveyev (30593) irc         (39)        0 2022-09-29 13:24:55.000000 beamline_console-1.0.0/beamline_console/devices/__init__.py
--rw-r--r--   0 matveyev (30593) irc         (39)     7838 2023-02-20 11:14:06.000000 beamline_console-1.0.0/beamline_console/devices/abstractmotor.py
--rw-r--r--   0 matveyev (30593) irc         (39)     3421 2023-02-20 08:51:12.000000 beamline_console-1.0.0/beamline_console/devices/dummymotor.py
--rw-r--r--   0 matveyev (30593) irc         (39)     5090 2023-02-20 11:20:20.000000 beamline_console-1.0.0/beamline_console/devices/motordevice.py
--rw-r--r--   0 matveyev (30593) irc         (39)     7028 2023-02-21 08:34:53.000000 beamline_console-1.0.0/beamline_console/devices/tangomotor.py
-drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-02-22 10:30:28.000000 beamline_console-1.0.0/beamline_console/gui/
--rw-r--r--   0 matveyev (30593) irc         (39)     4098 2023-02-21 10:29:05.000000 beamline_console-1.0.0/beamline_console/gui/AboutDialog_ui.py
--rw-r--r--   0 matveyev (30593) irc         (39)     2617 2023-02-21 10:29:02.000000 beamline_console-1.0.0/beamline_console/gui/BeamlineWidget_ui.py
--rw-r--r--   0 matveyev (30593) irc         (39)     4206 2023-02-21 10:29:05.000000 beamline_console-1.0.0/beamline_console/gui/DeviceItem_ui.py
--rw-r--r--   0 matveyev (30593) irc         (39)     3527 2023-02-21 10:29:05.000000 beamline_console-1.0.0/beamline_console/gui/DeviceWidget_ui.py
--rw-r--r--   0 matveyev (30593) irc         (39)     2004 2023-02-21 10:29:04.000000 beamline_console-1.0.0/beamline_console/gui/ErrorDialog_ui.py
--rw-r--r--   0 matveyev (30593) irc         (39)     8587 2023-02-21 10:29:03.000000 beamline_console-1.0.0/beamline_console/gui/InputDialog_ui.py
--rw-r--r--   0 matveyev (30593) irc         (39)     2504 2023-02-21 10:29:03.000000 beamline_console-1.0.0/beamline_console/gui/LoggingWidget_ui.py
--rw-r--r--   0 matveyev (30593) irc         (39)      820 2023-02-21 10:29:01.000000 beamline_console-1.0.0/beamline_console/gui/MainWindow_ui.py
--rw-r--r--   0 matveyev (30593) irc         (39)    11299 2023-02-21 10:29:05.000000 beamline_console-1.0.0/beamline_console/gui/MotorItemWidget_ui.py
--rw-r--r--   0 matveyev (30593) irc         (39)    21429 2023-02-21 10:29:05.000000 beamline_console-1.0.0/beamline_console/gui/MotorPropsDialog_ui.py
--rw-r--r--   0 matveyev (30593) irc         (39)     4188 2023-02-21 10:29:05.000000 beamline_console-1.0.0/beamline_console/gui/SaveSnapshotDialog_ui.py
--rw-r--r--   0 matveyev (30593) irc         (39)     3123 2023-02-21 10:29:03.000000 beamline_console-1.0.0/beamline_console/gui/SnapshotWidget_ui.py
--rw-r--r--   0 matveyev (30593) irc         (39)        0 2023-02-07 12:33:01.000000 beamline_console-1.0.0/beamline_console/gui/__init__.py
--rw-r--r--   0 matveyev (30593) irc         (39)   141271 2023-02-21 10:29:04.000000 beamline_console-1.0.0/beamline_console/gui/icons_rc.py
-drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-02-22 10:30:28.000000 beamline_console-1.0.0/beamline_console/logger/
--rw-r--r--   0 matveyev (30593) irc         (39)        0 2022-09-29 13:24:55.000000 beamline_console-1.0.0/beamline_console/logger/__init__.py
--rw-r--r--   0 matveyev (30593) irc         (39)      691 2023-02-10 14:27:22.000000 beamline_console-1.0.0/beamline_console/logger/guilogger.py
--rw-r--r--   0 matveyev (30593) irc         (39)     1685 2023-02-20 08:51:14.000000 beamline_console-1.0.0/beamline_console/logger/highlightlogs.py
--rw-r--r--   0 matveyev (30593) irc         (39)     4652 2023-02-21 13:21:25.000000 beamline_console-1.0.0/beamline_console/logger/loggingwidget.py
--rw-r--r--   0 matveyev (30593) irc         (39)      249 2023-02-07 13:05:05.000000 beamline_console-1.0.0/beamline_console/logger/logit.py
--rw-r--r--   0 matveyev (30593) irc         (39)    10443 2023-02-20 15:49:19.000000 beamline_console-1.0.0/beamline_console/main_window.py
--rw-r--r--   0 matveyev (30593) irc         (39)      878 2023-02-22 10:23:23.000000 beamline_console-1.0.0/beamline_console/release.py
-drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-02-22 10:30:28.000000 beamline_console-1.0.0/beamline_console/snapshot/
--rw-r--r--   0 matveyev (30593) irc         (39)        0 2023-01-04 14:14:18.000000 beamline_console-1.0.0/beamline_console/snapshot/__init__.py
--rw-r--r--   0 matveyev (30593) irc         (39)     8949 2023-02-21 11:40:13.000000 beamline_console-1.0.0/beamline_console/snapshot/beamsnapshot.py
--rw-r--r--   0 matveyev (30593) irc         (39)     5979 2023-02-20 16:55:06.000000 beamline_console-1.0.0/beamline_console/snapshot/savesnapshotdialog.py
--rw-r--r--   0 matveyev (30593) irc         (39)     5553 2023-02-21 11:40:13.000000 beamline_console-1.0.0/beamline_console/snapshot/snapshotmanager.py
--rw-r--r--   0 matveyev (30593) irc         (39)     9284 2023-02-20 16:51:01.000000 beamline_console-1.0.0/beamline_console/snapshot/snapshotwidget.py
-drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-02-22 10:30:28.000000 beamline_console-1.0.0/beamline_console/utils/
--rw-r--r--   0 matveyev (30593) irc         (39)        0 2022-09-29 13:24:55.000000 beamline_console-1.0.0/beamline_console/utils/__init__.py
--rw-r--r--   0 matveyev (30593) irc         (39)      868 2023-02-20 16:35:07.000000 beamline_console-1.0.0/beamline_console/utils/aboutdialog.py
--rw-r--r--   0 matveyev (30593) irc         (39)      868 2023-02-20 09:08:11.000000 beamline_console-1.0.0/beamline_console/utils/clickablelabel.py
--rw-r--r--   0 matveyev (30593) irc         (39)      814 2023-02-21 09:25:59.000000 beamline_console-1.0.0/beamline_console/utils/errordialog.py
--rw-r--r--   0 matveyev (30593) irc         (39)    12914 2023-02-20 08:52:42.000000 beamline_console-1.0.0/beamline_console/utils/functions.py
--rw-r--r--   0 matveyev (30593) irc         (39)     4092 2023-02-21 10:34:25.000000 beamline_console-1.0.0/beamline_console/utils/input_dialog.py
--rwxr-xr-x   0 matveyev (30593) irc         (39)     9475 2023-02-20 08:51:14.000000 beamline_console-1.0.0/beamline_console/utils/range_slider.py
--rw-r--r--   0 matveyev (30593) irc         (39)     1879 2023-02-20 08:51:14.000000 beamline_console-1.0.0/beamline_console/utils/settings.py
-drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-02-22 10:30:28.000000 beamline_console-1.0.0/beamline_console.egg-info/
--rw-r--r--   0 matveyev (30593) irc         (39)      732 2023-02-22 10:30:28.000000 beamline_console-1.0.0/beamline_console.egg-info/PKG-INFO
--rw-r--r--   0 matveyev (30593) irc         (39)     2769 2023-02-22 10:30:28.000000 beamline_console-1.0.0/beamline_console.egg-info/SOURCES.txt
--rw-r--r--   0 matveyev (30593) irc         (39)        1 2023-02-22 10:30:28.000000 beamline_console-1.0.0/beamline_console.egg-info/dependency_links.txt
--rw-r--r--   0 matveyev (30593) irc         (39)       60 2023-02-22 10:30:28.000000 beamline_console-1.0.0/beamline_console.egg-info/entry_points.txt
--rw-r--r--   0 matveyev (30593) irc         (39)       57 2023-02-22 10:30:28.000000 beamline_console-1.0.0/beamline_console.egg-info/requires.txt
--rw-r--r--   0 matveyev (30593) irc         (39)       17 2023-02-22 10:30:28.000000 beamline_console-1.0.0/beamline_console.egg-info/top_level.txt
--rw-r--r--   0 matveyev (30593) irc         (39)       75 2023-02-22 10:30:28.000000 beamline_console-1.0.0/setup.cfg
--rw-r--r--   0 matveyev (30593) irc         (39)     2457 2023-02-22 10:22:31.000000 beamline_console-1.0.0/setup.py
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-06-23 08:05:53.585771 beamline_console-1.1.0/
+-rw-r--r--   0 matveyev (30593) irc         (39)    35143 2023-03-14 11:26:07.000000 beamline_console-1.1.0/LICENSE.txt
+-rw-r--r--   0 matveyev (30593) irc         (39)      238 2023-03-14 11:26:07.000000 beamline_console-1.1.0/MANIFEST.in
+-rw-r--r--   0 matveyev (30593) irc         (39)      732 2023-06-23 08:05:53.585771 beamline_console-1.1.0/PKG-INFO
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-06-23 08:05:53.581771 beamline_console-1.1.0/beamline_console/
+-rw-r--r--   0 matveyev (30593) irc         (39)     4581 2023-06-22 14:07:35.000000 beamline_console-1.1.0/beamline_console/__init__.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     1016 2023-03-14 11:26:07.000000 beamline_console-1.1.0/beamline_console/base_widget.py
+-rw-r--r--   0 matveyev (30593) irc         (39)      157 2023-03-14 11:26:07.000000 beamline_console-1.1.0/beamline_console/beamline_console.desktop
+-rwxr-xr-x   0 matveyev (30593) irc         (39)       65 2023-03-14 11:26:07.000000 beamline_console-1.1.0/beamline_console/beamline_console.sh
+-rw-r--r--   0 matveyev (30593) irc         (39)    13467 2023-03-14 11:26:07.000000 beamline_console-1.1.0/beamline_console/beamlinehal.py
+-rw-r--r--   0 matveyev (30593) irc         (39)      795 2023-03-14 11:26:07.000000 beamline_console-1.1.0/beamline_console/constants.py
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-06-23 08:05:53.581771 beamline_console-1.1.0/beamline_console/default_config/
+-rw-r--r--   0 matveyev (30593) irc         (39)        0 2023-03-14 11:26:07.000000 beamline_console-1.1.0/beamline_console/default_config/__init__.py
+-rw-r--r--   0 matveyev (30593) irc         (39)      209 2023-03-14 11:26:07.000000 beamline_console-1.1.0/beamline_console/default_config/devices.xml
+-rw-r--r--   0 matveyev (30593) irc         (39)      603 2023-03-14 11:26:07.000000 beamline_console-1.1.0/beamline_console/default_config/main.cfg
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-06-23 08:05:53.585771 beamline_console-1.1.0/beamline_console/devicecontrol/
+-rw-r--r--   0 matveyev (30593) irc         (39)        0 2023-03-14 11:26:07.000000 beamline_console-1.1.0/beamline_console/devicecontrol/__init__.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     3230 2023-03-14 11:26:07.000000 beamline_console-1.1.0/beamline_console/devicecontrol/beamlinegraphicsscene.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     4536 2023-06-22 13:44:06.000000 beamline_console-1.1.0/beamline_console/devicecontrol/beamlinewidget.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     1268 2023-03-14 11:26:07.000000 beamline_console-1.1.0/beamline_console/devicecontrol/devicehistorydialog.py
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-06-23 08:05:53.585771 beamline_console-1.1.0/beamline_console/devicecontrol/deviceitem/
+-rw-r--r--   0 matveyev (30593) irc         (39)        0 2023-03-14 11:26:07.000000 beamline_console-1.1.0/beamline_console/devicecontrol/deviceitem/__init__.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     2236 2023-03-14 11:26:07.000000 beamline_console-1.1.0/beamline_console/devicecontrol/deviceitem/devicegraphicsitem.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     1947 2023-03-14 11:26:07.000000 beamline_console-1.1.0/beamline_console/devicecontrol/deviceitem/frameitem.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     3762 2023-03-14 11:26:07.000000 beamline_console-1.1.0/beamline_console/devicecontrol/deviceitem/statusitem.py
+-rw-r--r--   0 matveyev (30593) irc         (39)      902 2023-03-14 11:26:07.000000 beamline_console-1.1.0/beamline_console/devicecontrol/deviceitem/titleitem.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     4613 2023-03-14 11:26:07.000000 beamline_console-1.1.0/beamline_console/devicecontrol/devicewidget.py
+-rw-r--r--   0 matveyev (30593) irc         (39)    11471 2023-03-14 11:26:07.000000 beamline_console-1.1.0/beamline_console/devicecontrol/motoritemwidget.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     9570 2023-03-14 11:26:07.000000 beamline_console-1.1.0/beamline_console/devicecontrol/motorpropsdialog.py
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-06-23 08:05:53.585771 beamline_console-1.1.0/beamline_console/devices/
+-rw-r--r--   0 matveyev (30593) irc         (39)        0 2023-03-14 11:26:07.000000 beamline_console-1.1.0/beamline_console/devices/__init__.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     7838 2023-03-14 11:26:07.000000 beamline_console-1.1.0/beamline_console/devices/abstractmotor.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     3421 2023-03-14 11:26:07.000000 beamline_console-1.1.0/beamline_console/devices/dummymotor.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     5090 2023-03-14 11:26:07.000000 beamline_console-1.1.0/beamline_console/devices/motordevice.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     7028 2023-06-22 14:08:45.000000 beamline_console-1.1.0/beamline_console/devices/tangomotor.py
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-06-23 08:05:53.585771 beamline_console-1.1.0/beamline_console/gui/
+-rw-r--r--   0 matveyev (30593) irc         (39)     4098 2023-03-14 11:26:07.000000 beamline_console-1.1.0/beamline_console/gui/AboutDialog_ui.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     2617 2023-03-14 11:26:07.000000 beamline_console-1.1.0/beamline_console/gui/BeamlineWidget_ui.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     4206 2023-03-14 11:26:07.000000 beamline_console-1.1.0/beamline_console/gui/DeviceItem_ui.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     3527 2023-03-14 11:26:07.000000 beamline_console-1.1.0/beamline_console/gui/DeviceWidget_ui.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     2004 2023-03-14 11:26:07.000000 beamline_console-1.1.0/beamline_console/gui/ErrorDialog_ui.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     8587 2023-03-14 11:26:07.000000 beamline_console-1.1.0/beamline_console/gui/InputDialog_ui.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     2504 2023-03-14 11:26:07.000000 beamline_console-1.1.0/beamline_console/gui/LoggingWidget_ui.py
+-rw-r--r--   0 matveyev (30593) irc         (39)      820 2023-03-14 11:26:07.000000 beamline_console-1.1.0/beamline_console/gui/MainWindow_ui.py
+-rw-r--r--   0 matveyev (30593) irc         (39)    11299 2023-03-14 11:26:07.000000 beamline_console-1.1.0/beamline_console/gui/MotorItemWidget_ui.py
+-rw-r--r--   0 matveyev (30593) irc         (39)    21429 2023-03-14 11:26:07.000000 beamline_console-1.1.0/beamline_console/gui/MotorPropsDialog_ui.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     4188 2023-03-14 11:26:07.000000 beamline_console-1.1.0/beamline_console/gui/SaveSnapshotDialog_ui.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     3123 2023-03-14 11:26:07.000000 beamline_console-1.1.0/beamline_console/gui/SnapshotWidget_ui.py
+-rw-r--r--   0 matveyev (30593) irc         (39)        0 2023-03-14 11:26:07.000000 beamline_console-1.1.0/beamline_console/gui/__init__.py
+-rw-r--r--   0 matveyev (30593) irc         (39)   141271 2023-03-14 11:26:07.000000 beamline_console-1.1.0/beamline_console/gui/icons_rc.py
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-06-23 08:05:53.585771 beamline_console-1.1.0/beamline_console/logger/
+-rw-r--r--   0 matveyev (30593) irc         (39)        0 2023-03-14 11:26:07.000000 beamline_console-1.1.0/beamline_console/logger/__init__.py
+-rw-r--r--   0 matveyev (30593) irc         (39)      691 2023-06-22 13:22:01.000000 beamline_console-1.1.0/beamline_console/logger/guilogger.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     1685 2023-03-14 11:26:07.000000 beamline_console-1.1.0/beamline_console/logger/highlightlogs.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     4779 2023-06-22 13:34:29.000000 beamline_console-1.1.0/beamline_console/logger/loggingwidget.py
+-rw-r--r--   0 matveyev (30593) irc         (39)      249 2023-03-14 11:26:07.000000 beamline_console-1.1.0/beamline_console/logger/logit.py
+-rw-r--r--   0 matveyev (30593) irc         (39)    10795 2023-06-22 14:06:33.000000 beamline_console-1.1.0/beamline_console/main_window.py
+-rw-r--r--   0 matveyev (30593) irc         (39)      878 2023-06-23 08:05:32.000000 beamline_console-1.1.0/beamline_console/release.py
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-06-23 08:05:53.585771 beamline_console-1.1.0/beamline_console/snapshot/
+-rw-r--r--   0 matveyev (30593) irc         (39)        0 2023-03-14 11:26:07.000000 beamline_console-1.1.0/beamline_console/snapshot/__init__.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     8949 2023-03-14 11:26:07.000000 beamline_console-1.1.0/beamline_console/snapshot/beamsnapshot.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     5979 2023-03-14 11:26:07.000000 beamline_console-1.1.0/beamline_console/snapshot/savesnapshotdialog.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     5553 2023-03-14 11:26:07.000000 beamline_console-1.1.0/beamline_console/snapshot/snapshotmanager.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     9284 2023-03-14 11:26:07.000000 beamline_console-1.1.0/beamline_console/snapshot/snapshotwidget.py
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-06-23 08:05:53.585771 beamline_console-1.1.0/beamline_console/utils/
+-rw-r--r--   0 matveyev (30593) irc         (39)        0 2023-03-14 11:26:07.000000 beamline_console-1.1.0/beamline_console/utils/__init__.py
+-rw-r--r--   0 matveyev (30593) irc         (39)      868 2023-03-14 11:26:07.000000 beamline_console-1.1.0/beamline_console/utils/aboutdialog.py
+-rw-r--r--   0 matveyev (30593) irc         (39)      868 2023-03-14 11:26:07.000000 beamline_console-1.1.0/beamline_console/utils/clickablelabel.py
+-rw-r--r--   0 matveyev (30593) irc         (39)      815 2023-06-22 14:02:54.000000 beamline_console-1.1.0/beamline_console/utils/errordialog.py
+-rw-r--r--   0 matveyev (30593) irc         (39)    12914 2023-03-14 11:26:07.000000 beamline_console-1.1.0/beamline_console/utils/functions.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     4092 2023-03-14 11:26:07.000000 beamline_console-1.1.0/beamline_console/utils/input_dialog.py
+-rwxr-xr-x   0 matveyev (30593) irc         (39)     9475 2023-03-14 11:26:07.000000 beamline_console-1.1.0/beamline_console/utils/range_slider.py
+-rw-r--r--   0 matveyev (30593) irc         (39)     1879 2023-03-14 11:26:07.000000 beamline_console-1.1.0/beamline_console/utils/settings.py
+drwxr-xr-x   0 matveyev (30593) irc         (39)        0 2023-06-23 08:05:53.581771 beamline_console-1.1.0/beamline_console.egg-info/
+-rw-r--r--   0 matveyev (30593) irc         (39)      732 2023-06-23 08:05:53.000000 beamline_console-1.1.0/beamline_console.egg-info/PKG-INFO
+-rw-r--r--   0 matveyev (30593) irc         (39)     2769 2023-06-23 08:05:53.000000 beamline_console-1.1.0/beamline_console.egg-info/SOURCES.txt
+-rw-r--r--   0 matveyev (30593) irc         (39)        1 2023-06-23 08:05:53.000000 beamline_console-1.1.0/beamline_console.egg-info/dependency_links.txt
+-rw-r--r--   0 matveyev (30593) irc         (39)       60 2023-06-23 08:05:53.000000 beamline_console-1.1.0/beamline_console.egg-info/entry_points.txt
+-rw-r--r--   0 matveyev (30593) irc         (39)       57 2023-06-23 08:05:53.000000 beamline_console-1.1.0/beamline_console.egg-info/requires.txt
+-rw-r--r--   0 matveyev (30593) irc         (39)       17 2023-06-23 08:05:53.000000 beamline_console-1.1.0/beamline_console.egg-info/top_level.txt
+-rw-r--r--   0 matveyev (30593) irc         (39)       75 2023-06-23 08:05:53.585771 beamline_console-1.1.0/setup.cfg
+-rw-r--r--   0 matveyev (30593) irc         (39)     2457 2023-03-14 11:26:07.000000 beamline_console-1.1.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `beamline_console-1.0.0/LICENSE.txt` & `beamline_console-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `beamline_console-1.0.0/PKG-INFO` & `beamline_console-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beamline_console
-Version: 1.0.0
+Version: 1.1.0
 Summary: GUI for experimental control
 Home-page: UNKNOWN
 Author: Yury Matveev
 Author-email: yury.matveev@desy.de
 License: GPLv3
 Download-URL: https://gitlab.desy.de/yury.matveev/beamline_console.git
 Description: GUI for experimental control
```

### Comparing `beamline_console-1.0.0/beamline_console/__init__.py` & `beamline_console-1.1.0/beamline_console/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -133,15 +133,17 @@
     args = get_options(sys.argv)
     setup_logger(args)
 
     app = QtWidgets.QApplication([])
     sys.excepthook = excepthook
 
     mainWindow = ExperimentalControl(args)
-    mainWindow.show()
-
-    app.exec_()
+    if mainWindow.finish_init():
+        mainWindow.show()
+        app.exec_()
+    else:
+        mainWindow.exit_program(True)
 
 # --------------------------------------------------------------------
 # Start Qt event loop unless running in interactive mode.
 if __name__ == '__main__':
     main()
```

### Comparing `beamline_console-1.0.0/beamline_console/base_widget.py` & `beamline_console-1.1.0/beamline_console/base_widget.py`

 * *Files identical despite different names*

### Comparing `beamline_console-1.0.0/beamline_console/beamlinehal.py` & `beamline_console-1.1.0/beamline_console/beamlinehal.py`

 * *Files identical despite different names*

### Comparing `beamline_console-1.0.0/beamline_console/constants.py` & `beamline_console-1.1.0/beamline_console/constants.py`

 * *Files identical despite different names*

### Comparing `beamline_console-1.0.0/beamline_console/default_config/main.cfg` & `beamline_console-1.1.0/beamline_console/default_config/main.cfg`

 * *Files identical despite different names*

### Comparing `beamline_console-1.0.0/beamline_console/devicecontrol/beamlinegraphicsscene.py` & `beamline_console-1.1.0/beamline_console/devicecontrol/beamlinegraphicsscene.py`

 * *Files identical despite different names*

### Comparing `beamline_console-1.0.0/beamline_console/devicecontrol/beamlinewidget.py` & `beamline_console-1.1.0/beamline_console/devicecontrol/beamlinewidget.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,14 +26,17 @@
         BaseWidget.__init__(self, parent)
 
         self._ui = Ui_BeamlineWidget()
         self._ui.setupUi(self)
 
         self._access_level = "user"
 
+    # ----------------------------------------------------------------------
+    def finish_init(self):
+
         # widget displaying currently selected devices
         self._ui.device_widget.initialize(self._beamline_hal, self._settings)
         self._ui.device_widget.save_snapshot.connect(lambda selection: self.save_snapshot.emit(selection))
         self._selected_devices = []          # support multi-selection of devices
 
         self._ui.beamline_view.setFixedHeight(int(self._settings.option("beamline_ui", "section_height"))+25)
```

### Comparing `beamline_console-1.0.0/beamline_console/devicecontrol/devicehistorydialog.py` & `beamline_console-1.1.0/beamline_console/devicecontrol/devicehistorydialog.py`

 * *Files identical despite different names*

### Comparing `beamline_console-1.0.0/beamline_console/devicecontrol/deviceitem/devicegraphicsitem.py` & `beamline_console-1.1.0/beamline_console/devicecontrol/deviceitem/devicegraphicsitem.py`

 * *Files identical despite different names*

### Comparing `beamline_console-1.0.0/beamline_console/devicecontrol/deviceitem/frameitem.py` & `beamline_console-1.1.0/beamline_console/devicecontrol/deviceitem/frameitem.py`

 * *Files identical despite different names*

### Comparing `beamline_console-1.0.0/beamline_console/devicecontrol/deviceitem/statusitem.py` & `beamline_console-1.1.0/beamline_console/devicecontrol/deviceitem/statusitem.py`

 * *Files identical despite different names*

### Comparing `beamline_console-1.0.0/beamline_console/devicecontrol/deviceitem/titleitem.py` & `beamline_console-1.1.0/beamline_console/devicecontrol/deviceitem/titleitem.py`

 * *Files identical despite different names*

### Comparing `beamline_console-1.0.0/beamline_console/devicecontrol/devicewidget.py` & `beamline_console-1.1.0/beamline_console/devicecontrol/devicewidget.py`

 * *Files identical despite different names*

### Comparing `beamline_console-1.0.0/beamline_console/devicecontrol/motoritemwidget.py` & `beamline_console-1.1.0/beamline_console/devicecontrol/motoritemwidget.py`

 * *Files identical despite different names*

### Comparing `beamline_console-1.0.0/beamline_console/devicecontrol/motorpropsdialog.py` & `beamline_console-1.1.0/beamline_console/devicecontrol/motorpropsdialog.py`

 * *Files identical despite different names*

### Comparing `beamline_console-1.0.0/beamline_console/devices/abstractmotor.py` & `beamline_console-1.1.0/beamline_console/devices/abstractmotor.py`

 * *Files identical despite different names*

### Comparing `beamline_console-1.0.0/beamline_console/devices/dummymotor.py` & `beamline_console-1.1.0/beamline_console/devices/dummymotor.py`

 * *Files identical despite different names*

### Comparing `beamline_console-1.0.0/beamline_console/devices/motordevice.py` & `beamline_console-1.1.0/beamline_console/devices/motordevice.py`

 * *Files identical despite different names*

### Comparing `beamline_console-1.0.0/beamline_console/devices/tangomotor.py` & `beamline_console-1.1.0/beamline_console/devices/tangomotor.py`

 * *Files identical despite different names*

### Comparing `beamline_console-1.0.0/beamline_console/gui/AboutDialog_ui.py` & `beamline_console-1.1.0/beamline_console/gui/AboutDialog_ui.py`

 * *Files identical despite different names*

### Comparing `beamline_console-1.0.0/beamline_console/gui/BeamlineWidget_ui.py` & `beamline_console-1.1.0/beamline_console/gui/BeamlineWidget_ui.py`

 * *Files identical despite different names*

### Comparing `beamline_console-1.0.0/beamline_console/gui/DeviceItem_ui.py` & `beamline_console-1.1.0/beamline_console/gui/DeviceItem_ui.py`

 * *Files identical despite different names*

### Comparing `beamline_console-1.0.0/beamline_console/gui/DeviceWidget_ui.py` & `beamline_console-1.1.0/beamline_console/gui/DeviceWidget_ui.py`

 * *Files identical despite different names*

### Comparing `beamline_console-1.0.0/beamline_console/gui/ErrorDialog_ui.py` & `beamline_console-1.1.0/beamline_console/gui/ErrorDialog_ui.py`

 * *Files identical despite different names*

### Comparing `beamline_console-1.0.0/beamline_console/gui/InputDialog_ui.py` & `beamline_console-1.1.0/beamline_console/gui/InputDialog_ui.py`

 * *Files identical despite different names*

### Comparing `beamline_console-1.0.0/beamline_console/gui/LoggingWidget_ui.py` & `beamline_console-1.1.0/beamline_console/gui/LoggingWidget_ui.py`

 * *Files identical despite different names*

### Comparing `beamline_console-1.0.0/beamline_console/gui/MainWindow_ui.py` & `beamline_console-1.1.0/beamline_console/gui/MainWindow_ui.py`

 * *Files identical despite different names*

### Comparing `beamline_console-1.0.0/beamline_console/gui/MotorItemWidget_ui.py` & `beamline_console-1.1.0/beamline_console/gui/MotorItemWidget_ui.py`

 * *Files identical despite different names*

### Comparing `beamline_console-1.0.0/beamline_console/gui/MotorPropsDialog_ui.py` & `beamline_console-1.1.0/beamline_console/gui/MotorPropsDialog_ui.py`

 * *Files identical despite different names*

### Comparing `beamline_console-1.0.0/beamline_console/gui/SaveSnapshotDialog_ui.py` & `beamline_console-1.1.0/beamline_console/gui/SaveSnapshotDialog_ui.py`

 * *Files identical despite different names*

### Comparing `beamline_console-1.0.0/beamline_console/gui/SnapshotWidget_ui.py` & `beamline_console-1.1.0/beamline_console/gui/SnapshotWidget_ui.py`

 * *Files identical despite different names*

### Comparing `beamline_console-1.0.0/beamline_console/gui/icons_rc.py` & `beamline_console-1.1.0/beamline_console/gui/icons_rc.py`

 * *Files identical despite different names*

### Comparing `beamline_console-1.0.0/beamline_console/logger/guilogger.py` & `beamline_console-1.1.0/beamline_console/logger/guilogger.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,8 +13,8 @@
     # ----------------------------------------------------------------------
     def __init__(self):
         QtCore.QObject.__init__(self)
         StreamHandler.__init__(self)
 
     # ----------------------------------------------------------------------
     def emit(self, record):
-        self.emit_record.emit(int(record.levelno) ,f'{record.asctime.split(",")[0]} {record.levelname} {record.msg}')
+        self.emit_record.emit(int(record.levelno), f'{record.asctime.split(",")[0]} {record.levelname} {record.msg}')
```

### Comparing `beamline_console-1.0.0/beamline_console/logger/highlightlogs.py` & `beamline_console-1.1.0/beamline_console/logger/highlightlogs.py`

 * *Files identical despite different names*

### Comparing `beamline_console-1.0.0/beamline_console/logger/loggingwidget.py` & `beamline_console-1.1.0/beamline_console/logger/loggingwidget.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,18 @@
         self._ui.cb_log_level.currentIndexChanged.connect(self._display_logs)
 
         self._highlighter = self._setup_text_edit()
 
         self.read_log()
 
     # ----------------------------------------------------------------------
+    def access_level_changed(self):
+        pass
+
+    # ----------------------------------------------------------------------
     def get_record(self, log_level, message):
 
         if len(self._logs_buffer) > BUFFER_SIZE:        # circular buffer
             self._logs_buffer.pop(0)
 
         self._logs_buffer.append((log_level, message))
         self._display_logs()
```

### Comparing `beamline_console-1.0.0/beamline_console/main_window.py` & `beamline_console-1.1.0/beamline_console/main_window.py`

 * *Files 15% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 from beamline_console.utils.errordialog import ErrormsgLogger
 from beamline_console.utils.settings import Settings
 from beamline_console.utils.input_dialog import InputDialog
 
 from beamline_console.gui.MainWindow_ui import Ui_MainWindow
 
 logger = logging.getLogger(APP_NAME)
+gui_settings = QtCore.QSettings(APP_NAME)
+
 
 # ----------------------------------------------------------------------
 class ExperimentalControl(QtWidgets.QMainWindow):
     """
     """
     windowClosed = QtCore.pyqtSignal()
 
@@ -85,100 +87,111 @@
 
         self.setCentralWidget(None)
 
         self.setDockOptions(QtWidgets.QMainWindow.AnimatedDocks |
                             QtWidgets.QMainWindow.AllowNestedDocks |
                             QtWidgets.QMainWindow.AllowTabbedDocks)
 
-        self._beamline_widget, self._beamline_dock = \
-            self._add_dock(BeamlineWidget, "Beamline Control", QtCore.Qt.LeftDockWidgetArea, self)
+        self.widgets = []
 
-        self._snapshot_widget, self._snapshot_dock = \
-            self._add_dock(SnapshotWidget, "Beamline Snapshots", QtCore.Qt.LeftDockWidgetArea, self)
+        try:
+            self.restoreGeometry(gui_settings.value("mainWindow/geometry"))
+            self.restoreState(gui_settings.value("mainWindow/state"))
+        except:
+            pass
 
-        self._logging_widget, self._logging_dock = \
-            self._add_dock(LoggingWidget, "Logs", QtCore.Qt.RightDockWidgetArea, self)
+        self._init_status_bar()
 
-        # Cross-connection signals
+        self._refresh_status_timer = QtCore.QTimer(self)
+        self._refresh_status_timer.timeout.connect(self._refresh_status_bar)
+        self._refresh_status_timer.start(1000)
 
-        self._gui_logger.emit_record.connect(self._logging_widget.get_record)
+    # ----------------------------------------------------------------------
+    def finish_init(self):
+        try:
+            logging_widget = LoggingWidget(self)
+            self._add_dock(logging_widget, "Logs")
+            logging_widget.load_ui_settings(gui_settings)
+            self._gui_logger.emit_record.connect(logging_widget.get_record)
+            self.widgets.append(logging_widget)
+        except Exception as err:
+            logger.error(f"Cannot initialize log widget: {err}")
+            return
 
-        self._beamline_widget.save_snapshot.connect(self._snapshot_widget.save_snapshot)
-        self._beamline_widget.device_selected.connect(self._snapshot_widget.device_selected)
+        try:
+            snapshot_widget = SnapshotWidget(self)
+            self._add_dock(snapshot_widget, "Beamline Snapshots")
+            snapshot_widget.load_ui_settings(gui_settings)
+            self.widgets.append(snapshot_widget)
+        except Exception as err:
+            logger.error(f"Cannot initialize snapshots widget: {err}")
+            return
 
-        self._snapshot_widget.motors_moved.connect(self._beamline_widget.sync_control_widget)
+        try:
+            beamline_widget = BeamlineWidget(self)
+            self._add_dock(beamline_widget, "Beamline Control")
+            beamline_widget.load_ui_settings(gui_settings)
+            self.widgets.append(beamline_widget)
+        except Exception as err:
+            logger.error(f"Cannot initialize control widget: {err}")
+            return
 
-        dev_list = list(self.beamline_hal.device_map.keys())
-        if len(dev_list) == 1:
-            self._snapshot_widget.device_selected(dev_list)
+        try:
+            beamline_widget.finish_init()
+        except Exception as err:
+            logger.error(f"Cannot initialize control widget: {err}")
+            return
 
-        self._load_ui_settings()
+        # Cross-connection signals
+        beamline_widget.save_snapshot.connect(snapshot_widget.save_snapshot)
+        beamline_widget.device_selected.connect(snapshot_widget.device_selected)
 
-        self._refresh_status_timer = QtCore.QTimer(self)
-        self._refresh_status_timer.timeout.connect(self._refresh_status_bar)
-        self._refresh_status_timer.start(1000)
+        snapshot_widget.motors_moved.connect(beamline_widget.sync_control_widget)
 
-        self._init_status_bar()
+        dev_list = list(self.beamline_hal.device_map.keys())
+        if len(dev_list) == 1:
+            snapshot_widget.device_selected(dev_list)
+
+        self.widgets = [beamline_widget, snapshot_widget, logging_widget]
 
         logger.info("Beamline console successfully initialized")
 
     # ----------------------------------------------------------------------
-    def _add_dock(self, WidgetClass, label, location, *args, **kwargs):
+    def _add_dock(self, widget, label):
         """
         """
-        widget = WidgetClass(*args, **kwargs)
-    
+
         dock = QtWidgets.QDockWidget(label)
         dock.setContextMenuPolicy(QtCore.Qt.CustomContextMenu)
         dock.setFocusPolicy(QtCore.Qt.StrongFocus)
         dock._currentWindow = '0'
         dock.setObjectName("{}Dock".format("".join(label.split())))
         dock.setWidget(widget)
 
-        self.addDockWidget(location, dock)
+        self.addDockWidget(QtCore.Qt.LeftDockWidgetArea, dock)
         self._dockList.append(dock)
         self.menu_view.addAction(dock.toggleViewAction())
 
-        return widget, dock
-
     # ----------------------------------------------------------------------
     def _stop_beamline(self):
         """
         """
         self.beamline_hal.stop_all()
         self.beamline_hal.safe_close()
      
     # ----------------------------------------------------------------------  
     def _save_ui_settings(self):
         """Save GUI state using QT settings mechanism.
         """
-        settings = QtCore.QSettings(APP_NAME)
-  
-        self._beamline_widget.save_ui_settings(settings)
-        self._snapshot_widget.save_ui_settings(settings)
-        self._logging_widget.save_ui_settings(settings)
 
-        settings.setValue("mainWindow/state", self.saveState())
-        settings.setValue("mainWindow/geometry", self.saveGeometry())
+        for widget in self.widgets:
+            widget.save_ui_settings(gui_settings)
 
-    # ----------------------------------------------------------------------
-    def _load_ui_settings(self):
-        """Load GUI state using QT settings system.
-        """
-        settings = QtCore.QSettings(APP_NAME)
-
-        try:
-            self.restoreGeometry(settings.value("mainWindow/geometry"))
-            self.restoreState(settings.value("mainWindow/state"))
-        except:
-            pass
-
-        self._beamline_widget.load_ui_settings(settings)
-        self._snapshot_widget.load_ui_settings(settings)
-        self._logging_widget.load_ui_settings(settings)
+        gui_settings.setValue("mainWindow/state", self.saveState())
+        gui_settings.setValue("mainWindow/geometry", self.saveGeometry())
 
     # ----------------------------------------------------------------------
     def _init_status_bar(self):
 
         # move progressbar TODO
         self.pb_movement = QtWidgets.QProgressBar()
         self.pb_movement.setMaximumSize(2000, 25)
@@ -204,21 +217,21 @@
         """
         """
         try:
             if self.beamline_hal.access_level != 'superuser':
                 if InputDialog(mode="pin", super_user_password=int(self.settings.option("general", "superuser_pin")),
                                max_attempts=int(self.settings.option("general", "max_attempts"))).exec():
                     self.beamline_hal.access_level_changed('superuser')
-                    self._beamline_widget.access_level_changed('superuser')
-                    self._snapshot_widget.access_level_changed('superuser')
+                    for widget in self.widgets:
+                        widget.access_level_changed('superuser')
                     self.action_user.setText('Disable superuser')
             else:
                 self.beamline_hal.access_level_changed('user')
-                self._beamline_widget.access_level_changed('superuser')
-                self._snapshot_widget.access_level_changed('superuser')
+                for widget in self.widgets:
+                    widget.access_level_changed('user')
                 self.action_user.setText('Enable superuser')
 
         except Exception as err:
             logger.error(f"Authorization Failed: {repr(err)}", exc_info=sys.exc_info())
 
     # ----------------------------------------------------------------------
     def _refresh_status_bar(self):
@@ -244,25 +257,26 @@
         """
         if self._clean_exit():
             event.accept()  
         else:  
             event.ignore()  
 
     # ----------------------------------------------------------------------
-    def exit_program(self):
+    def exit_program(self, force=False):
         """Called when Quit action is triggered.
         """
-        if self._clean_exit():
+        if self._clean_exit(force):
             QtWidgets.qApp.quit()
 
     # ----------------------------------------------------------------------
-    def _clean_exit(self):
+    def _clean_exit(self, force=False):
         """
         """ 
-        if self._really_quit():
+        really_quit = True if force else self._really_quit()
+        if really_quit:
             self._refresh_status_timer.stop()
             self._stop_beamline()
             # unlockAppInstance(self._lockFileName)
             self._save_ui_settings()
             QtWidgets.qApp.clipboard().clear()
             return True
```

### Comparing `beamline_console-1.0.0/beamline_console/release.py` & `beamline_console-1.1.0/beamline_console/release.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 class Release:
     """Summarize release information as class attributes.
     """
 
     name = 'beamline_console'
-    version_info = (1, 0, 0)
+    version_info = (1, 1, 0)
     version = '.'.join(map(str, version_info[:3]))
     release = ''.join(map(str, version_info[3:]))
     separator = '.' if 'dev' in release or 'post' in release else ''
     version_long = version + separator + release
 
     version_number = int(version.replace('.', ''))
     long_description = description = 'GUI for experimental control'
```

### Comparing `beamline_console-1.0.0/beamline_console/snapshot/beamsnapshot.py` & `beamline_console-1.1.0/beamline_console/snapshot/beamsnapshot.py`

 * *Files identical despite different names*

### Comparing `beamline_console-1.0.0/beamline_console/snapshot/savesnapshotdialog.py` & `beamline_console-1.1.0/beamline_console/snapshot/savesnapshotdialog.py`

 * *Files identical despite different names*

### Comparing `beamline_console-1.0.0/beamline_console/snapshot/snapshotmanager.py` & `beamline_console-1.1.0/beamline_console/snapshot/snapshotmanager.py`

 * *Files identical despite different names*

### Comparing `beamline_console-1.0.0/beamline_console/snapshot/snapshotwidget.py` & `beamline_console-1.1.0/beamline_console/snapshot/snapshotwidget.py`

 * *Files identical despite different names*

### Comparing `beamline_console-1.0.0/beamline_console/utils/aboutdialog.py` & `beamline_console-1.1.0/beamline_console/utils/aboutdialog.py`

 * *Files identical despite different names*

### Comparing `beamline_console-1.0.0/beamline_console/utils/clickablelabel.py` & `beamline_console-1.1.0/beamline_console/utils/clickablelabel.py`

 * *Files identical despite different names*

### Comparing `beamline_console-1.0.0/beamline_console/utils/errordialog.py` & `beamline_console-1.1.0/beamline_console/utils/errordialog.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
     # ----------------------------------------------------------------------
     def emit(self, record):
         if record.levelno >= 40:
             ErrorDialog(record.msg).exec_()
 
 
+
 # ----------------------------------------------------------------------
 class ErrorDialog(QtWidgets.QDialog):
     """
     """
 
     # ---------------------------------------------------------------------- 
     def __init__(self, record):
```

### Comparing `beamline_console-1.0.0/beamline_console/utils/functions.py` & `beamline_console-1.1.0/beamline_console/utils/functions.py`

 * *Files identical despite different names*

### Comparing `beamline_console-1.0.0/beamline_console/utils/input_dialog.py` & `beamline_console-1.1.0/beamline_console/utils/input_dialog.py`

 * *Files identical despite different names*

### Comparing `beamline_console-1.0.0/beamline_console/utils/range_slider.py` & `beamline_console-1.1.0/beamline_console/utils/range_slider.py`

 * *Files identical despite different names*

### Comparing `beamline_console-1.0.0/beamline_console/utils/settings.py` & `beamline_console-1.1.0/beamline_console/utils/settings.py`

 * *Files identical despite different names*

### Comparing `beamline_console-1.0.0/beamline_console.egg-info/PKG-INFO` & `beamline_console-1.1.0/beamline_console.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beamline-console
-Version: 1.0.0
+Version: 1.1.0
 Summary: GUI for experimental control
 Home-page: UNKNOWN
 Author: Yury Matveev
 Author-email: yury.matveev@desy.de
 License: GPLv3
 Download-URL: https://gitlab.desy.de/yury.matveev/beamline_console.git
 Description: GUI for experimental control
```

### Comparing `beamline_console-1.0.0/beamline_console.egg-info/SOURCES.txt` & `beamline_console-1.1.0/beamline_console.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `beamline_console-1.0.0/setup.py` & `beamline_console-1.1.0/setup.py`

 * *Files identical despite different names*

